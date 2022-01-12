---
title: managedTenantGenericError 资源类型
description: 表示托管租户的常规错误。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 167d8a581f2e8020ea4efabf951d07c409947ef3
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61789976"
---
# <a name="managedtenantgenericerror-resource-type"></a>managedTenantGenericError 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示托管租户的常规错误。

继承自 [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|error|String|异常的错误消息。 继承自 [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md)。 必需。 只读。|
|tenantId|String|托管Azure Active Directory租户的租户标识符。 继承自 [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md)。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantGenericError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantGenericError",
  "tenantId": "String",
  "error": "String"
}
```
