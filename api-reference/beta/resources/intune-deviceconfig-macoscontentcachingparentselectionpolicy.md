---
title: macOSContentCachingParentSelectionPolicy 枚举类型
description: 确定内容缓存如何选择父缓存。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 45cc23160ba937481eb6b1af8f404c0a2fd4f3cb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026633"
---
# <a name="macoscontentcachingparentselectionpolicy-enum-type"></a>macOSContentCachingParentSelectionPolicy 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

确定内容缓存如何选择父缓存。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认值为循环策略。|
|roundRobin|1 |按顺序旋转父项。 使用此策略进行负载平衡。|
|firstAvailable|2 |始终使用父列表中的第一个可用父项。 使用此策略可指定永久的主要、次要和后续父项。|
|urlPathHash|第三章|对所请求 URL 的路径部分进行哈希运算，以便始终将相同的父项用于相同的 URL。 这有助于最大限度地提高父项的合并缓存的大小。|
|随机|4 |随机选择父项。 使用此策略进行负载平衡。|
|stickyAvailable|5 |使用父列表中的第一个可用父项，直到其不可用，然后前进到下一个。 使用此策略可指定浮动的主要、辅助和后续的父项。|






