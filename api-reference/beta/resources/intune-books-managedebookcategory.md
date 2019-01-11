---
title: managedEBookCategory 资源类型
description: 包含单个 Intune 电子图书类别的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b415554d47c33f06a917c10327dad983db762578
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894185"
---
# <a name="managedebookcategory-resource-type"></a>managedEBookCategory 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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
|displayName|字符串|电子图书类别的名称。|
|lastModifiedDateTime|DateTimeOffset|日期和 ManagedEBookCategory 上次修改的时间。|

## <a name="relationships"></a>Relationships
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





