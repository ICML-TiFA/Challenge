---
marp: true
# theme: academic
theme: rose-pine-dawn
paginate: true
math: katex
style: pre.mermaid { all: unset; }

---
<!-- _class: lead-->
<!-- header: ICML 2024 Workshop on **T**rustworthy **i**n Multi-modal **F**oundation Models and AI **A**gents **(TiFA)** -->

# Challenges Plan

---
# Track1: Hackathon

<div class="container">

<div class="col">

#### Motivation
大模型的研究依赖算力、数据、专家等大量资源，一般研究者往往无法获取这些资源。我们希望社区提供方案以及配套的工具，以便更多的研究者参与到大模型的研究与比赛中来。

#### Proposed Topics
- 开源工具
- 比赛方案


</div>

<div class="col">

#### Program

<pre class="mermaid">
%%{init: {'theme':'neutral'}}%%
flowchart LR
subgraph Phase1
    topic[主题发布] --> signup
    signup[开放报名] --> propose[方案提交]
    propose --> community[方案评审+投票]
    expert[专家组筹建]
    expert --> community
    community --> plan[公布入选方案]
end
Phase1 --提供开发环境--> Phase2
subgraph Phase2
    pr[提交代码]
    coder[工程专家] --> cr
    pr --> cr[代码评审]
    cr --> test[平台联调]
    test --> anno[开源发布]
end

</pre>
</div>

</div>

---
# Track2: Red Teaming

<div class="container">

<div class="col">

#### Motivation

#### Proposed Topics


</div>

<div class="col">

#### Program

</div>

</div>


---
# Expected Outcomes

## 开源工具集
## 比赛方案
## Benchmark Report

---
# Resources Requirements

## 计算资源
## 数据资源
## 专家资源
## 宣传资源

---
# Timeline

<pre class="mermaid">
%%{init: {'theme':'neutral'}}%%

gantt
    %% title 安全竞赛准备日程
    dateFormat YYYY-MM-DD
    axisFormat %d/%m
    excludes    weekends

   
    section Organization
    比赛方案制定: active, plan, 2024-04-8, 2024-04-26
    Sponsor确定: active, 2024-04-15, 2024-04-26
    专家委员会组织: active, 2024-04-26, 2024-05-13
    合作协议签署+发布比赛公告: crit, milestone, signco, 2024-04-25, 1d
    结果公布: crit, milestone, 2024-07-01, 1d

    section Platform
    CI/CD准备:, 2024-05-05, 2024-05-17
    算力平台准备:, 2024-05-17, 2024-05-31
    评分模型准备:, 2024-05-05, 2024-05-31

    section 1-Hackathon
    Hackaton征集: crit, milestone, 2024-04-30, 2024-05-12
    方案评审:, 2024-05-13, 2024-05-17
    公布入选方案: crit, milestone, 2024-05-17, 1d
    选手开发: dev, 2024-05-20, 2024-05-31

    section 2-RedTeaming
    比赛进行: , 2024-05-31, 2024-06-23
    结果评审: , 2024-06-23, 2024-06-30
</pre>


---
<!-- _class: lead-->
# Come Join the Party!

<!-- Put this script at the end of Markdown file. -->
<!-- Mermaid -->
<script type="module">
import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
mermaid.initialize({ startOnLoad: true });

window.addEventListener('vscode.markdown.updateContent', function() { mermaid.init() });
</script>

