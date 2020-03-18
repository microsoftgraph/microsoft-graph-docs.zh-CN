---
title: vppTokenActionFailureReason 枚举类型
description: Apple Volume Purchase Program 令牌操作失败的可能原因类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8765d0dd62579f470133e81005ff995638e00a5d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767097"
---
# <a name="vpptokenactionfailurereason-enum-type"></a>vppTokenActionFailureReason 枚举类型

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



