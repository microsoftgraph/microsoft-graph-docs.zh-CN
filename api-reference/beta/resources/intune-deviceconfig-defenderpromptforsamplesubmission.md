---
title: defenderPromptForSampleSubmission 枚举类型
description: 提示用户输入示例提交的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b706c0086791543a5cbb13d26ae1d86a2e3b1760
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403313"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>defenderPromptForSampleSubmission 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

提示用户输入示例提交的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|用户定制|0|用户定义，默认值、 没有用途。|
|alwaysPrompt|1|始终提示。|
|promptBeforeSendingPersonalData|2|将个人数据发送前提示。|
|neverSendData|3|从不发送数据。|
|sendAllDataWithoutPrompting|4|发送所有数据，而不提示。|




