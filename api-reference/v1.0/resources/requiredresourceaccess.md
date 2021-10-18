---
title: requiredResourceAccess 资源类型
description: 指定 OAuth 2.0 权限范围的应用程序角色集。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 374d88cd9cc0166c003618af4382aafe498eaf87
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60452830"
---
# <a name="requiredresourceaccess-resource-type"></a>requiredResourceAccess 资源类型

命名空间：microsoft.graph

指定应用程序需要访问的指定资源下的 OAuth 2.0 权限范围和应用角色集。 [应用程序可以通过](application.md) **requiredResourceAccess 属性（requiredResourceAccess** 对象的集合）请求指定的 OAuth 2.0 权限范围 [或应用](requiredresourceaccess.md)角色。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|resourceAccess|[resourceAccess](resourceaccess.md) 集合|应用程序从指定资源请求的 OAuth2.0 权限范围和应用角色列表。|
|resourceAppId|String|应用程序需要访问的资源的唯一标识符。 这应该等于在目标资源应用程序上声明的 **appId。**|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [
    {
      "@odata.type": "microsoft.graph.resourceAccess"
    }
  ],
  "resourceAppId": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

