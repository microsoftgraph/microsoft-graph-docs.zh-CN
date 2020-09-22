---
title: macOSContentCachingPeerPolicy 枚举类型
description: 确定哪些内容缓存其他内容缓存将对等。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e45f6d0e92624693139cd09ca4eff52cd483b46c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993824"
---
# <a name="macoscontentcachingpeerpolicy-enum-type"></a>macOSContentCachingPeerPolicy 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

确定哪些内容缓存其他内容缓存将对等。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认值为本地网络中的对等方。|
|peersInLocalNetwork|1 |内容缓存将仅对其直接本地网络中的缓存具有同等的对等缓存。|
|peersWithSamePublicIpAddress|2 |内容缓存将仅对共享相同公用 IP 地址的缓存具有同等的对等缓存。|
|peersInCustomLocalNetworks|第三章|内容缓存将使用 contentCachingPeerFilterRanges 和 contentCachingPeerListenRanges 来确定与对等方的缓存。|






