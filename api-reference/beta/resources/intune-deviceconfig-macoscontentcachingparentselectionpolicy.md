---
title: macOSContentCachingParentSelectionPolicy 枚举类型
description: 确定内容缓存如何选择父缓存。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 26ee398da892231e79d85b2377bae103b36e671c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783552"
---
# <a name="macoscontentcachingparentselectionpolicy-enum-type"></a>macOSContentCachingParentSelectionPolicy 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

确定内容缓存如何选择父缓存。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认为循环策略。|
|roundRobin|1|按序在父对象中旋转。 使用此策略实现负载平衡。|
|firstAvailable|2|始终使用"父项"列表中的第一个可用父级。 使用此策略可指定永久主要、辅助和后续父项。|
|urlPathHash|3|对请求的 URL 的路径部分进行哈希处理，以便始终将同一个父级用于同一 URL。 这对最大程度地增加父项的组合缓存的大小非常有用。|
|random|4 |随机选择父级。 使用此策略实现负载平衡。|
|stickyAvailable|5 |使用"父项"列表中可用的第一个可用父级，直到其不可用，然后前进到下一个。 使用此策略指定浮动主要、辅助和后续父项。|



