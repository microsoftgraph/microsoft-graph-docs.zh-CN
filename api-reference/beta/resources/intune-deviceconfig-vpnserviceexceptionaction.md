---
title: vpnServiceExceptionAction 枚举类型
description: 对特定服务要采取 VPN 操作。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a43e97e993a9a605aee3561c188bf3a969f0510d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59027076"
---
# <a name="vpnserviceexceptionaction-enum-type"></a>vpnServiceExceptionAction 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

对特定服务要采取 VPN 操作。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|forceTrafficViaVPN|0|使该服务的所有流量都通过 VPN|
|allowTrafficOutside|1|允许 VPN 外部的服务|
|dropTraffic|2|从服务删除所有流量|



