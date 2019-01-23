---
title: deviceEnrollmentFailureReason 枚举类型
description: 注册的顶部级别故障类别。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fbfe7193c72f1ff1a03a7e7bb4da57d0a032e530
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396208"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>deviceEnrollmentFailureReason 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




