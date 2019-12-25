---
title: 调用中的 IVR 方案
description: 以下是 Microsoft Graph 中的调用 Api 支持的交互语音响应（IVR）方案：
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 4ebb278981ef066aae409d3cc276046a04f79806
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870930"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="40185-103">调用中的 IVR 方案</span><span class="sxs-lookup"><span data-stu-id="40185-103">IVR scenarios in calls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40185-104">以下是 Microsoft Graph 中的调用 Api 支持的交互语音响应（IVR）方案：</span><span class="sxs-lookup"><span data-stu-id="40185-104">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="40185-105">播放音频提示-例如，当呼叫位于客户服务代理的队列中时。</span><span class="sxs-lookup"><span data-stu-id="40185-105">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="40185-106">录制响应-例如，录制呼叫者的音频（通常是在听到选项提示后）。</span><span class="sxs-lookup"><span data-stu-id="40185-106">Recording a response -for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="40185-107">订阅声音-例如，当您想要了解呼叫者选择的 DTMF 铃声时，通常会听到音频提示。</span><span class="sxs-lookup"><span data-stu-id="40185-107">Subscribing to tones - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="40185-108">取消媒体处理-例如，当您想要取消可能正在处理的任何 playPrompt 或 recordResponse 操作时。</span><span class="sxs-lookup"><span data-stu-id="40185-108">Cancel media processing - for example, when you want to cancel any playPrompt or recordResponse operations that might be in process.</span></span>
