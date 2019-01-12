---
title: deviceEnrollmentFailureReason 枚举类型
description: 注册的顶部级别故障类别。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 25834f9c6e972a5a12d3e8d1e2a1283646483000
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981033"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>deviceEnrollmentFailureReason 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

注册的顶部级别故障类别。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认值是未知失败原因。|
|身份验证|1|失败的身份验证|
|授权|2|呼叫已通过身份验证，但未被授权注册。|
|accountValidation|3|无法验证注册的帐户。 （帐户已被阻止，注册未启用）|
|userValidation|4|无法验证用户。 (不存在用户，缺少许可证)|
|deviceNotSupported|5|不支持移动设备管理设备。|
|inMaintenance|6|帐户是在维护。|
|badRequest|7|客户端发送请求不是服务理解/支持。|
|featureNotSupported|8|此帐户不支持使用此注册的功能。|
|enrollmentRestrictionsEnforced|9|注册限制配置被管理员阻止此注册。|
|clientDisconnected|10|客户端超时或注册已中止由最终用户。|
|userAbandonment|11|注册已放弃的最终用户。 （最终用户启动入职培训，但无法完成及时）|





