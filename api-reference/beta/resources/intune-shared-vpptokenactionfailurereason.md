---
title: vppTokenActionFailureReason 枚举类型
description: 可能的 Apple 卷购买计划令牌操作失败的原因的类型。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f488302b7fc701e8a419357ad7d6cbbb6015759b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883718"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>vppTokenActionFailureReason 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

可能的 Apple 卷购买计划令牌操作失败的原因的类型。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|无|0|无。|
|appleFailure|1|在 Apple 的服务时出错。|
|internalError|2|存在内部错误。|
|expiredVppToken|3|因为 Apple 卷购买计划令牌已过期时出错。|
|expiredApplePushNotificationCertificate|4|由于 Apple 卷购买程序推送通知证书过期时出错。|





