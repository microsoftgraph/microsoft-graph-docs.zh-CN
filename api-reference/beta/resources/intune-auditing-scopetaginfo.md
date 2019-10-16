---
title: scopeTagInfo 资源类型
description: 包含 Scope 标记对象的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8238881d8a14cb8aa1dfcc01031105be0069c21
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538502"
---
# <a name="scopetaginfo-resource-type"></a>scopeTagInfo 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Scope 标记对象的属性的类。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|scopeTagName|字符串|范围标记显示名称。|
|scopeTagId|字符串|范围标记 Id。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.scopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.scopeTagInfo",
  "scopeTagName": "String",
  "scopeTagId": "String"
}
```



