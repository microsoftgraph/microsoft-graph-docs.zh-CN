---
title: managedEBookCategory 资源类型
description: 包含单个 Intune 电子图书类别的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df057c3aa05d181365397d150aeae93754b63dad
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415332"
---
# <a name="managedebookcategory-resource-type"></a>managedEBookCategory 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含单个 Intune 电子图书类别的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 managedEBookCategories](../api/intune-books-managedebookcategory-list.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)集合|列出属性和[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象之间的关系。|
|[获取 managedEBookCategory](../api/intune-books-managedebookcategory-get.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|读取属性和[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的关系。|
|[创建 managedEBookCategory](../api/intune-books-managedebookcategory-create.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|创建新的[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象。|
|[删除 managedEBookCategory](../api/intune-books-managedebookcategory-delete.md)|无|删除[managedEBookCategory](../resources/intune-books-managedebookcategory.md)。|
|[更新 managedEBookCategory](../api/intune-books-managedebookcategory-update.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|更新[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|displayName|String|电子图书类别的名称。|
|lastModifiedDateTime|DateTimeOffset|日期和 ManagedEBookCategory 上次修改的时间。|

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




