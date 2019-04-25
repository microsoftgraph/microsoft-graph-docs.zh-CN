---
title: defenderPromptForSampleSubmission 枚举类型
description: 提示用户提交示例的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c81fe62d7ed2696b233b8684c665f7cf8341fbcd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534778"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>defenderPromptForSampleSubmission 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

提示用户提交示例的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|用户定义, 默认值, 无意向。|
|alwaysPrompt|1|始终提示。|
|promptBeforeSendingPersonalData|2 |发送个人数据前提示。|
|neverSendData|3 |从不发送数据。|
|sendAllDataWithoutPrompting|4 |在不提示的情况下发送所有数据。|





