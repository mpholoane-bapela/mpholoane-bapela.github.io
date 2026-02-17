---
title: "GitHub Copilot Model Showdown – Visual Studio 2026 Speed Test"
tags: [AI, GitHubCopilot, DeveloperTools]
---

# GitHub Copilot Model Showdown – Visual Studio 2026 Speed Test

GitHub Copilot gives you access to multiple AI coding models under a single subscription—but **speed, focus, and cost** vary widely. I decided to put them head-to-head in **Visual Studio 2026** to see which ones actually deliver on real coding tasks. Spoiler: the differences are bigger than you might think.

---

## The Task

I chose a realistic, repetitive challenge: **refactor six repository classes from synchronous to async patterns** with proper **Entity Framework Core** optimization.

**Original code snippet:**
```csharp
public IQueryable<ResultCheckSumSa> GetAll()
{
    return _repository.Query<ResultCheckSumSa>();
}
````

**Target refactor:**

```csharp
public async Task<IReadOnlyList<ResultCheckSumSa>> GetAll()
{
    return await GetAllQuery().ToListAsync() 
        as IReadOnlyList<ResultCheckSumSa>;
}

private IQueryable<ResultCheckSumSa> GetAllQuery()
{
    return _repository.GetAll<ResultCheckSumSa>()
        .AsNoTracking();
}
```

**Key changes required:**

* Add async/await patterns
* Replace `Query<T>()` with `GetAll<T>()`
* Apply `.AsNoTracking()` for read-only queries
* Extract helper methods to reduce duplication
* Update return types to `Task<T>`

> A human developer could complete this in ~15–20 minutes. How would AI stack up?

---

## Contestants

**Premium Tier:**

* Claude Sonnet 4.5
* ChatGPT 5
* Claude Haiku 4.5

**Free Tier:**

* Grok Fast
* ChatGPT 5 Mini

> *(Grok Fast was warmed up before timing to avoid cold-start lag.)*

---

## The Results

| Model             | Time     | Notes                     |
| ----------------- | -------- | ------------------------- |
| Claude Sonnet 4.5 | 90 sec   | Laser-focused, zero fluff |
| ChatGPT 5         | 90 sec   | Fast, but verbose         |
| Claude Haiku 4.5  | 2.5 min  | Solid budget option       |
| Grok Fast         | 2.5 min* | First run: 5 min          |
| ChatGPT 5 Mini    | 4.25 min | Drifted off-task          |

---

## Model Personalities

**Claude Sonnet 4.5 – The Efficient Specialist**

* 90 seconds, $0.02 per task
* Applied all changes exactly, no commentary
* Like a senior developer who reads the ticket and delivers

**ChatGPT 5 – The Overexplainer**

* Same speed, but full of suggestions and alternative ideas
* Correct work, sometimes distracting

**Claude Haiku 4.5 – The Budget Player**

* 2.5 minutes, inexpensive, accurate, slightly slower finish

**Grok Fast – The Slow Starter**

* First run: 5 min; subsequent: 2.5 min
* Backend caching or warm-up effects likely

**ChatGPT 5 Mini – The Distracted Freebie**

* 4+ minutes, explored unrelated files
* Free, but context-breaking

<img src="/assets/img/posts/2026/02_Feb/17-SpeedTests/Info-02.png" 
     alt="Speed Test Results" 
     style="max-width: 100%; height: auto;" 
     loading="lazy">

---

## Premium vs Free

* Occasional refactors → free models are fine
* Daily use → premium models **save time and preserve focus**

Example: Claude Sonnet 4.5 → 90 sec vs 4+ min for free

> Saves ~2.5 hours/week and keeps you in flow

---

## Takeaways

* **Speed and focus matter more than price alone**
* Premium models excel on repetitive, targeted refactors
* Free models are OK for casual use but can cost time in context switching
* IDE integration often matters more than raw model speed

---

## Recommendations

* **Fast & precise:** Claude Sonnet 4.5 or ChatGPT 5
* **Focus without noise:** Claude Sonnet 4.5
* **Budget-conscious:** Claude Haiku 4.5
* **Learning/exploration:** ChatGPT 5

---

## Watch the Full Test

Check out the **full video** comparing all five models, including bonus web chat experiments:

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%;">
  <iframe src="https://www.youtube.com/embed/Lpdf8BC7BWs" 
          frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
          allowfullscreen 
          style="position: absolute; top:0; left: 0; width: 100%; height: 100%;">
  </iframe>
</div>

---
