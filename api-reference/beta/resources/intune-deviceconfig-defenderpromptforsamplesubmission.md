---
title: defenderPromptForSampleSubmission 枚举类型
description: 提示用户提交示例的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d5cf699b386dbf0c6d75a19522529386ab36977d
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177700"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>defenderPromptForSampleSubmission 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

提示用户提交示例的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|用户定义，默认值，无意向。|
|alwaysPrompt|1|始终提示。|
|promptBeforeSendingPersonalData|双面|自动发送安全示例。|
|neverSendData|第三章|从不发送数据。|
|sendAllDataWithoutPrompting|4 |在不提示的情况下发送所有数据。|



