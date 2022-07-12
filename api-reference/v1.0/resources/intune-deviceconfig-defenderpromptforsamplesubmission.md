---
title: defenderPromptForSampleSubmission 枚举类型
description: 提示用户提交示例的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5445d9e279c1bbc98e58767d79638b0b8872ae25
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734345"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>defenderPromptForSampleSubmission 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

提示用户提交示例的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|用户定义，默认值，无意向。|
|alwaysPrompt|1|始终提示。|
|promptBeforeSendingPersonalData|2|自动发送安全示例。|
|neverSendData|3|切勿发送数据。|
|sendAllDataWithoutPrompting|4|在不提示的情况下发送所有数据。|





