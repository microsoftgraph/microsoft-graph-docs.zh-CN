---
title: operatingSystemVersionRange 资源类型
description: 操作系统版本范围。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e9019150efed2f52f884746d7c62f1d7e5a35e83
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293953"
---
# <a name="operatingsystemversionrange-resource-type"></a>operatingSystemVersionRange 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

操作系统版本范围。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|字符串|此范围的说明 (例如，有效的1702版本) |
|lowestVersion|字符串|此范围包含的最低包含版本。|
|highestVersion|字符串|此范围包含的最高包含版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```




