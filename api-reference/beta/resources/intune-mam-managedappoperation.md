---
title: managedAppOperation 资源类型
description: 表示对应用注册应用的操作。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cb72c4bf8cf7f2a4a55790087c3d46746c46a84a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424656"
---
# <a name="managedappoperation-resource-type"></a>managedAppOperation 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示对应用注册应用的操作。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedAppOperations](../api/intune-mam-managedappoperation-list.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md) 集合|列出 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。|
|[获取 managedAppOperation](../api/intune-mam-managedappoperation-get.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|读取 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性和关系。|
|[创建 managedAppOperation](../api/intune-mam-managedappoperation-create.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|创建新的 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象。|
|[删除 managedAppOperation](../api/intune-mam-managedappoperation-delete.md)|无|删除 [managedAppOperation](../resources/intune-mam-managedappoperation.md)。|
|[更新 managedAppOperation](../api/intune-mam-managedappoperation-update.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|更新 [managedAppOperation](../resources/intune-mam-managedappoperation.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|操作名称。|
|lastModifiedDateTime|DateTimeOffset|上次修改应用操作的时间。|
|state|String|操作的当前状态|
|id|String|实体的键。|
|version|String|实体的版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```




