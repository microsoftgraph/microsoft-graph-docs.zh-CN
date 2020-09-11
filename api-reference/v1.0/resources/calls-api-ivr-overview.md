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
# <a name="ivr-scenarios-in-calls"></a>调用中的 IVR 方案

命名空间：microsoft.graph

以下是 Microsoft Graph 中的调用 Api 支持的交互式语音响应 (IVR) 方案：

- 播放音频提示-例如，当呼叫位于客户服务代理的队列中时。
- 录制响应-例如，录制呼叫者的音频（通常是在听到选项提示后）。
- 订阅声音-例如，当您想要了解呼叫者选择的 DTMF 铃声时，通常会听到音频提示。
- 取消媒体处理-例如，当您想要取消可能正在处理的任何 playPrompt 或 recordResponse 操作时。
