---
title: emailSyncDuration 枚举类型
description: 电子邮件同步持续时间的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8bf62aea1904c0fd25867aef308ca5a269e3ea20
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399407"
---
# <a name="emailsyncduration-enum-type"></a>emailSyncDuration 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

电子邮件同步持续时间的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|用户定制|0|用户定义，默认值、 没有用途。|
|工期|1|同步电子邮件中的一天。|
|3 个工作日|2|同步三天的电子邮件。|
|1 周时间|3|同步电子邮件的一周。|
|twoWeeks|4|同步电子邮件的两个星期。|
|oneMonth|5|同步电子邮件的一个月。|
|无限制|6|同步电子邮件不受限制的持续的时间。|




