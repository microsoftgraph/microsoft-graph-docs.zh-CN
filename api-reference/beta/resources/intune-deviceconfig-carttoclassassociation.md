---
title: cartToClassAssociation 资源类型
description: 与教室关联设备车 CartToClassAssociation。
author: tfitzmac
ms.openlocfilehash: f712759d82b5edf7d364658211f1f2142fb6eb87
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328278"
---
# <a name="carttoclassassociation-resource-type"></a>cartToClassAssociation 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

与教室关联设备车 CartToClassAssociation。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 cartToClassAssociations](../api/intune-deviceconfig-carttoclassassociation-list.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)集合|列出属性和[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象之间的关系。|
|[获取 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|读取属性和[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象的关系。|
|[创建 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|创建新的[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象。|
|[删除 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-delete.md)|无|删除[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)。|
|[更新 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|更新[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。|
|version|Int32|CartToClassAssociation 版本。|
|displayName|String|管理员提供的设备配置的名称。|
|说明|字符串|管理员提供 CartToClassAssociation 的说明。|
|deviceCartIds|String 集合|设备车与类相关联的标识符。|
|classroomIds|String 集合|教室与设备车相关联的标识符。|

## <a name="relationships"></a>Relationships
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





