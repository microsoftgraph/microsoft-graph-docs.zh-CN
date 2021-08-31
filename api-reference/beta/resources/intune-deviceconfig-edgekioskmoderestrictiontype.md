---
title: edgeKioskModeRestrictionType 枚举类型
description: 指定如何Microsoft Edge展台模式限制用户设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b08d5190992433f0f3457c29fb74ccfa8c57e998
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796626"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a>edgeKioskModeRestrictionType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定如何Microsoft Edge展台模式限制用户设置。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未 (无限制) 。|
|digitalSignage|1|单应用模式下的交互式/数字标志。|
|normalMode|2|正常模式 (完整版本的Microsoft Edge) 。|
|publicBrowsingSingleApp|3|单应用模式下的公共浏览。|
|publicBrowsingMultiApp|4 |在多 (模式下) 公共浏览模式。|



