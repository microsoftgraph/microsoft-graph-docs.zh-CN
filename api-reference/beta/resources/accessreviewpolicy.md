---
title: accessReviewPolicy 资源类型
description: 访问评审策略是使组织能够管理目录级别访问评审策略的单一单位。
author: kafen
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 02940987682d84aa3fc3dbb076c998abfe24bf8e
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067873"
---
# <a name="accessreviewpolicy-resource-type"></a>accessReviewPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

访问评审策略是使管理员能够管理目录级别访问评审策略的单一文件。 例如，管理员可以使用访问评审策略启用和禁用组所有者在自己拥有的组上创建访问评审的能力。


继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 accessReviewPolicy](../api/accessreviewpolicy-get.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|读取 [accessReviewPolicy](../resources/accessreviewpolicy.md) 对象的属性和关系。|
|[更新 accessReviewPolicy](../api/accessreviewpolicy-update.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|更新 [accessReviewPolicy 对象](../resources/accessreviewpolicy.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|此策略的说明。 只读。|
|displayName|String|此策略的显示名称。 只读。|
|isGroupOwnerManagementEnabled|布尔值|如果 `true` 为 ，组所有者可以在他们拥有的组上创建和管理访问评审。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewPolicy",
  "displayName": "Access Review Policy",
  "description": "Policy contains directory-level access review settings.",
  "isGroupOwnerManagementEnabled": false
}
```
