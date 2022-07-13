---
title: externalIdentitiesPolicy 资源类型
description: 表示租户范围的策略，该策略控制外部用户是否可以通过自助式控制离开 Azure AD 租户。
author: KuiGithui
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 49701027e0dace54a8f74a2eebef0115329de9a4
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768339"
---
# <a name="externalidentitiespolicy-resource-type"></a>externalIdentitiesPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户范围的策略，该策略控制外部用户是否可以通过自助式控制离开来宾 Azure AD 租户。 如果管理员允许，外部用户可以通过 [“我的帐户](https://myaccount.microsoft.com/)”门户的 **组织** 菜单离开来宾 Azure AD 租户。

继承自 [policyBase](../resources/policybase.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 externalIdentitiesPolicy](../api/externalidentitiespolicy-get.md)|[externalIdentitiesPolicy](../resources/externalidentitiespolicy.md)|读取 [externalIdentitiesPolicy](../resources/externalidentitiespolicy.md) 对象的属性和关系。|
|[更新 externalIdentitiesPolicy](../api/externalidentitiespolicy-update.md)|[externalIdentitiesPolicy](../resources/externalidentitiespolicy.md)|更新 [externalIdentitiesPolicy 对象的](../resources/externalidentitiespolicy.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowDeletedIdentitiesDataRemoval|Boolean|通知 Azure AD 在用户在其主租户中删除用户时，是否从来宾租户中清理有关外部标识的用户信息。 |
|allowExternalIdentitiesToLeave|布尔值|定义外部用户是否可以离开来宾租户。 如果设置为 `false`，则不会启用自助服务控件，并且来宾租户的管理员必须手动从来宾租户中删除外部用户。|
|displayName|String|策略名称。 继承自 [policyBase](../resources/policybase.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalIdentitiesPolicy",
  "baseType": "microsoft.graph.policyBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalIdentitiesPolicy",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "allowExternalIdentitiesToLeave": "Boolean",
  "allowDeletedIdentitiesDataRemoval": "Boolean"
}
```

