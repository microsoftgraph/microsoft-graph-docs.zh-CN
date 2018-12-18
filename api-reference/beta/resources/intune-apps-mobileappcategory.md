---
title: mobileAppCategory 资源类型
description: 包含单个 Intune 应用类别的属性。
author: tfitzmac
ms.openlocfilehash: f40e9a24269d276c89d770acb0d772a7bdf94c51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340759"
---
# <a name="mobileappcategory-resource-type"></a>mobileAppCategory 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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





