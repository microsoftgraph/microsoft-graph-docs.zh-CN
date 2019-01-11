---
title: defenderPromptForSampleSubmission 枚举类型
description: 提示用户输入示例提交的可能值。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f1dbd79d58fa46a4e5e50f989e807763ff10356
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849824"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>defenderPromptForSampleSubmission 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

提示用户输入示例提交的可能值。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|用户定制|0|用户定义，默认值、 没有用途。|
|alwaysPrompt|1|始终提示。|
|promptBeforeSendingPersonalData|2|将个人数据发送前提示。|
|neverSendData|3|从不发送数据。|
|sendAllDataWithoutPrompting|4|发送所有数据，而不提示。|





