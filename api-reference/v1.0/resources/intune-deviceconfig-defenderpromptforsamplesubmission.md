---
title: defenderPromptForSampleSubmission 枚举类型
description: 提示用户输入示例提交的可能值。
author: tfitzmac
ms.openlocfilehash: 36a9790b669c588205824be60d350d2750637b15
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312745"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a>defenderPromptForSampleSubmission 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

提示用户输入示例提交的可能值。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|用户定制|0|用户定义，默认值、 没有用途。|
|alwaysPrompt|1|始终提示。|
|promptBeforeSendingPersonalData|2|将个人数据发送前提示。|
|neverSendData|3|从不发送数据。|
|sendAllDataWithoutPrompting|4|发送所有数据，而不提示。|



