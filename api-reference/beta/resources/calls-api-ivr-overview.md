---
title: 调用中的 IVR 方案
description: '以下是 Microsoft Graph 中的调用 api 支持的交互语音响应 (IVR) 方案:'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 69023de179714797156f8ed039e2086e060fe9b1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338768"
---
# <a name="ivr-scenarios-in-calls"></a>调用中的 IVR 方案

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

以下是 Microsoft Graph 中的调用 api 支持的交互语音响应 (IVR) 方案:

- 播放音频提示-例如, 当呼叫位于客户服务代理的队列中时。
- 记录-例如, 录制呼叫者的音频 (通常是在听到选项提示后)。
- 订阅语气-例如, 当您想要了解呼叫者选择的 DTMF 铃声时, 通常会听到音频提示。
- 取消媒体处理-例如, 当您想要取消任何可能正在处理的 PlayPrompt 或记录操作时。
