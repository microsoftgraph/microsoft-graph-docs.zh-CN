---
title: deviceEnrollmentFailureReason 枚举类型
description: 用于注册的顶级失败类别。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7f47c4903c17d8c99408449d32b83a38a7389204
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266630"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>deviceEnrollmentFailureReason 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于注册的顶级失败类别。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认值，失败原因未知。|
|身份验证|1 |身份验证失败|
|authorization|2 |呼叫已通过身份验证，但无权注册。|
|accountValidation|3 |未能验证帐户注册。  (帐户被阻止，注册未) |
|userValidation|4 |无法验证用户。  (用户不存在，缺少许可证) |
|deviceNotSupported|5 |移动设备管理不支持设备。|
|inMaintenance|6 |帐户在维护中。|
|badRequest|7 |客户端发送了服务无法理解/不支持的请求。|
|featureNotSupported|8 |此 () 不支持此注册使用的功能。|
|enrollmentRestrictionsEnforced|9 |管理员配置的注册限制阻止了此注册。|
|clientDisconnected|10 |客户端已暂停或注册已由最终用户中止。|
|userAbandonment|11 |最终用户已放弃注册。  (Enduser 开始载入，但未能及时完成) |




