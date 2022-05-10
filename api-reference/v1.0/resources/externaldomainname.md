---
title: externalDomainName 资源类型
description: 充当资源租户的Azure Active Directory (Azure AD) 租户所与之联合的外部组织的域名。
author: namkedia
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: de723382ddfdbb7ef68c871e84498560d2b03ce8
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296571"
---
# <a name="externaldomainname-resource-type"></a>externalDomainName 资源类型

命名空间：microsoft.graph

表示充当资源租户的Azure Active Directory (Azure AD) 租户所与之联合的外部组织的域名。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>方法
无。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Azure AD租户联合的外部组织的域名。 继承自 [entity](../resources/entity.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalDomainName",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalDomainName",
  "id": "String (identifier)"
}
```
