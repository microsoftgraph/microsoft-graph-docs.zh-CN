---
title: macOSContentCachingClientPolicy 枚举类型
description: 确定内容缓存将服务的客户端。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b8b2baeb66173b8e09f46bd570aa799ca9d2845e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268781"
---
# <a name="macoscontentcachingclientpolicy-enum-type"></a>macOSContentCachingClientPolicy 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

确定内容缓存将服务的客户端。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认值为本地网络中的客户端。|
|clientsInLocalNetwork|1|内容缓存将仅在其直接本地网络中向设备提供内容。|
|clientsWithSamePublicIpAddress|双面|内容缓存将向共享相同公用 IP 地址的设备提供内容。|
|clientsInCustomLocalNetworks|第三章|内容缓存将向 contentCachingClientListenRanges 中的设备提供内容。|
|clientsInCustomLocalNetworksWithFallback|4 |内容缓存将向 contentCachingClientListenRanges、contentCachingPeerListenRanges 和 contentCachingParents 中的设备提供内容。|




