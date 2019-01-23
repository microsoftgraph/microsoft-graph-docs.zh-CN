---
title: managedMobileApp 资源类型
description: 部署应用的标识符。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b8de88976937a967f60a0842eeb9f24b465e50f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419252"
---
# <a name="managedmobileapp-resource-type"></a>managedMobileApp 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

部署应用的标识符。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedMobileApps](../api/intune-mam-managedmobileapp-list.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合|列出 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性和关系。|
|[获取 managedMobileApp](../api/intune-mam-managedmobileapp-get.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|读取 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性和关系。|
|[创建 managedMobileApp](../api/intune-mam-managedmobileapp-create.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|创建新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。|
|[删除 managedMobileApp](../api/intune-mam-managedmobileapp-delete.md)|无|删除 [managedMobileApp](../resources/intune-mam-managedmobileapp.md)。|
|[更新 managedMobileApp](../api/intune-mam-managedmobileapp-update.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|更新 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|mobileAppIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|包含其操作系统类型的应用标识符。|
|id|String|实体的键。|
|version|String|实体的版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




