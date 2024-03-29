---
title: mobileAppRelationship 资源类型
description: 描述两个移动应用程序之间的关系。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6e3a355b2eab4c70349156a921d508f33705c65c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59124152"
---
# <a name="mobileapprelationship-resource-type"></a>mobileAppRelationship 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述两个移动应用程序之间的关系。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppRelationships](../api/intune-apps-mobileapprelationship-list.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) 集合|列出 [mobileAppRelationship 对象的属性和](../resources/intune-apps-mobileapprelationship.md) 关系。|
|[获取 mobileAppRelationship](../api/intune-apps-mobileapprelationship-get.md)|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|读取 [mobileAppRelationship 对象的属性和](../resources/intune-apps-mobileapprelationship.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|关系实体 ID。|
|targetId|String|目标移动应用的应用 ID。|
|targetDisplayName|String|目标移动应用显示名称。|
|targetDisplayVersion|String|目标移动应用的显示版本。|
|targetPublisher|String|目标移动应用的发布者。|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|关系类型，指示目标是父对象还是子级。 可取值为：`child`、`parent`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppRelationship"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppRelationship",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "targetDisplayVersion": "String",
  "targetPublisher": "String",
  "targetType": "String"
}
```



