## Welcome to:
<!-- .slide: data-background="#09091e" data-transition="fade" -->

![](images/01-fcc-logo.png)

Hands-On Local AI Workshop <!-- .element: class="fragment r-fit-text" -->

OR Hands-On Private AI Workshop <!-- .element: class="fragment" -->

---
---

## <small>House Keeping &#127968; &#129529;</small>
<!-- .slide: data-transition="fade" -->

<small>&#128732; `TBD` (Encode Club)</small>
![](images/00-qr.svg)

---
---

## <small>House Keeping &#127968; &#129529;</small>
<!-- .slide: data-transition="fade" -->

![](images/00-qr-discord.svg)

---
---

## Poster
<!-- .slide: data-transition="fade" -->

![](images/00-poster-transparent.png)

---
---

## <small>Similar to:</small>
<!-- .slide: data-transition="fade" -->

![](images/01-osi-logo.svg)

---
---

## <small>Similar to:</small>
<!-- .slide: data-transition="fade" -->

![](images/02-osi-hardware-logo.svg)

---
---

## <small>What if:</small>
<!-- .slide: data-transition="fade" -->

![](images/03-open-source-ai.png)

---
---

## <small>Possible definition:</small>
<!-- .slide: data-transition="fade" -->

<small>Following the same idea behind **Open Source Software**, an **Open Source AI** is a system made available under terms that grant users the freedoms to:</small>

* Use    <!-- .element: class="fragment" -->
* Study  <!-- .element: class="fragment" -->
* Modify <!-- .element: class="fragment" -->
* Share  <!-- .element: class="fragment" -->

---

### Use

![](images/04-osi-ai-a.png)

---

### Study

![](images/04-osi-ai-b.png)

---

### Modify

![](images/04-osi-ai-c.png)

---

### Share

![](images/04-osi-ai-d.png)

---
---

## <small>Why Open Source? Use Cases?</small>
<!-- .slide: data-transition="fade" -->

- Don't want to pay $ to Silicon Valley <!-- .element: class="fragment" --> <small>(or use these hosted services online)</small> <!-- .element: class="fragment" -->
- You want something that works OFFLINE <!-- .element: class="fragment" -->
- You want PRIVACY or confidentiality <!-- .element: class="fragment" -->
- You want to avoid LATENCY issues <!-- .element: class="fragment" -->
- You want something that DOESN'T CHANGE <!-- .element: class="fragment" -->
- You want proper CUSTOMISATION <!-- .element: class="fragment" -->
- You want to save the ENVIRONMENT <!-- .element: class="fragment" -->

---

### <small>Not convinced?</small>

<small>

No ~~$~~ to BigTech: `11 Jul 2025` - [Cursor's Pricing Disaster: How a "Routine Update" Turned Into a Developer Exodus](https://www.wearefounders.uk/cursors-pricing-disaster-how-a-routine-update-turned-into-a-developer-exodus/)

OFFLINE: `10 June 2025` - [ChatGPT down: OpenAI reports major outage as users see error message](https://www.independent.co.uk/tech/chatgpt-down-outage-open-ai-broken-b2767111.html)

PRIVACY: `6 Jun 2025` - [OpenAI is storing deleted ChatGPT conversations as part of its NYT lawsuit](https://www.theverge.com/news/681280/openai-storing-deleted-chats-nyt-lawsuit)

LATENCY: `21 Apr 2025` - [Report: Amazon Says AI Rate Limits Are For "Fair Access," Not Capacity Constraints](https://www.pymnts.com/amazon/2025/report-amazon-says-ai-rate-limits-are-for-fair-access-not-capacity-constraints/)

DOESN'T CHANGE `29 Apr 2025` - [OpenAI explains why ChatGPT became too sycophantic](https://techcrunch.com/2025/04/29/openai-explains-why-chatgpt-became-too-sycophantic/)

CUSTOMISATION `01 Nov 2023` - [Is there a way to know the current SYSTEM prompt by OpenAI?](https://redd.it/17la364)

ENVIRONMENT `8 Jul 2025` - [Elon Musk xAI Importing Power Plant for New Data Center](https://aibusiness.com/data-centers/elon-musk-xai-importing-power-plant-for-new-data-center)

</small>

---
---

## <small>Why Open Source? Use Cases?</small>
<!-- .slide: data-transition="fade" -->

<small>1. Primary use case: when dealing with sensitive / private data OR your personal data</small> <!-- .element: class="fragment" -->
<small>2. Secondary use case: A.I. system that require fast inference</small> <!-- .element: class="fragment" -->

---
---

## <small>&#128736; Tools for running local LLMs</small>
<!-- .slide: data-transition="fade" -->

| Name            | Link                         |
|-----------------|------------------------------|
| Ollama          | https://ollama.com           |
| LM Studio       | https://lmstudio.ai          |
| vLLM            | https://blog.vllm.ai         |
| Others (Nomic?) | https://www.nomic.ai/gpt4all |

---
---

## <small>&nbsp;</small>
<!-- .slide: data-transition="fade" -->

![](images/05-ollama-ascii.png)

---
---

## <small>&nbsp;</small>
<!-- .slide: data-transition="fade" -->

**Ollama** is a local AI model runner. <br /> Allows users to **manage** (download / rename / rm / etc) & **infer** large language models (LLMs) locally.

---
---

## <small>Is Ollama installed?</small>
<!-- .slide: data-transition="fade" -->

```shell [1|2]
ollama --version
ollama version is 0.9.6
```

---

### <small>Ollama installation instructions MacOs?</small>
<!-- .slide: data-transition="fade" -->

<small>Full Ollama manual installation instructions can be found at **[github.com/ollama/ollama/](https://github.com/ollama/ollama/)** (use if non-admin). Download either the **ZIP** file or the **DMG** file.</small>

<small>1). Download [https://ollama.com/download/Ollama-darwin.zip](https://ollama.com/download/Ollama-darwin.zip) or [https://ollama.com/download/Ollama.dmg](https://ollama.com/download/Ollama.dmg). Then unzip then drag-n-drop the file into /Applications or Double-click on the DMG file then drag-n-drop</small>

<small>2). Open it from your Launchpad. Check the icon next to the clock. To test, open Terminal and type `ollama run qwen`</small>

---

### <small>Ollama installation instructions Win?</small>
<!-- .slide: data-transition="fade" -->

Ollama manual installation info can be found at [github.com/ollama/ollama/blob/main/docs/windows.md](https://github.com/ollama/ollama/blob/main/docs/windows.md) (use if non-admin). Download the OllamaSetup EXE file.

<small>1). Download [ollama.com/download/OllamaSetup.exe](ollama.com/download/OllamaSetup.exe) - Double-click and follow the instructions. Make Sure Ollama Is Running in the Background. Check the icon next to the clock and don't forget, you can stop it / startup enable it from TaskManager.</small>

<small>2). Open it from your Start. To test, open Cmd and type `ollama run qwen`</small>

---

### <small>Ollama installation instructions Linux?</small>
<!-- .slide: data-transition="fade" -->

```sh
curl -fsSL https://ollama.com/install.sh | sh
```

---
---

## <small></small>
<!-- .slide: data-transition="fade" -->

```txt [1:7-18|12|14|10|15|7]
> ollama
Usage:
  ollama [flags]
  ollama [command]

Available Commands:
  serve       Start ollama
  create      Create a model from a Modelfile
  show        Show information for a model
  run         Run a model
  stop        Stop a running model
  pull        Pull a model from a registry
  push        Push a model to a registry
  list        List models
  ps          List running models
  cp          Copy a model
  rm          Remove a model
  help        Help about any command

Flags:
  -h, --help      help for ollama
  -v, --version   Show version information

Use "ollama [command] --help" for more information about a command.
```

---
---

## <small>Pull Command (1 of 5)</small>
<!-- .slide: data-transition="fade" -->

`ollama pull ModelName` <!-- class="fragment r-fit-text" -->

---

## <small>Pull Command (1 of 5)</small>
<!-- .slide: data-transition="fade" -->

[https://ollama.com/search](https://ollama.com/search)

<small>

| Model              | Parameters | Size  | Download                          |
|--------------------|------------|-------|-----------------------------------|
| Qwen 3             | 0.6B       | 523MB | `ollama pull qwen3:0.6b`          |
| Qwen 3             | 4B         | 2.6GB | `ollama pull qwen3:4b`            |
| Qwen 3             | 8B         | 5.2GB | `ollama pull qwen3:8b`            |
| Qwen 3             | 235B-a22b  | 142GB | `ollama pull qwen3:235b`          |
| Gemma 3            | 1B         | 815MB | `ollama pull gemma3:1b`           |
| Gemma 3            | 4B         | 3.3GB | `ollama pull gemma3`              |
| Gemma 3            | 12B        | 8.1GB | `ollama pull gemma3:12b`          |
| Gemma 3            | 27B        | 17GB  | `ollama pull gemma3:27b`          |
| QwQ                | 32B        | 20GB  | `ollama pull qwq`                 |
| DeepSeek-R1        | 7B         | 4.7GB | `ollama pull deepseek-r1`         |
| DeepSeek-R1        | 671B       | 404GB | `ollama pull deepseek-r1:671b`    |
| Llama 4            | 109B       | 67GB  | `ollama pull llama4:scout`        |
| Llama 4            | 400B       | 245GB | `ollama pull llama4:maverick`     |
| Llama 3.3          | 70B        | 43GB  | `ollama pull llama3.3`            |
| Llama 3.2          | 3B         | 2.0GB | `ollama pull llama3.2`            |
| Llama 3.2          | 1B         | 1.3GB | `ollama pull llama3.2:1b`         |
| Llama 3.2 Vision   | 11B        | 7.9GB | `ollama pull llama3.2-vision`     |
| Llama 3.2 Vision   | 90B        | 55GB  | `ollama pull llama3.2-vision:90b` |
| Llama 3.1          | 8B         | 4.7GB | `ollama pull llama3.1`            |
| Llama 3.1          | 405B       | 231GB | `ollama pull llama3.1:405b`       |
| Phi 4              | 14B        | 9.1GB | `ollama pull phi4`                |
| Phi 4 Mini         | 3.8B       | 2.5GB | `ollama pull phi4-mini`           |
| Mistral            | 7B         | 4.1GB | `ollama pull mistral`             |
| Moondream 2        | 1.4B       | 829MB | `ollama pull moondream`           |
| Starling           | 7B         | 4.1GB | `ollama pull starling-lm`         |
| Code Llama         | 7B         | 3.8GB | `ollama pull codellama`           |
| Llama 2 Uncensored | 7B         | 3.8GB | `ollama pull llama2-uncensored`   |
| LLaVA              | 7B         | 4.5GB | `ollama pull llava`               |

</small>

---

### <small>Pull Command (1 of 5)</small>

![](images/07-weight.png)

---

### <small>Pull Command (1 of 5)</small>

![](images/08-mnist-2-layer-system.gif)

---

### <small>Pull Command (1 of 5)</small>

![](images/09-mnist-anim.gif)

---
---

## <small>List Command (2 of 5)</small>
<!-- .slide: data-transition="fade" -->

```text
ollama list
NAME                                  ID              SIZE      MODIFIED
qwen3                                 500a1f067a9f    5.2 GB    6 seconds ago
qwen3:30b-a3b                         0b28110b7a33    18 GB     6 weeks ago
qwen3:8b                              500a1f067a9f    5.2 GB    6 weeks ago
qwen3:14b                             bdbd181c33f2    9.3 GB    6 weeks ago
qwen3:30b                             0b28110b7a33    18 GB     6 weeks ago
qwen2.5:7b                            845dbda0ea48    4.7 GB    6 weeks ago
deepseek-r1:1.5b                      e0979632db5a    1.1 GB    7 weeks ago
qwen3:0.6b                            7df6b6e09427    522 MB    7 weeks ago
qwen2.5-coder:0.5b                    4ff64a7f502a    397 MB    7 weeks ago
phi4-reasoning:latest                 47e2630ccbcd    11 GB     7 weeks ago
devstral:24b                          c4b2fa0c33d7    14 GB     7 weeks ago
devstral:latest                       c4b2fa0c33d7    14 GB     7 weeks ago
devstral:24b-small-2505-q4_K_M        c4b2fa0c33d7    14 GB     7 weeks ago
llama3.1:latest                       46e0c10c039e    4.9 GB    3 months ago
llama3.1:8b                           46e0c10c039e    4.9 GB    3 months ago
deepseek-coder-v2:latest              63fb193b3a9b    8.9 GB    3 months ago
gemma3:12b                            f4031aab637d    8.1 GB    3 months ago
gemma3:4b                             a2af6cc3eb7f    3.3 GB    3 months ago
llama2-uncensored:latest              44040b922233    3.8 GB    3 months ago
llama2-uncensored:7b                  44040b922233    3.8 GB    3 months ago
```

---

### <small>List Command (2 of 5)</small>

```sh [1-3|1]
ollama list | grep mini
phi4-mini-reasoning:latest            3ca8c2865ce9    3.2 GB    6 weeks ago
phi4-mini-reasoning:3.8b              3ca8c2865ce9    3.2 GB    6 weeks ago
```

---
---

## <small>Run Command (3 of 5)</small>
<!-- .slide: data-transition="fade" -->

```shell [18|19]
ollama run --help
Run a model

Usage:
  ollama run MODEL [PROMPT] [flags]

Flags:
      --format string      Response format (e.g. json)
  -h, --help               help for run
      --hidethinking       Hide thinking output (if provided)
      --insecure           Use an insecure registry
      --keepalive string   Duration to keep a model loaded (e.g. 5m)
      --nowordwrap         Don't wrap words to the next line automatically
      --think              Whether to use thinking mode for supported models
      --verbose            Show timings for response

Environment Variables:
      OLLAMA_HOST                IP Address for the ollama server (default 127.0.0.1:11434)
      OLLAMA_NOHISTORY           Do not preserve readline history ( ~/.ollama/history )
```

---

### <small>Run Command (3 of 5)</small>

```sh [1|3]
ollama run qwen3 "What is the colour of the sky? Keep it short!"
# OR
ollama run qwen3
# Type /? for help
```

---

### <small>Run Command (3 of 5)</small>

```sh
OLLAMA_HOST=82.154.12.187:11434 ollama run llama3.2-vision
```

---
---

## <small>Process Status Command (4 of 5)</small>

```sh [1-3|1|3]
ollama ps
NAME            ID              SIZE      PROCESSOR    UNTIL
qwen3:latest    500a1f067a9f    7.6 GB    100% GPU     4 minutes from now
```

---
---

## <small>Serve Comma (5 of 5)</small>
<!-- .slide: data-transition="fade" -->

```sh [1-4|4]
ollama serve # AFTER CLOSING OLLAMA
time=2025-07-22T23:42:59.386+01:00 level=INFO source=routes.go:1235 msg="server config"
...
[GIN] 2025/07/22 - 23:43:53 | 200 |  2.713770959s |       127.0.0.1 | POST     "/api/generate"
```

---

## <small>Serve Comma (5 of 5)</small>
<!-- .slide: data-transition="fade" -->

```sh [14-28|16|15|19|22|]
ollama serve --help
Start ollama

Usage:
  ollama serve [flags]

Aliases:
  serve, start

Flags:
  -h, --help   help for serve

Environment Variables:
      OLLAMA_DEBUG               Show additional debug information (e.g. OLLAMA_DEBUG=1)
      OLLAMA_HOST                IP Address for the ollama server (default 127.0.0.1:11434)
      OLLAMA_KEEP_ALIVE          The duration that models stay loaded in memory (default "5m")
      OLLAMA_MAX_LOADED_MODELS   Maximum number of loaded models per GPU
      OLLAMA_MAX_QUEUE           Maximum number of queued requests
      OLLAMA_MODELS              The path to the models directory
      OLLAMA_NUM_PARALLEL        Maximum number of parallel requests
      OLLAMA_NOPRUNE             Do not prune model blobs on startup
      OLLAMA_ORIGINS             A comma separated list of allowed origins
      OLLAMA_SCHED_SPREAD        Always schedule model across all GPUs
      OLLAMA_FLASH_ATTENTION     Enabled flash attention
      OLLAMA_KV_CACHE_TYPE       Quantization type for the K/V cache (default: f16)
      OLLAMA_LLM_LIBRARY         Set LLM library to bypass autodetection
      OLLAMA_GPU_OVERHEAD        Reserve a portion of VRAM per GPU (bytes)
      OLLAMA_LOAD_TIMEOUT        How long to allow model loads to stall before giving up (default "5m")
```

---
---

## <small>Adding UI with ChatBoxAi APP</small>
<!-- .slide: data-transition="fade" data-background="#d5d772" -->

**[https://chatboxai.app](https://chatboxai.app)** <!-- .element: class="fragment r-fit-text" -->

---
---

## <small>&nbsp;</small>
<!-- .slide: data-transition="fade" -->

![](images/00-qr-discord.svg)
