---
title: cartToClassAssociation 资源类型
description: 用于将设备购物车与教室关联的 CartToClassAssociation。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 952701547c2cdf8a8b7778316f7e1f28739279b3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333756"
---
# <a name="carttoclassassociation-resource-type"></a>cartToClassAssociation 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于将设备购物车与教室关联的 CartToClassAssociation。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 cartToClassAssociations](../api/intune-deviceconfig-carttoclassassociation-list.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)集合|列出[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象的属性和关系。|
|[获取 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|读取[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象的属性和关系。|
|[创建 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|创建新的[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象。|
|[删除 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-delete.md)|无|删除[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)。|
|[更新 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|更新[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。|
|version|Int32|CartToClassAssociation 的版本。|
|displayName|String|管理员提供的设备配置的名称。|
|说明|String|管理员提供的 CartToClassAssociation 说明。|
|deviceCartIds|String collection|要与类关联的设备购物车的标识符。|
|classroomIds|String collection|要与设备购物车关联的教室的标识符。|

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



