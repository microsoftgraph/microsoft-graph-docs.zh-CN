---
title: unifiedRoleManagementPolicyNotificationRule 资源类型
description: 一种派生自 unifiedRoleManagementPolicyRule 资源类型的类型，用于定义角色分配、激活和审批的电子邮件通知规则。
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a7f70afe8daa0bd296033be244bf2f7370ce1bdd
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898537"
---
# <a name="unifiedrolemanagementpolicynotificationrule-resource-type"></a>unifiedRoleManagementPolicyNotificationRule 资源类型

命名空间：microsoft.graph

一种派生自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 资源类型的类型，用于定义角色分配、激活和审批的电子邮件通知规则。

继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|规则的标识符。 继承自 [entity](../resources/entity.md)。|
|isDefaultRecipientsEnabled|Boolean|指示默认收件人是否会收到通知电子邮件。|
|notificationLevel|字符串|通知级别。 可能的值是 `None`， `Critical`. `All`|
|notificationRecipients|字符串集合|电子邮件通知的收件人列表。|
|notificationType|字符串|通知的类型。 仅 `Email` 支持。|
|recipientType|字符串|通知的收件人的类型。 可能的值是 `Requestor`， `Approver`. `Admin`|
|target|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|定义通知规则所针对的范围的详细信息。 详细信息可以包括主体类型、角色分配类型和影响角色的操作。 继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。 支持 `$filter`（`eq`、`ne`）。|

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
  "isDefaultRecipientsEnabled": "Boolean",
  "notificationRecipients": [
    "String"
  ]
}
```