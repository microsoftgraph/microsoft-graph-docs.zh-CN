---
title: suggestedEnrollmentLimit 资源类型
description: 当给定注册类型时，suggestedEnrollmentLimit 资源表示建议的注册限制。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 880fb5d77c7fa16a23349918973a33ba0952e07a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256258"
---
# <a name="suggestedenrollmentlimit-resource-type"></a>suggestedEnrollmentLimit 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

当给定注册类型时，suggestedEnrollmentLimit 资源表示建议的注册限制。

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|suggestedDailyLimit|Int32|一天内建议的登记限制|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.suggestedEnrollmentLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.suggestedEnrollmentLimit",
  "suggestedDailyLimit": 1024
}
```




