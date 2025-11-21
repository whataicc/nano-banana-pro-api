# Nano Banana Pro代理API_低价稳定Nano Banana Pro API_国内直连Nano Banana2_Nano Banana Pro API中转站

神马中转 API 现已全面支持 Nano Banana Pro，为开发者在统一接口下调用该模型提供了极高的兼容性与易用性。通过对接 Nano Banana Pro 的推理能力，神马中转 API 能够在保持原有调用格式不变的前提下，为用户带来更快的响应速度、更低的请求延迟和更稳定的服务体验。

同时，依托神马中转 API 的多节点调度、健康探测与自动容灾机制，Nano Banana Pro 的模型能力得以在生产环境中得到更高可靠性保障。开发者无需额外配置复杂的网络或代理，即可直接享受 Nano Banana Pro 的性能优势，让项目快速集成、轻松扩展。

![Nano Banana Pro代理API_低价稳定Nano Banana Pro API_国内直连Nano Banana2_Nano Banana Pro API中转站](https://pic.imgdd.cc/item/691ff344c828c4c6defae888.jpg)    

为了方便国内开发者调用 Nano Banana Pro 模型，可以通过 **神马中转 API** 进行图像生成，接口遵循 OPENAI 标准格式，但做了以下增强：

**/v1/images/generations（通用绘图接口）特性：**

* **支持 DALL·E 格式请求******

* **返回 URL（方便直接下载可见图）******

* **失败不扣费******

* **支持自定义长宽比（ratio / width / height）******

* **兼容 nano-banana-2 等模型名称**

***

### **API 接口调用说明**

> **POST https\://api.whatai.cc/v1/images/generations**

#### **请求体（示例）：**

```
{
  "prompt": "a cute cat wearing sunglasses",
  "model": "nano-banana-2",
  "size": "1024x1024",
  "n": 1
}
```

#### **返回示例（结构示意）：**

```
{
  "data": [
    {
      "url": "https://image-cdn.xxx/xxx.png"
    }
  ]
}
```

***

### **Python 调用示例（可直接使用）**

下面是你提供的 Python 示例，我补充了完整写法，确保即可运行：

```
import http.client
import json

# 神马中转API域名，例如：ahttps://api.whatai.cc
conn = http.client.HTTPSConnection("YOUR_DOMAIN")

payload = json.dumps({
    "prompt": "cat",
    "model": "nano-banana-2",
    "size": "1024x1024"
})

headers = {
    'Authorization': 'Bearer {{YOUR_API_KEY}}',
    'Content-Type': 'application/json'
}

conn.request("POST", "/v1/images/generations", payload, headers)
res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

"{{YOUR\_API\_KEY}}" 替换为你自己的即可。

***

### **可视化操作（无需代码）**

你也可以直接通过网页界面体验 Nano Banana Pro 的图像生成：

**步骤 1：进入首页**

进入你的神马中转平台主页（如 console.xxx.ai）

***

**步骤 2：进入「操练场」**

这是可视化操作区域，可进行 Prompt 输入与模型选择。

***

**步骤 3：选择模型 nano-banana-2**

模型选择下拉框中找到：

```
nano-banana-2
```

***

**步骤 4：输入 Prompt（如：）**

```
一幅具有电影感的广角画面：未来感的沙漠公路上，两辆巨大的悬浮运输载具掠过，空气中弥漫着尘土，夕阳在边缘勾勒出光晕，质感逼真，16:9 画幅
```

***

**步骤 5：点击 “生成 / 提交”**

系统会开始生成图像，等待

***

**步骤 6：查看与下载图片**

生成完成后会显示图像，同时提供：

* **下载1按钮，下载图片（不要刷新页面，等生成完成一定要第一时间下载）**

![【2025最新】Nano Banana 2 Pro代理API：Nano Banana2怎么用，国内直连gemini-3-pro-image-preview API接口服务](https://pic.imgdd.cc/item/691fdb85c828c4c6defabc03.png)    


Gemini 3 Pro Image 模型（内部代号 “Nano Banana Pro/Nano Banana2/gemini-3-pro-image-preview”）是其最新一代的图像生成与编辑系统，面向专业创作与工作流集成。根据官网介绍：

* 大香蕉2模型它支持 “studio-quality control” —— 即可在生成／编辑图像时，对构图、光线、色彩、分辨率、文字等细节进行精细控制。 

* 它支持“real-world knowledge”—— 即可生成知识性、信息性图像（如流程图、信息图、历史场景）并且具备一定的世界认知。 

* 功能模块包括：清晰可读的文字生成、色彩灯光调整、不同截图／镜头角度、不同长宽比、主体一致性、多帧生成以支持故事板、4K或更高分辨率输出。 

* 同时，官网也列出其**限制**：文字容易出错、细节（如人脸、小物件）偶有瑕疵、数据与事实可能不完全准确、翻译本地化、复杂编辑（如融合图片／大幅度光照变化）仍有挑战。 

* 安全机制也涵盖：所有生成／编辑图像嵌入了 SynthID 水印，可用于检测是否为 AI 生成或编辑。 

总的来说，Gemini 3 Pro Image（Nano Banana Pro）定位于高端图像创作与编辑场景，是一个从 “Prompt → 图像” 到 “编辑／定制” 的完整工具。

![Nano Banana2是什么？怎么用？国内如何使用nano banana Pro，gemini-3-pro-image-preview](https://pic.imgdd.cc/item/691fdf97c828c4c6defadc19.jpg)

***

## **Nano Banana2核心功能亮点**

以下是几个该模型尤其值得关注的功能板块：

**清晰文字生成**：可在海报、图示、产品渲染中生成可读文字、手写风格、标识符等。官网展示了例如用 “How much wood would a woodchuck chuck…” 生成木头组成文字的例子。 

* * 提示语里可以明确指定字体、字母构造（如用物体拼字）、背景、长宽比、色彩风格。

  * 注意：虽然比早期模型好很多，但文字还是可能拼错、字母歪斜或识别困难，使用时需检查。

![【2025最新】Nano Banana 2 Pro代理API：Nano Banana2怎么用，国内直连gemini-3-pro-image-preview API接口服务](https://pic.imgdd.cc/item/691fd65ec828c4c6defa8eaf.png)  

**构图与镜头控制**：支持指定视角（如广角、近景、俯拍）、景深效果、主体聚焦或背景虚化。 

* * 例如你可以设定“wide shot of woman walking in forest, sunbeams, 16:9”或者“focus on hand, blur face”。

  * 在工作流中，这意味着你可以把模型当作拍摄导演：先定义镜头，再定义风格。

![【2025最新】Nano Banana 2 Pro代理API：Nano Banana2怎么用，国内直连gemini-3-pro-image-preview API接口服务](https://pic.imgdd.cc/item/691fd6fbc828c4c6defa8fcb.png)  

**色彩与光线调整**：可直接在 Prompt 中要求例如“change to nighttime”“replace volumetric lighting with bokeh”“intense chiaroscuro effect”。 

* * 这让它适合广告、概念艺术、产品展示中需要光影故事感的场景。

  * 注意：光照变化往往比生成新场景更难，模型偶尔可能产生光影断裂、物体阴影不自然等瑕疵。

![【2025最新】Nano Banana 2 Pro代理API：Nano Banana2怎么用，国内直连gemini-3-pro-image-preview API接口服务](https://pic.imgdd.cc/item/691fd731c828c4c6defa9066.png)  

**分辨率／比例／多帧输出**：

* * 支持高分辨率（1K、2K、4K 等）输出。 

  * 支持任意长宽比，从 1:1、4:3、2.39:1、9:16、1:4 等皆可。 

  * 支持“一次多个版本”生成（比如同一 Prompt 多帧输出）用于选稿、制作动画帧、故事板。 

![【2025最新】Nano Banana 2 Pro代理API：Nano Banana2怎么用，国内直连gemini-3-pro-image-preview API接口服务](https://pic.imgdd.cc/item/691fd759c828c4c6defa9098.png)  

**主题一致性 & 编辑能力**：可维持一至多主体（最多五个角色）的一致性、多个对象（最多十四个物体）在同一创作流程中不同场景／服饰变化等。 

* * 例如您可以设定“same six people, different outfits, fashion editorial shot”然后每帧输出一个版本。

  * 编辑方面亦包含：在已有图像基础上做遮罩编辑、改变背景、融合参考图、迁移场景等。

![【2025最新】Nano Banana 2 Pro代理API：Nano Banana2怎么用，国内直连gemini-3-pro-image-preview API接口服务](https://pic.imgdd.cc/item/691fd77fc828c4c6defa90bd.png)  

***

## **Nano Banana Pro使用技巧与建议**

为让你更有效地使用 Gemini 3 Pro Image（Nano Banana Pro），这里整理一些实用技巧：

**✔ 推荐 Prompt 结构**

```
主体 + 场景 + 镜头 + 光照 + 细节 + 风格 + 比例 + 分辨率
```

**✔ 示例**

```
A cinematic wide-angle shot of a futuristic desert highway,
two enormous hovering transports, dusty atmosphere,
sunset rim-lighting, realistic textures, 16:9, 4K resolution
```

**✔ 提高稳定性的技巧**

* 把关键内容放在句首

* 明确“风格词”：realistic / cinematic / neon / 3D render

* 若需要文字：明确写 “clear legible text saying ‘XXXX’ ”

* 若失败/不合适：多用“重生成多个版本”挑选最优

#### **1. 精确构造 Prompt**

* 明确说明 **主体**（主角／物体）、**背景／环境**、**视角**、**灯光／时段**、**风格／色彩**。例如：“A cinematic medium shot of a futuristic city at twilight, two giant starships hovering, long shadows, 16:9, dramatic lighting”.

* 如果需要文字／标识，直接在 Prompt 中说明：“Generate legible bold typography saying ‘Taste the Aura’ on a London street dusk neon lights, 16:9”.

* 指定分辨率或比例：“4K resolution, 16:9”; 或：“square format 1:1 for Instagram”.

* 若想进行编辑以现有图像为基础，则应提供参考图（若平台支持上传）＋说明修改：“Keep the character locked in position, change aspect ratio to 1:1 reducing background only”.

#### **2. 多版本迭代选稿**

* 利用“一次多个版本”能力，生成 4-8 个稍有差别的版本（如角度/构图稍不同）来选最佳。

* 保存好每次 Prompt 的细微差别，方便后续控制与复用。

* 对选定版本再做微调 Prompt／编辑，直到达到满意效果。

#### **3. 注意输出质量限制**

* 虽然模型支持高分辨率，但细节仍可能存在瑕疵（例如文字拼写、手指畸变、小物件透视不自然）——生成后务必人工校对。

* 特别是知识图／信息图、翻译内容、含文字的图表时，需确认数据／翻译准确。官网明确指出“数据和事实准确性仍有限”。 

* 编辑功能（如深度融合、从白天变夜晚）虽强，但复杂场景下仍可能产生视觉瑕疵。建议少量尝试、分步编辑。

***

## Nano Banana2模型官方价格

原生图片生成模型，在速度、灵活性和上下文理解方面经过专门优化。文本输入和输出的定价与 Gemini 3 Pro 相同。 预览版模型在稳定之前可能会发生变化，并且速率限制更严格。 ![【2025最新】Nano Banana 2 Pro代理API：Nano Banana2怎么用，国内直连gemini-3-pro-image-preview API接口服务](https://pic.imgdd.cc/item/691fd854c828c4c6defa9180.png)  

***

## **Nano Banana2 API接口调用与可视化操作**

为了方便国内开发者调用 Nano Banana Pro 模型，可以通过 **神马中转 API** 进行图像生成，接口遵循 OPENAI 标准格式，但做了以下增强：

**/v1/images/generations（通用绘图接口）特性：**

* **支持 DALL·E 格式请求******

* **返回 URL（方便直接下载可见图）******

* **失败不扣费******

* **支持自定义长宽比（ratio / width / height）******

* **兼容 nano-banana-2 等模型名称**

***

### **API 接口调用说明**

> **POST https\://api.whatai.cc/v1/images/generations**

#### **请求体（示例）：**

```
{
  "prompt": "a cute cat wearing sunglasses",
  "model": "nano-banana-2",
  "size": "1024x1024",
  "n": 1
}
```

#### **返回示例（结构示意）：**

```
{
  "data": [
    {
      "url": "https://image-cdn.xxx/xxx.png"
    }
  ]
}
```

***

### **Python 调用示例（可直接使用）**

下面是你提供的 Python 示例，我补充了完整写法，确保即可运行：

```
import http.client
import json

# 神马中转API域名，例如：ahttps://api.whatai.cc
conn = http.client.HTTPSConnection("YOUR_DOMAIN")

payload = json.dumps({
    "prompt": "cat",
    "model": "nano-banana-2",
    "size": "1024x1024"
})

headers = {
    'Authorization': 'Bearer {{YOUR_API_KEY}}',
    'Content-Type': 'application/json'
}

conn.request("POST", "/v1/images/generations", payload, headers)
res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

"{{YOUR\_API\_KEY}}" 替换为你自己的即可。

***

### **可视化操作（无需代码）**

你也可以直接通过网页界面体验 Nano Banana Pro 的图像生成：

**步骤 1：进入首页**

进入你的神马中转平台主页（如 console.xxx.ai）

***

**步骤 2：进入「操练场」**

这是可视化操作区域，可进行 Prompt 输入与模型选择。

***

**步骤 3：选择模型 nano-banana-2**

模型选择下拉框中找到：

```
nano-banana-2
```

***

**步骤 4：输入 Prompt（如：）**

```
一幅具有电影感的广角画面：未来感的沙漠公路上，两辆巨大的悬浮运输载具掠过，空气中弥漫着尘土，夕阳在边缘勾勒出光晕，质感逼真，16:9 画幅
```

***

**步骤 5：点击 “生成 / 提交”**

系统会开始生成图像，等待

***

**步骤 6：查看与下载图片**

生成完成后会显示图像，同时提供：

* **下载1按钮，下载图片（不要刷新页面，等生成完成一定要第一时间下载）**

![【2025最新】Nano Banana 2 Pro代理API：Nano Banana2怎么用，国内直连gemini-3-pro-image-preview API接口服务](https://pic.imgdd.cc/item/691fdb85c828c4c6defabc03.png)    

Gemini 3 Pro Image（Nano Banana Pro）是一个面向高端创作、编辑与生产工作流程的图像生成系统。它在文字清晰度、镜头与灯光控制、分辨率与比例调整、多版本迭代、主体一致性等方面具备显著优势。若合理构造 Prompt、注意其限制、结合人工校对流程，即可大幅提升创作效率与输出品质。

