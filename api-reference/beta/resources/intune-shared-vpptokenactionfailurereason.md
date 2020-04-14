---
title: vppTokenActionFailureReason 枚举类型
description: Apple Volume Purchase Program 令牌操作失败的可能原因类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3b7d236aa9b3cc0b6e20a90b646ba3a95eaf0d3f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463321"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>vppTokenActionFailureReason 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Apple Volume Purchase Program 令牌操作失败的可能原因类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|无。|
|appleFailure|1|Apple 的服务上出现错误。|
|internalError|双面|有一个内部错误。|
|expiredVppToken|第三章|由于 Apple Volume Purchase Program 令牌已过期，因此出现错误。|
|expiredApplePushNotificationCertificate|4 |由于 Apple Volume Purchase Program 推送通知证书已过期，因此出现错误。|



