---
title: 调用中的 IVR 方案
description: 以下是 Microsoft Graph 中的调用 Api 支持的交互式语音响应 (IVR) 方案：
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 2b9d4b26d121c7abef1b677db7490a8ec03386c9
ms.sourcegitcommit: c7c198f6fa252b68e91be341b93b818afd387486
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2020
ms.locfileid: "47439946"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="0f0c9-103">调用中的 IVR 方案</span><span class="sxs-lookup"><span data-stu-id="0f0c9-103">IVR scenarios in calls</span></span>

<span data-ttu-id="0f0c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f0c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f0c9-105">以下是 Microsoft Graph 中的调用 Api 支持的交互式语音响应 (IVR) 方案：</span><span class="sxs-lookup"><span data-stu-id="0f0c9-105">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="0f0c9-106">播放音频提示-例如，当呼叫位于客户服务代理的队列中时。</span><span class="sxs-lookup"><span data-stu-id="0f0c9-106">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="0f0c9-107">录制响应-例如，录制呼叫者的音频（通常是在听到选项提示后）。</span><span class="sxs-lookup"><span data-stu-id="0f0c9-107">Recording a response -for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="0f0c9-108">订阅声音-例如，当您想要了解呼叫者选择的 DTMF 铃声时，通常会听到音频提示。</span><span class="sxs-lookup"><span data-stu-id="0f0c9-108">Subscribing to tones - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="0f0c9-109">取消媒体处理-例如，当您想要取消可能正在处理的任何 playPrompt 或 recordResponse 操作时。</span><span class="sxs-lookup"><span data-stu-id="0f0c9-109">Cancel media processing - for example, when you want to cancel any playPrompt or recordResponse operations that might be in process.</span></span>
