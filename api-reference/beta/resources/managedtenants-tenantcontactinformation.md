---
title: tenantContactInformation 资源类型
description: 表示托管租户的联系人。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: b60005cf60a9ac1b96a3b650a853f8b198d27e48
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402394"
---
# <a name="tenantcontactinformation-resource-type"></a>tenantContactInformation 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示托管租户的联系人。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|email|String|联系人的电子邮件地址。 可选|
|name|String|联系人的名称。 必填。|
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
