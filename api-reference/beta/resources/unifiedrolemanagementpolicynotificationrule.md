---
title: unifiedRoleManagementPolicyNotificationRule 资源类型
description: unifiedRoleManagementPolicyNotificationRule 指定与角色管理策略关联的通知规则。 它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8f6c8324869fa7a6ec800368f7b47609abd7920b
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453644"
---
# <a name="unifiedrolemanagementpolicynotificationrule-resource-type"></a>unifiedRoleManagementPolicyNotificationRule 资源类型

命名空间：microsoft.graph

unifiedRoleManagementPolicyNotificationRule 指定与角色管理策略关联的通知规则。 它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。

继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|规则的唯一标识符。 继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|notificationLevel|String|通知级别。 None、Critical、All 之一。|
|notificationRecipients|字符串集合|通知接收者列表，如电子邮件。|
|notificationType|String|通知的类型。 电子邮件之一。|
|recipientType|String|收件人的类型。 请求者、审批者、管理员之一。|
|isDefaultRecipientsEnabled|Boolean|默认收件人是否收到电子邮件。|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|规则的目标。 继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "notificationType": "String",
  "recipientType": "String",
  "notificationLevel": "String",
  "isDefaultRecipientsEnabled": true,
  "notificationRecipients": [
    "String"
  ]
}
```

