---
title: externalDomainName 资源类型
description: 充当资源租户Azure Active Directory (Azure AD) 租户尝试设置联盟的外部组织的域名。
author: namkedia
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a84c13d4800d79263ef63423ef390846eecb5ec2
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697006"
---
# <a name="externaldomainname-resource-type"></a>externalDomainName 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示作为资源租户Azure Active Directory (Azure AD) 租户尝试设置联盟的外部组织的域名。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
无。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Azure AD 租户与外部组织的域名。 继承自 [实体](../resources/entity.md)。|

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
