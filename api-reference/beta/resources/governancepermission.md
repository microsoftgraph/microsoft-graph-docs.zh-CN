---
title: governancePermission 资源类型
description: '表示 governanceSubject 对特定 governanceResource 具有的访问权限。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: f316a863ecba9ed546b9ba4045e57ada87e97ab9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128832"
---
# <a name="governancepermission-resource-type"></a>governancePermission 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [governanceSubject](../resources/governancesubject.md) 对特定 [governanceResource 具有的访问权限](../resources/governanceresource.md)。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accessLevel|字符串|访问级别。 有效值： ``None`` 、 ``UserRead`` 和 ``AdminRead`` ``AdminReadWrite`` 。|
|isActive|Boolean|指示请求程序是否具有访问角色分配活动应用程序。|
|isEligible|Boolean|指示请求者是否具有访问角色分配条件。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governancePermission"
}-->
```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```


