---
title: unifiedRoleManagementPolicyNotificationRule 资源类型
description: unifiedRoleManagementPolicyNotificationRule 指定与角色管理策略关联的通知规则。 它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c4392055d199e444acefa497a009cf5b71cb8cda
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680197"
---
# <a name="unifiedrolemanagementpolicynotificationrule-resource-type"></a><span data-ttu-id="07967-104">unifiedRoleManagementPolicyNotificationRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="07967-104">unifiedRoleManagementPolicyNotificationRule resource type</span></span>

<span data-ttu-id="07967-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07967-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="07967-106">unifiedRoleManagementPolicyNotificationRule 指定与角色管理策略关联的通知规则。</span><span class="sxs-lookup"><span data-stu-id="07967-106">A unifiedRoleManagementPolicyNotificationRule specifies the notification rule associated with a role management policy.</span></span> <span data-ttu-id="07967-107">它派生自 microsoft.graph.unifiedRoleManagementPolicyRule。</span><span class="sxs-lookup"><span data-stu-id="07967-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="07967-108">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)。</span><span class="sxs-lookup"><span data-stu-id="07967-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="07967-109">属性</span><span class="sxs-lookup"><span data-stu-id="07967-109">Properties</span></span>
|<span data-ttu-id="07967-110">属性</span><span class="sxs-lookup"><span data-stu-id="07967-110">Property</span></span>|<span data-ttu-id="07967-111">类型</span><span class="sxs-lookup"><span data-stu-id="07967-111">Type</span></span>|<span data-ttu-id="07967-112">说明</span><span class="sxs-lookup"><span data-stu-id="07967-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07967-113">id</span><span class="sxs-lookup"><span data-stu-id="07967-113">id</span></span>|<span data-ttu-id="07967-114">String</span><span class="sxs-lookup"><span data-stu-id="07967-114">String</span></span>|<span data-ttu-id="07967-115">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="07967-115">Unique identifier for the rule.</span></span> <span data-ttu-id="07967-116">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="07967-116">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="07967-117">notificationLevel</span><span class="sxs-lookup"><span data-stu-id="07967-117">notificationLevel</span></span>|<span data-ttu-id="07967-118">String</span><span class="sxs-lookup"><span data-stu-id="07967-118">String</span></span>|<span data-ttu-id="07967-119">通知级别。</span><span class="sxs-lookup"><span data-stu-id="07967-119">The level of notification.</span></span> <span data-ttu-id="07967-120">None、Critical、All 之一。</span><span class="sxs-lookup"><span data-stu-id="07967-120">One of None, Critical, All.</span></span>|
|<span data-ttu-id="07967-121">notificationRecipients</span><span class="sxs-lookup"><span data-stu-id="07967-121">notificationRecipients</span></span>|<span data-ttu-id="07967-122">String collection</span><span class="sxs-lookup"><span data-stu-id="07967-122">String collection</span></span>|<span data-ttu-id="07967-123">通知接收者列表，如电子邮件。</span><span class="sxs-lookup"><span data-stu-id="07967-123">The list of notification recepients like email.</span></span>|
|<span data-ttu-id="07967-124">notificationType</span><span class="sxs-lookup"><span data-stu-id="07967-124">notificationType</span></span>|<span data-ttu-id="07967-125">String</span><span class="sxs-lookup"><span data-stu-id="07967-125">String</span></span>|<span data-ttu-id="07967-126">通知的类型。</span><span class="sxs-lookup"><span data-stu-id="07967-126">The type of notification.</span></span> <span data-ttu-id="07967-127">电子邮件之一。</span><span class="sxs-lookup"><span data-stu-id="07967-127">One of Email.</span></span>|
|<span data-ttu-id="07967-128">recipientType</span><span class="sxs-lookup"><span data-stu-id="07967-128">recipientType</span></span>|<span data-ttu-id="07967-129">String</span><span class="sxs-lookup"><span data-stu-id="07967-129">String</span></span>|<span data-ttu-id="07967-130">收件人的类型。</span><span class="sxs-lookup"><span data-stu-id="07967-130">The type of recipient.</span></span> <span data-ttu-id="07967-131">请求者、审批者、管理员之一。</span><span class="sxs-lookup"><span data-stu-id="07967-131">One of Requestor, Approver, Admin.</span></span>|
|<span data-ttu-id="07967-132">isDefaultRecipientsEnabled</span><span class="sxs-lookup"><span data-stu-id="07967-132">isDefaultRecipientsEnabled</span></span>|<span data-ttu-id="07967-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="07967-133">Boolean</span></span>|<span data-ttu-id="07967-134">默认收件人是否收到电子邮件。</span><span class="sxs-lookup"><span data-stu-id="07967-134">Whether default recipient is receiving the email or not.</span></span>|
|<span data-ttu-id="07967-135">target</span><span class="sxs-lookup"><span data-stu-id="07967-135">target</span></span>|[<span data-ttu-id="07967-136">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="07967-136">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="07967-137">规则的目标。</span><span class="sxs-lookup"><span data-stu-id="07967-137">The target for the rule.</span></span> <span data-ttu-id="07967-138">继承自 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="07967-138">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="07967-139">关系</span><span class="sxs-lookup"><span data-stu-id="07967-139">Relationships</span></span>
<span data-ttu-id="07967-140">无。</span><span class="sxs-lookup"><span data-stu-id="07967-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07967-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07967-141">JSON representation</span></span>
<span data-ttu-id="07967-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07967-142">The following is a JSON representation of the resource.</span></span>
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

