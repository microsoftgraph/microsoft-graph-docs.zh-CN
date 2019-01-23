---
title: mobileAppCategory 资源类型
description: 包含单个 Intune 应用类别的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 59f840bdd3a01ca8f8614f6e14e53d9ba95005dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422262"
---
# <a name="mobileappcategory-resource-type"></a>mobileAppCategory 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




