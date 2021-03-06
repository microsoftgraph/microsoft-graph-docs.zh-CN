---
title: managedEBookCategory 资源类型
description: 包含单个 Intune 电子书类别的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 140552741ba3d08ab1821508de0e283ab5b3e6a9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295255"
---
# <a name="managedebookcategory-resource-type"></a>managedEBookCategory 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含单个 Intune 电子书类别的属性。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 managedEBookCategories](../api/intune-books-managedebookcategory-list.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md) 集合|列出 [managedEBookCategory](../resources/intune-books-managedebookcategory.md) 对象的属性和关系。|
|[获取 managedEBookCategory](../api/intune-books-managedebookcategory-get.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|读取 [managedEBookCategory](../resources/intune-books-managedebookcategory.md) 对象的属性和关系。|
|[创建 managedEBookCategory](../api/intune-books-managedebookcategory-create.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|创建新的 [managedEBookCategory](../resources/intune-books-managedebookcategory.md) 对象。|
|[删除 managedEBookCategory](../api/intune-books-managedebookcategory-delete.md)|无|删除 [managedEBookCategory](../resources/intune-books-managedebookcategory.md)。|
|[更新 managedEBookCategory](../api/intune-books-managedebookcategory-update.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|更新 [managedEBookCategory](../resources/intune-books-managedebookcategory.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。|
|displayName|字符串|电子书类别的名称。|
|lastModifiedDateTime|DateTimeOffset|上次修改 ManagedEBookCategory 的日期和时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```




