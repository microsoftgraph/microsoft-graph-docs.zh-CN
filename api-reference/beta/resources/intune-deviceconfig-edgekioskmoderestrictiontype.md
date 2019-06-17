---
title: edgeKioskModeRestrictionType 枚举类型
description: 根据展台模式指定 Microsoft Edge 设置的限制方式。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5dc2aa6dbea5e5fc068691c7de878321047c967d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989824"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a>edgeKioskModeRestrictionType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

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





