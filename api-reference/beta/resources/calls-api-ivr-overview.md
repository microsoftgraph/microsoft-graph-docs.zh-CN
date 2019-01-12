---
title: 呼叫中的 IVR 方案
description: 在 Microsoft Graph 中的调用 Api 支持互动语音响应 (IVR) 方案如下：
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a3657d60344941de931e4f77bddde922d7d01f21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936359"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="9b4eb-103">呼叫中的 IVR 方案</span><span class="sxs-lookup"><span data-stu-id="9b4eb-103">IVR scenarios in calls</span></span>

> <span data-ttu-id="9b4eb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9b4eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b4eb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9b4eb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b4eb-106">在 Microsoft Graph 中的调用 Api 支持互动语音响应 (IVR) 方案如下：</span><span class="sxs-lookup"><span data-stu-id="9b4eb-106">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="9b4eb-107">客户服务代理队列中发出呼叫时播放音频提示-例如。</span><span class="sxs-lookup"><span data-stu-id="9b4eb-107">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="9b4eb-108">记录-例如，通常后它们听到选项提示记录呼叫者的音频。</span><span class="sxs-lookup"><span data-stu-id="9b4eb-108">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="9b4eb-109">订阅音-例如，当您想知道哪些 DTMF 铃声选择，通常后听到音频提示呼叫者。</span><span class="sxs-lookup"><span data-stu-id="9b4eb-109">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="9b4eb-110">例如，取消媒体处理-，您想要取消任何 PlayPrompt 或记录操作过程中可能存在时。</span><span class="sxs-lookup"><span data-stu-id="9b4eb-110">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
