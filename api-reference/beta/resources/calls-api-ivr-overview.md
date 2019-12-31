---
title: 调用中的 IVR 方案
description: 以下是 Microsoft Graph 中的调用 Api 支持的交互语音响应（IVR）方案：
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: 561f0097eae74ca3f5d36fc18ec62aef8bcca3d6
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913504"
---
# <a name="ivr-scenarios-in-calls"></a>调用中的 IVR 方案

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

以下是 Microsoft Graph 中的调用 Api 支持的交互语音响应（IVR）方案：

- 播放音频提示-例如，当呼叫位于客户服务代理的队列中时。
- 录制响应-例如，录制呼叫者的音频（通常是在听到选项提示后）。
- 订阅声音-例如，当您想要了解呼叫者选择的 DTMF 铃声时，通常会听到音频提示。
- 取消媒体处理-例如，当您想要取消可能正在处理的任何 playPrompt 或 recordResponse 操作时。
