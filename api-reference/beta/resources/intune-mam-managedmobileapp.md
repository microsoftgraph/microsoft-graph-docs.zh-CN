---
title: managedMobileApp 资源类型
description: 部署应用的标识符。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: acd69164becf0b0199c9ddc845b8e45afb4420a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838414"
---
# <a name="managedmobileapp-resource-type"></a>managedMobileApp 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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





