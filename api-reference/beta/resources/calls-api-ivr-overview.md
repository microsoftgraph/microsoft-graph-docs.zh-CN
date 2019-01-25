---
title: 呼叫中的 IVR 方案
description: 在 Microsoft Graph 中的调用 Api 支持互动语音响应 (IVR) 方案如下：
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aed30bc5ad109dc3f21d381f4d6b04e087a779a3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519379"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="35b69-103">呼叫中的 IVR 方案</span><span class="sxs-lookup"><span data-stu-id="35b69-103">IVR scenarios in calls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35b69-104">在 Microsoft Graph 中的调用 Api 支持互动语音响应 (IVR) 方案如下：</span><span class="sxs-lookup"><span data-stu-id="35b69-104">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="35b69-105">客户服务代理队列中发出呼叫时播放音频提示-例如。</span><span class="sxs-lookup"><span data-stu-id="35b69-105">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="35b69-106">记录-例如，通常后它们听到选项提示记录呼叫者的音频。</span><span class="sxs-lookup"><span data-stu-id="35b69-106">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="35b69-107">订阅音-例如，当您想知道哪些 DTMF 铃声选择，通常后听到音频提示呼叫者。</span><span class="sxs-lookup"><span data-stu-id="35b69-107">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="35b69-108">例如，取消媒体处理-，您想要取消任何 PlayPrompt 或记录操作过程中可能存在时。</span><span class="sxs-lookup"><span data-stu-id="35b69-108">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/calls-api-ivr-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
