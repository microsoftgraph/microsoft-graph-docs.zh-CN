---
title: 呼叫中的 IVR 方案
description: 在 Microsoft Graph 中的调用 Api 支持互动语音响应 (IVR) 方案如下：
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 014fd2169678617043a5a540f625479e68302b34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855809"
---
# <a name="ivr-scenarios-in-calls"></a>呼叫中的 IVR 方案

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在 Microsoft Graph 中的调用 Api 支持互动语音响应 (IVR) 方案如下：

- 客户服务代理队列中发出呼叫时播放音频提示-例如。
- 记录-例如，通常后它们听到选项提示记录呼叫者的音频。
- 订阅音-例如，当您想知道哪些 DTMF 铃声选择，通常后听到音频提示呼叫者。
- 例如，取消媒体处理-，您想要取消任何 PlayPrompt 或记录操作过程中可能存在时。
