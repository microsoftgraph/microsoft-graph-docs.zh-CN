---
title: macOSContentCachingPeerPolicy 枚举类型
description: 确定其他内容缓存将对等哪些内容缓存。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 22adc6cd2df6dad85875deb190f40c305776a991
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783545"
---
# <a name="macoscontentcachingpeerpolicy-enum-type"></a>macOSContentCachingPeerPolicy 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

确定其他内容缓存将对等哪些内容缓存。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认为本地网络的对等方。|
|peersInLocalNetwork|1|内容缓存仅与直接本地网络中缓存对等。|
|peersWithSamePublicIpAddress|2|内容缓存仅与共享同一公共 IP 地址的缓存对等。|
|peersInCustomLocalNetworks|3|内容缓存将使用 contentCachingPeerFilterRanges 和 contentCachingPeerListenRanges 来确定要对等的缓存。|



