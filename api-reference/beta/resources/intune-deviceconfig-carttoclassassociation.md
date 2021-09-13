---
title: cartToClassAssociation 资源类型
description: CartToClassAssociation，用于将设备购物车与教室关联。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 10050d3cb9bcc73549244f07077f4c4b7de97bf3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127477"
---
# <a name="carttoclassassociation-resource-type"></a>cartToClassAssociation 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

CartToClassAssociation，用于将设备购物车与教室关联。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 cartToClassAssociations](../api/intune-deviceconfig-carttoclassassociation-list.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 集合|列出 [cartToClassAssociation 对象的属性和](../resources/intune-deviceconfig-carttoclassassociation.md) 关系。|
|[获取 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|读取 [cartToClassAssociation 对象的属性和](../resources/intune-deviceconfig-carttoclassassociation.md) 关系。|
|[创建 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|创建新的 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 对象。|
|[删除 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-delete.md)|无|删除 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)。|
|[更新 cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|更新 [cartToClassAssociation 对象](../resources/intune-deviceconfig-carttoclassassociation.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。|
|version|Int32|CartToClassAssociation 的版本。|
|displayName|String|管理员提供的设备配置的名称。|
|说明|String|管理员提供了 CartToClassAssociation 的说明。|
|deviceCartIds|字符串集合|要与类关联的设备购物车的标识符。|
|classroomIds|字符串集合|要与设备购物车关联的教室的标识符。|

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



