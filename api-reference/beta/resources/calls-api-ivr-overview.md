---
title: 调用中的 IVR 方案
description: '以下是 Microsoft Graph 中的调用 api 支持的交互语音响应 (IVR) 方案:'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aed30bc5ad109dc3f21d381f4d6b04e087a779a3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535552"
---
# <a name="ivr-scenarios-in-calls"></a><span data-ttu-id="91d1e-103">调用中的 IVR 方案</span><span class="sxs-lookup"><span data-stu-id="91d1e-103">IVR scenarios in calls</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91d1e-104">以下是 Microsoft Graph 中的调用 api 支持的交互语音响应 (IVR) 方案:</span><span class="sxs-lookup"><span data-stu-id="91d1e-104">The following are the Interactive Voice Response (IVR) scenarios that the calling APIs in Microsoft Graph support:</span></span>

- <span data-ttu-id="91d1e-105">播放音频提示-例如, 当呼叫位于客户服务代理的队列中时。</span><span class="sxs-lookup"><span data-stu-id="91d1e-105">Playing an audio prompt - for example, when a call is placed in a customer service agent's queue.</span></span>
- <span data-ttu-id="91d1e-106">记录-例如, 录制呼叫者的音频 (通常是在听到选项提示后)。</span><span class="sxs-lookup"><span data-stu-id="91d1e-106">Record - for example, to record the caller's audio, usually after they heard a prompt with options.</span></span>
- <span data-ttu-id="91d1e-107">订阅语气-例如, 当您想要了解呼叫者选择的 DTMF 铃声时, 通常会听到音频提示。</span><span class="sxs-lookup"><span data-stu-id="91d1e-107">Subscribe to tone - for example, when you want to know what DTMF tones the caller selected, usually after hearing the audio prompt.</span></span>
- <span data-ttu-id="91d1e-108">取消媒体处理-例如, 当您想要取消任何可能正在处理的 PlayPrompt 或记录操作时。</span><span class="sxs-lookup"><span data-stu-id="91d1e-108">Cancel Media Processing - for example, when you want to cancel any PlayPrompt or Record operations that might be in process.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/calls-api-ivr-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
