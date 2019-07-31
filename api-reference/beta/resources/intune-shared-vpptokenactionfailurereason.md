---
title: vppTokenActionFailureReason 枚举类型
description: Apple Volume Purchase Program 令牌操作失败的可能原因类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 697dd182aa21d98418cfee056da8cc18b1aa0aee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967305"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>vppTokenActionFailureReason 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Apple Volume Purchase Program 令牌操作失败的可能原因类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|无。|
|appleFailure|1|Apple 的服务上出现错误。|
|internalError|双面|有一个内部错误。|
|expiredVppToken|第三章|由于 Apple Volume Purchase Program 令牌已过期, 因此出现错误。|
|expiredApplePushNotificationCertificate|4|由于 Apple Volume Purchase Program 推送通知证书已过期, 因此出现错误。|





