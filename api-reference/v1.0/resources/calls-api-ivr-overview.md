---
title: 呼叫中的 IVR 方案
description: 以下是 Microsoft 中的呼叫 API (支持的交互式语音) IVR Graph方案：
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: cbf46e81d537c704e6225a6d756140dd3ce8221fc70a7e86f188cead4ec9d3e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54238186"
---
# <a name="ivr-scenarios-in-calls"></a>呼叫中的 IVR 方案

命名空间：microsoft.graph

以下是 Microsoft 中的呼叫 API (支持的交互式语音) IVR Graph方案：

- 播放音频提示 - 例如，在客户服务代理的队列中进行呼叫时。
- 录制响应 -例如，录制呼叫者的音频，通常是在听到包含选项的提示后录制。
- 订阅音调 - 例如，当你想要了解呼叫者选择的 DTMF 音时（通常在听到音频提示后）。
- 取消媒体处理 - 例如，当您想要取消可能正在处理的任何 playPrompt 或 recordResponse 操作时。
