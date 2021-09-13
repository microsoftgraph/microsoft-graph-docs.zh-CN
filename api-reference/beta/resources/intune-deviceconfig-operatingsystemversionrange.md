---
title: operatingSystemVersionRange 资源类型
description: 操作系统版本范围。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1f9ceb269b541e303c7d240659777c1276a90c07
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101378"
---
# <a name="operatingsystemversionrange-resource-type"></a>operatingSystemVersionRange 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

操作系统版本范围。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|此范围的说明 (例如有效 1702 内部) |
|lowestVersion|String|此范围包含的最低包含版本。|
|highestVersion|String|此范围包含的最高包含版本。|

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



