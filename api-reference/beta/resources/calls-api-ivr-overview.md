---
title: 呼叫中的 IVR 方案
description: 在 Microsoft Graph 中的调用 Api 支持互动语音响应 (IVR) 方案如下：
author: VinodRavichandran
ms.openlocfilehash: cf7d6543c09b69050db9aedc270616cfea113c28
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380462"
---
# <a name="ivr-scenarios-in-calls"></a>呼叫中的 IVR 方案

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在 Microsoft Graph 中的调用 Api 支持互动语音响应 (IVR) 方案如下：

- 客户服务代理队列中发出呼叫时播放音频提示-例如。
- 记录-例如，通常后它们听到选项提示记录呼叫者的音频。
- 订阅音-例如，当您想知道哪些 DTMF 铃声选择，通常后听到音频提示呼叫者。
- 例如，取消媒体处理-，您想要取消任何 PlayPrompt 或记录操作过程中可能存在时。
