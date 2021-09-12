---
title: macOSContentCachingClientPolicy 枚举类型
description: 确定内容缓存将服务于哪些客户端。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8bc8ab9be74dc9686ea534ae98ea170b4ed6760d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017497"
---
# <a name="macoscontentcachingclientpolicy-enum-type"></a>macOSContentCachingClientPolicy 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

确定内容缓存将服务于哪些客户端。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认为本地网络的客户端。|
|clientsInLocalNetwork|1|内容缓存将仅在其直接本地网络中向设备提供内容。|
|clientsWithSamePublicIpAddress|2|内容缓存将为共享同一公共 IP 地址的设备提供内容。|
|clientsInCustomLocalNetworks|3|内容缓存将为 contentCachingClientListenRanges 中的设备提供内容。|
|clientsInCustomLocalNetworksWithFallback|4 |内容缓存将为 contentCachingClientListenRanges、contentCachingPeerListenRanges 和 contentCachingParents 中的设备提供内容。|



