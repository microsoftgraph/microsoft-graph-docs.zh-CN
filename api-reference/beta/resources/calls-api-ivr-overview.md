---
title: 调用中的 IVR 方案
description: '以下是 Microsoft Graph 中的调用 Api 支持的交互语音响应 (IVR) 方案:'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: conceptualPageType
ms.openlocfilehash: 25f9339f33a6a679a8c8829214526fc29bc88b04
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013036"
---
# <a name="ivr-scenarios-in-calls"></a>调用中的 IVR 方案

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

以下是 Microsoft Graph 中的调用 Api 支持的交互语音响应 (IVR) 方案:

- 播放音频提示-例如, 当呼叫位于客户服务代理的队列中时。
- 记录-例如, 录制呼叫者的音频 (通常是在听到选项提示后)。
- 订阅语气-例如, 当您想要了解呼叫者选择的 DTMF 铃声时, 通常会听到音频提示。
- 取消媒体处理-例如, 当您想要取消任何可能正在处理的 PlayPrompt 或记录操作时。
