---
title: edgeKioskModeRestrictionType 枚举类型
description: 根据展台模式指定 Microsoft Edge 设置的限制方式。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0dcd1d30895acbdecf9d9cc706ee14b7907f14f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177957"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a>edgeKioskModeRestrictionType 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

根据展台模式指定 Microsoft Edge 设置的限制方式。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置 (无限制)。|
|digitalSignage|1|单应用模式中的交互/数字告示。|
|normalMode|双面|正常模式 (Microsoft Edge 的完整版本)。|
|publicBrowsingSingleApp|第三章|单应用模式中的公共浏览。|
|publicBrowsingMultiApp|4|多应用模式中的公共浏览 (inPrivate)。|




