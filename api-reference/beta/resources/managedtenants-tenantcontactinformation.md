---
title: tenantContactInformation 资源类型
description: 表示托管租户的联系人。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: f852bbae5a08c00d101e122443b9e5b50382eb62
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860458"
---
# <a name="tenantcontactinformation-resource-type"></a>tenantContactInformation 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示托管租户的联系人。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|email|String|联系人的电子邮件地址。 可选|
|name|String|联系人的名称。 必需。|
|notes|String|与联系人关联的注释。 可选|
|phone|String|联系人的电话号码。 可选。|
|title|String|联系人的标题。 必填。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantContactInformation",
  "name": "String",
  "title": "String",
  "email": "String",
  "phone": "String",
  "notes": "String"
}
```
