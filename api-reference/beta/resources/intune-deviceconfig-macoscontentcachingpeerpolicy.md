---
title: macOSContentCachingPeerPolicy 枚举类型
description: 确定其他内容缓存将对等哪些内容缓存。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b89b7043ca64f106ec1d3bbded041ae15461195c916db0d31cf32dd848d42e40
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54181193"
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
|peersInLocalNetwork|1 |内容缓存仅与直接本地网络中缓存对等。|
|peersWithSamePublicIpAddress|2 |内容缓存仅与共享同一公共 IP 地址的缓存对等。|
|peersInCustomLocalNetworks|3 |内容缓存将使用 contentCachingPeerFilterRanges 和 contentCachingPeerListenRanges 来确定要对等的缓存。|




