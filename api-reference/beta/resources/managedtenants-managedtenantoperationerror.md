---
title: managedTenantOperationError 资源类型
description: 表示托管租户操作的错误的抽象类型。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 3708f0a2727a59390dc0c91c26191d12a9f28b0e
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791887"
---
# <a name="managedtenantoperationerror-resource-type"></a>managedTenantOperationError 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示托管租户操作的错误的抽象类型。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|error|String|异常的错误消息。|
|tenantId|String|托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantOperationError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantOperationError",
  "tenantId": "String",
  "error": "String"
}
```
