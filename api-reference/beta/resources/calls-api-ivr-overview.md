---
title: 调用中的 IVR 方案
description: 以下是 Microsoft Graph 中的调用 Api 支持的交互语音响应（IVR）方案：
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 62872c07dcf8072a9a5e471c53950a0b77b96814
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507787"
---
# <a name="ivr-scenarios-in-calls"></a>调用中的 IVR 方案

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

以下是 Microsoft Graph 中的调用 Api 支持的交互语音响应（IVR）方案：

- 播放音频提示-例如，当呼叫位于客户服务代理的队列中时。
- 录制响应-例如，录制呼叫者的音频（通常是在听到选项提示后）。
- 订阅声音-例如，当您想要了解呼叫者选择的 DTMF 铃声时，通常会听到音频提示。
- 取消媒体处理-例如，当您想要取消可能正在处理的任何 playPrompt 或 recordResponse 操作时。
