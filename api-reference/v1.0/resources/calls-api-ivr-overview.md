---
title: 呼叫中的 IVR 方案
description: 以下是 Microsoft 中的呼叫 API 支持 (IVR) IVR Graph方案：
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: conceptualPageType
ms.openlocfilehash: d8b08455e417b228fa22faf6083f721d342ee7ed
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59053137"
---
# <a name="ivr-scenarios-in-calls"></a>呼叫中的 IVR 方案

命名空间：microsoft.graph

以下是 Microsoft 中的呼叫 API 支持 (IVR) IVR Graph方案：

- 播放音频提示 - 例如，在客户服务代理队列中进行呼叫时。
- 录制响应 -例如，录制呼叫者的音频，通常是在听到包含选项的提示后录制。
- 订阅音调 - 例如，当你希望了解呼叫者选择的 DTMF 音调时，通常在听到音频提示后。
- 取消媒体处理 - 例如，当您想要取消可能正在处理的任何 playPrompt 或 recordResponse 操作时。
