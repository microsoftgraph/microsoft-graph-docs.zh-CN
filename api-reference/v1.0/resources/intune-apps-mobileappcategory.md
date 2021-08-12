---
title: mobileAppCategory 资源类型
description: 包含单个 Intune 应用类别的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 51f316bb7a3b86c3e571c8af4d661f3820c4018dcd86508546c07d1a62419be9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235672"
---
# <a name="mobileappcategory-resource-type"></a>mobileAppCategory 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含单个 Intune 应用类别的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppCategories](../api/intune-apps-mobileappcategory-list.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|列出 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性和关系。|
|[获取 mobileAppCategory](../api/intune-apps-mobileappcategory-get.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|读取 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性和关系。|
|[创建 mobileAppCategory](../api/intune-apps-mobileappcategory-create.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|创建新的 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象。|
|[删除 mobileAppCategory](../api/intune-apps-mobileappcategory-delete.md)|无|删除 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)。|
|[更新 mobileAppCategory](../api/intune-apps-mobileappcategory-update.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|更新 [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|displayName|String|应用类别的名称。|
|lastModifiedDateTime|DateTimeOffset|上次修改 mobileAppCategory 的日期和时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```




