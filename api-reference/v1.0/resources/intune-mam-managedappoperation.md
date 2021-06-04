---
title: managedAppOperation 资源类型
description: 表示对应用注册应用的操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6b435d9daedb7adcd630dd276241d39493d5b39d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754488"
---
# <a name="managedappoperation-resource-type"></a>managedAppOperation 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示对应用注册应用的操作。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
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




