---
title: deviceEnrollmentFailureReason 枚举类型
description: 注册的顶级失败类别。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fefe8adf226f99a239bd9a04331596861237c0ad
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445551"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a>deviceEnrollmentFailureReason 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

注册的顶级失败类别。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|默认值，失败原因未知。|
|authentication|1|身份验证失败|
|批准|双面|呼叫已通过身份验证，但未获授权进行注册。|
|accountValidation|第三章|无法验证注册帐户。 （帐户被阻止，未启用注册）|
|userValidation|4 |无法验证用户。 （用户不存在，缺少许可证）|
|deviceNotSupported|5 |移动设备管理不支持设备。|
|inMaintenance|6 |帐户处于维护中。|
|badRequest|7 |客户端发送了服务无法理解/支持的请求。|
|featureNotSupported|8 |此帐户不支持此注册使用的功能。|
|enrollmentRestrictionsEnforced|9 |由管理员配置的注册限制阻止了此注册。|
|clientDisconnected|10 |客户端超时或注册被 enduser 中止。|
|userAbandonment|11x17|注册已被 enduser 放弃。 （Enduser 已开始加入，但无法及时完成它）|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->





