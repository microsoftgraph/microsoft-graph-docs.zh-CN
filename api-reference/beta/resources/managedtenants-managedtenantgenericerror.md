---
title: managedTenantGenericError 资源类型
description: 表示托管租户的一般错误。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d9cb6ac80bb48e7d8afc91db2cf386a21c7318e9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402025"
---
# <a name="managedtenantgenericerror-resource-type"></a>managedTenantGenericError 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示托管租户的一般错误。

继承自 [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|error|String|异常的错误消息。 继承自 [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md)。 必填。 只读。|
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
