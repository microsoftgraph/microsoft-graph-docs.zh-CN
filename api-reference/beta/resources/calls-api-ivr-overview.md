---
title: 调用中的 IVR 方案
description: 以下是 Microsoft Graph 中的调用 Api 支持的交互语音响应（IVR）方案：
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 094b0677e243696a1dfe81a3916a863c09e73b92
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006731"
---
# <a name="ivr-scenarios-in-calls"></a>调用中的 IVR 方案

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

以下是 Microsoft Graph 中的调用 Api 支持的交互语音响应（IVR）方案：

- 播放音频提示-例如，当呼叫位于客户服务代理的队列中时。
- 记录-例如，录制呼叫者的音频（通常是在听到选项提示后）。
- 订阅语气-例如，当您想要了解呼叫者选择的 DTMF 铃声时，通常会听到音频提示。
- 取消媒体处理-例如，当您想要取消任何可能正在处理的 PlayPrompt 或记录操作时。
