---
theme: default
background: https://source.unsplash.com/1600x900/?technology,dark
class: text-center
highlighter: shiki
drawings:
  persist: false
transition: fade
title: Claude 3.7 Sonnet
mdc: true
---

# Claude 3.7 Sonnet

<div class="text-6xl font-bold text-gradient-red-blue mb-4">100 SECONDS OF KNOWLEDGE</div>

<div class="abs-br m-6 flex gap-2 text-xl">
  <a href="https://github.com/brylie/create-with-brylie" target="_blank" class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />&nbsp;
    github.com/brylie
  </a>
</div>

<!--
Claude 3.7 Sonnet just dropped and it's changing the AI game. I'm going to break down this monster in just 100 seconds.
-->

---
layout: default
---

# What is Claude 3.7?

<div class="text-xl mt-2">
  <div class="grid grid-cols-2 gap-16">
    <div>
      <div class="text-5xl font-bold mb-4 text-purple-400">The Ferrari of AI models</div>
      <div class="text-base opacity-70">Full name: Claude 3.7 Sonnet</div>
      <div class="text-base opacity-70">Released: February 2025</div>
      <div class="text-base opacity-70">Made by: Anthropic</div>
      <div class="mt-8 text-lg">
        Fast when you need it. Careful when it matters. Production-ready for the real world.
      </div>
    </div>
    <div class="flex items-center justify-center">
      <div class="text-center">
        <div class="flex justify-center">
          <carbon:rocket class="text-9xl text-blue-500"/>
        </div>
        <div class="text-2xl font-bold mt-4">State-of-the-art performance</div>
      </div>
    </div>
  </div>
</div>

<!--
Claude 3.7 is Anthropic's latest AI model blowing up the charts on nearly every benchmark. Think of it as the Ferrari of AI models - fast when you need it, but with the option to slow down and think carefully when the problem gets complex.
-->

---
layout: two-cols
---

# The Big Innovation: Hybrid Reasoning

<div class="text-2xl font-bold mb-6 text-green-400">Switch between:</div>

<div class="mb-4 flex items-center">
  <carbon:flash class="text-yellow-400 text-3xl mr-4"/>
  <span class="text-xl">Quick responses for simple tasks</span>
</div>

<div class="mb-4 flex items-center">
  <carbon:idea class="text-blue-400 text-3xl mr-4"/>
  <span class="text-xl">Deep thinking for complex problems</span>
</div>

<div class="text-base opacity-70 mt-8">
  First model to combine both modes in one system
</div>

::right::

```js
// Normal mode: Quick response
const quickAnswer = claude.complete("What's 2+2?"); 
// Near instant

// Extended thinking: Deep analysis 
const deepAnswer = claude.complete({
  prompt: "Solve this complex math proof...",
  extendedThinking: true // More time, higher accuracy
});
```

<!--
The killer feature? Something Anthropic calls "hybrid reasoning." Claude can now toggle between quick responses and deep, step-by-step thinking. It's like having both a sprinter and chess grandmaster in one package.
-->

---
layout: default
class: text-center
---

# Benchmark Destruction

<div class="grid grid-cols-3 gap-4 mt-12">
  <div class="flex flex-col items-center border border-gray-400 rounded-lg p-6 bg-gray-800 bg-opacity-50">
    <div class="text-5xl font-bold text-blue-400 mb-4">84.8%</div>
    <div class="text-xl">GPQA Diamond</div>
    <div class="text-sm opacity-70">(Graduate-level reasoning)</div>
  </div>
  <div class="flex flex-col items-center border border-gray-400 rounded-lg p-6 bg-gray-800 bg-opacity-50">
    <div class="text-5xl font-bold text-green-400 mb-4">80.0%</div>
    <div class="text-xl">AIME 2024</div>
    <div class="text-sm opacity-70">(High school math competition)</div>
  </div>
  <div class="flex flex-col items-center border border-gray-400 rounded-lg p-6 bg-gray-800 bg-opacity-50">
    <div class="text-5xl font-bold text-purple-400 mb-4">70.3%</div>
    <div class="text-xl">SWE-bench Verified</div>
    <div class="text-sm opacity-70">(Real software engineering tasks)</div>
  </div>
</div>

<div class="mt-12 text-xl text-yellow-400">
  Outperforming OpenAI's o1, o3-mini, and DeepSeek R1 across multiple benchmarks
</div>

<!--
Claude 3.7 is shredding the competition on benchmarks. Look at these numbers:

- GPQA Diamond: 84.8% with extended thinking
- AIME 2024 math: 80%
- SWE-bench Verified: 70.3% with scaffold

That SWE-bench result means it can solve real software engineering problems better than most junior devs.
-->

---
layout: two-cols
---

# Code Editing

<div class="text-xl mt-4">
  <div class="flex items-center mb-4">
    <carbon:checkmark-filled class="text-green-500 mr-2"/> Front-end development
  </div>
  <div class="flex items-center mb-4">
    <carbon:checkmark-filled class="text-green-500 mr-2"/> Back-end systems
  </div>
  <div class="flex items-center mb-4">
    <carbon:checkmark-filled class="text-green-500 mr-2"/> Testing and debugging
  </div>
  <div class="flex items-center mb-4">
    <carbon:checkmark-filled class="text-green-500 mr-2"/> Production-ready code
  </div>
  <div class="flex items-center mb-4">
    <carbon:checkmark-filled class="text-green-500 mr-2"/> Fewer hallucinations
  </div>
</div>

::right::

```python
import anthropic

client = anthropic.Client(
    api_key="your_key_here"
)

response = client.completions.create(
    model="claude-3-7-sonnet-20250219",
    prompt="Fix this React component that's causing memory leaks",
    max_tokens_to_sample=800,
)

print(response.completion)
```

<!--
For developers, Claude 3.7 is a game changer. It does front-end, back-end, debugging, all with fewer hallucinations and more production-ready code.
-->

---
layout: default
---

# Token Limits? What Token Limits?

<div class="grid grid-cols-2 gap-12 mt-8">
  <div class="flex flex-col items-center justify-center">
    <div class="text-8xl font-bold text-blue-500">128K</div>
    <div class="text-2xl mt-4">Tokens output limit</div>
    <div class="text-base opacity-70 mt-2">15x previous versions</div>
  </div>
  <div class="flex flex-col justify-center">
    <div class="text-xl mb-4">What can you do with 128K tokens?</div>
    <div class="flex items-center mb-3">
      <carbon:document class="text-yellow-500 mr-2"/> Generate entire codebases
    </div>
    <div class="flex items-center mb-3">
      <carbon:document class="text-yellow-500 mr-2"/> Process large datasets
    </div>
    <div class="flex items-center mb-3">
      <carbon:document class="text-yellow-500 mr-2"/> Create comprehensive analyses
    </div>
    <div class="flex items-center">
      <carbon:document class="text-yellow-500 mr-2"/> Write full technical documentation
    </div>
  </div>
</div>

<!--
Remember when AI models had tiny context windows? Claude 3.7 laughs at that with a massive 128,000 token output limit. That's about 15 times more than previous versions. Want to generate an entire codebase? Now you can.
-->

---
layout: default
---

# Claude Code - Your AI Pair Programmer

<div class="grid grid-cols-2 gap-8 mt-8">
  <div>
    <div class="text-xl mb-6">A revolutionary command-line tool</div>
    <div class="flex items-center mb-4">
      <carbon:search class="text-blue-400 mr-2"/> Search and read codebases
    </div>
    <div class="flex items-center mb-4">
      <carbon:edit class="text-blue-400 mr-2"/> Edit files intelligently
    </div>
    <div class="flex items-center mb-4">
      <carbon:chemistry class="text-blue-400 mr-2"/> Write and run tests
    </div>
    <div class="flex items-center mb-4">
      <carbon:cloud class="text-blue-400 mr-2"/> Commit directly to GitHub
    </div>
    <div class="flex items-center mb-4">
      <carbon:terminal class="text-blue-400 mr-2"/> Execute command-line tools
    </div>
  </div>
  <div class="flex flex-col justify-center">
    <div class="bg-gray-900 p-4 rounded-lg font-mono text-sm">
      <div class="text-gray-400">$</div>
      <div class="text-green-400">claude-code "Refactor our authentication system to use JWT"</div>
      <div class="text-gray-300 mt-2">Analyzing codebase...</div>
      <div class="text-gray-300">Found 3 files that need changes</div>
      <div class="text-gray-300">Creating JWT implementation...</div>
      <div class="text-gray-300">Running tests...</div>
      <div class="text-green-500">All tests passed! Ready to commit.</div>
    </div>
  </div>
</div>

<!--
Anthropic also dropped Claude Code, a command-line tool that's like having a senior dev watching over your shoulder. It can search codebases, write tests, commit to GitHub, and more.
-->

---
layout: default
class: text-center
---

# Real World Applications

<div class="grid grid-cols-5 gap-4 mt-12">
  <div class="flex flex-col items-center p-4">
    <carbon:chat class="text-5xl text-blue-400 mb-4"/>
    <div class="text-sm">Customer-facing Agents</div>
  </div>
  <div class="flex flex-col items-center p-4">
    <carbon:chart-line class="text-5xl text-green-400 mb-4"/>
    <div class="text-sm">Visual Data Extraction</div>
  </div>
  <div class="flex flex-col items-center p-4">
    <carbon:search class="text-5xl text-yellow-400 mb-4"/>
    <div class="text-sm">Advanced Q&A Systems</div>
  </div>
  <div class="flex flex-col items-center p-4">
    <carbon:earth class="text-5xl text-purple-400 mb-4"/>
    <div class="text-sm">Multilingual Support</div>
  </div>
  <div class="flex flex-col items-center p-4">
    <carbon:code class="text-5xl text-red-400 mb-4"/>
    <div class="text-sm">Complex Coding</div>
  </div>
</div>

<div class="mt-12 text-xl">
  Transforming industries with AI that can think, reason, and create
</div>

<!--
This isn't just theoretical. Claude 3.7 excels at:

- Customer-facing AI agents
- Visual data extraction
- Advanced Q&A systems
- Multilingual support
- Complex coding projects
-->

---
layout: default
---

# Pricing

<div class="grid grid-cols-2 gap-16 mt-12">
  <div class="flex flex-col items-center justify-center">
    <div class="text-4xl font-bold mb-4">Same pricing as before</div>
    <div class="text-2xl text-green-400 mt-6">$3</div>
    <div class="text-base">per million input tokens</div>
    <div class="text-2xl text-green-400 mt-6">$15</div>
    <div class="text-base">per million output tokens</div>
  </div>
  <div>
    <div class="text-xl mb-6">Available on:</div>
    <div class="flex items-center mb-4">
      <carbon:user class="text-blue-400 mr-2"/> Free tier (basic access)
    </div>
    <div class="flex items-center mb-4">
      <carbon:user-profile class="text-blue-400 mr-2"/> Pro tier (with extended thinking)
    </div>
    <div class="flex items-center mb-4">
      <carbon:partnership class="text-blue-400 mr-2"/> Team accounts
    </div>
    <div class="flex items-center mb-4">
      <carbon:enterprise class="text-blue-400 mr-2"/> Enterprise plans
    </div>
    <div class="flex items-center mt-8">
      <carbon:api class="text-yellow-400 mr-2"/> Accessible via API, Amazon Bedrock, and Google Cloud
    </div>
  </div>
</div>

<!--
Here's the kicker - same pricing as before: $3 per million input tokens, $15 per million output tokens. Extended thinking mode is available on all paid plans.
-->

---
layout: center
class: text-center
---

# Claude 3.7 Sonnet

<div class="text-3xl mb-8">Not just an incremental update - a new era of AI reasoning</div>

<div class="flex justify-center gap-8 mt-12">
  <div class="flex flex-col items-center">
    <carbon:idea class="text-6xl text-yellow-400 mb-4"/>
    <div>Hybrid Reasoning</div>
  </div>
  <div class="flex flex-col items-center">
    <carbon:code class="text-6xl text-blue-400 mb-4"/>
    <div>Advanced Coding</div>
  </div>
  <div class="flex flex-col items-center">
    <carbon:document class="text-6xl text-green-400 mb-4"/>
    <div>Massive Context</div>
  </div>
</div>

<div class="mt-16 text-xl opacity-80">
  Thanks for watching! Hit subscribe for more 100-second explainers.
</div>

<!--
Claude 3.7 Sonnet isn't just an incremental update - it's a fundamental shift in how AI models can reason. The combination of speed, deep thinking, and massive context windows makes this a serious contender for the AI throne.

Thanks for watching! Hit subscribe for more 100-second explainers, and remember: the AI revolution won't be televised - it'll be tokenized.
-->

---
layout: center
class: text-center
---

<div class="text-3xl mb-12">Oh, and it can operate computers like a human would...</div>

<div class="flex justify-center">
  <carbon:warning-alt class="text-6xl text-yellow-400 mb-4"/>
</div>

<div class="text-2xl mt-8 text-red-400">
  The robot uprising starts now
</div>

<div class="text-xl mt-4 opacity-70">
  Sleep tight!
</div>

<!--
Oh, and it can operate computers like a human would. Move the cursor, click buttons, type text - basically, the robot uprising starts now. Sleep tight!
-->