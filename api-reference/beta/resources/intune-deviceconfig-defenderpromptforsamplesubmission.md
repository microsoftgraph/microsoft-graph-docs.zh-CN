---
title: defenderPromptForSampleSubmission 枚举类型
description: 提示用户提交示例的可能值。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 86b8bdb6096aa9ea86f3ce202b107c27610a1ff3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091760"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>defenderPromptForSampleSubmission 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

提示用户提交示例的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|用户定义，默认值，无意图。|
|alwaysPrompt|1|始终提示。|
|promptBeforeSendingPersonalData|2|自动发送安全示例。|
|neverSendData|3|从不发送数据。|
|sendAllDataWithoutPrompting|4 |在不提示的情况下发送所有数据。|



