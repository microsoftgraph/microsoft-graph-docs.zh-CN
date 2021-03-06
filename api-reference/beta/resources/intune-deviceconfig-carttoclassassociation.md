---
title: cartToClassAssociation 资源类型
description: 用于将设备购物车与教室关联的 CartToClassAssociation。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 16026ff5a89dc43aabb92dc64f0f95524f8fafef
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260486"
---
# <a name="carttoclassassociation-resource-type"></a>cartToClassAssociation 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于将设备购物车与教室关联的 CartToClassAssociation。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 cartToClassAssociations](../api/intune-deviceconfig-carttoclassassociation-list.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 集合|列出 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 对象的属性和关系。|
|[获取 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|读取 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 对象的属性和关系。|
|[创建 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|创建新的 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 对象。|
|[删除 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-delete.md)|无|删除 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)。|
|[更新 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|更新 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。|
|version|Int32|CartToClassAssociation 的版本。|
|displayName|String|管理员提供的设备配置的名称。|
|description|String|管理员提供的 CartToClassAssociation 说明。|
|deviceCartIds|String 集合|要与类关联的设备购物车的标识符。|
|classroomIds|String 集合|要与设备购物车关联的教室的标识符。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cartToClassAssociation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "deviceCartIds": [
    "String"
  ],
  "classroomIds": [
    "String"
  ]
}
```




