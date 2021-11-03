---
title: governancePermission 资源类型
description: '表示 governanceSubject 对特定 governanceResource 具有的访问权限。  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 0cb80e78e3cbdb2c019347d28ff79be262ec7b99
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696215"
---
# <a name="governancepermission-resource-type"></a>governancePermission 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1resourceroles-deprecation](../../includes/pim-v1resourceroles-deprecation.md)]

表示 [governanceSubject](../resources/governancesubject.md) 对特定 [governanceResource 具有的访问权限](../resources/governanceresource.md)。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accessLevel|String|访问级别。 有效值 ``None`` ``UserRead`` ：、、 ``AdminRead`` 和 ``AdminReadWrite`` 。|
|isActive|布尔值|指示请求程序是否具有访问角色分配活动状态。|
|isEligible|布尔值|指示请求者是否有符合访问角色分配条件。|

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


