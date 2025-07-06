# LangGraph-multi-modal-researcher
基于LangGraph，结合多模态信息，构建deep_research研究报告


## 概要：
- 您可以传递一个研究主题，也可以选择传递一个YouTube视频URL。
Example:Pass a topic and optionally a video_url.
topic: Give me an overview of the idea that LLMs are like a new kind of operating system.给我一个LLM就像一种新的操作系统的概念的概述。
video_url: https://youtu.be/LCEmiRjPEtQ?si=raeMN2Roy5pESNG2
- 然后系统将使用搜索对该主题进行研究，分析视频，联合见解，并为您生成一份包含引用的报告。

它利用了Gemini的一些本地功能：
1)视频理解和原生YouTube工具：YouTube视频的集成处理
2)Google搜索工具：原生Google搜索工具与实时Web结果集成


## 图结构流程：
搜索研究节点：使用Gemini的Google搜索集成执行Web搜索
分析视频节点：分析YouTube视频（有条件）==如果提供YouTube URL，则工作流有条件地包括视频分析，否则直接进行报告生成。
创建报告节点：将调查结果合成为全面的报告
创建播客节点：生成一个带有TTS音频的双扬声器播客讨论


## 启动：
- 🚀 API: http://127.0.0.1:2024
- 🎨 Studio UI: https://smith.langchain.com/studio/?baseUrl=http://127.0.0.1:2024
- 📚 API Docs: http://127.0.0.1:2024/docs
