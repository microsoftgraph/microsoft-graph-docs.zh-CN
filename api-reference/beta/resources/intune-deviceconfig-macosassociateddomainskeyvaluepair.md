---
title: macOSAssociatedDomainsKeyValuePair 资源类型
description: 关联域的键值对
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ebf62a01d4a97fde51974ea2e7984b97c39dc5d4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439720"
---
# <a name="macosassociateddomainskeyvaluepair-resource-type"></a>macOSAssociatedDomainsKeyValuePair 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

关联域的键值对


继承自[keyValuePair](../resources/intune-shared-keyvaluepair.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|String|从[KeyValuePair](../resources/intune-shared-keyvaluepair.md)继承的此键/值对的名称|
|value|String|从[KeyValuePair](../resources/intune-shared-keyvaluepair.md)继承的此键/值对的值|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAssociatedDomainsKeyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAssociatedDomainsKeyValuePair",
  "name": "String",
  "value": "String"
}
```



