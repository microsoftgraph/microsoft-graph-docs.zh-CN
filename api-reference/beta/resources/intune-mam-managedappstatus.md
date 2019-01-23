---
title: managedAppStatus 资源类型
description: 表示组织的应用保护和配置状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7625543106b1ccf019df9622c1b0f37d40232f0c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415563"
---
# <a name="managedappstatus-resource-type"></a>managedAppStatus 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示组织的应用保护和配置状态。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedAppStatuses](../api/intune-mam-managedappstatus-list.md)|[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合|列出 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。|
|[获取 managedAppStatus](../api/intune-mam-managedappstatus-get.md)|[managedAppStatus](../resources/intune-mam-managedappstatus.md)|读取 [managedAppStatus](../resources/intune-mam-managedappstatus.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|状态报告的友好名称。|
|id|String|实体的键。|
|version|String|实体的版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```




