---
title: vppTokenActionFailureReason 枚举类型
description: Apple Volume Purchase Program 令牌操作失败的可能原因类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 883772d99077e8587ba5467ec8c9492eddfb62e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070672"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>vppTokenActionFailureReason 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Apple Volume Purchase Program 令牌操作失败的可能原因类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|无。|
|appleFailure|1 |Apple 的服务上出现错误。|
|internalError|2 |有一个内部错误。|
|expiredVppToken|第三章|由于 Apple Volume Purchase Program 令牌已过期，因此出现错误。|
|expiredApplePushNotificationCertificate|4 |由于 Apple Volume Purchase Program 推送通知证书已过期，因此出现错误。|






