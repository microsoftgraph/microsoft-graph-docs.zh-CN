---
title: messageRule 资源类型
description: 适用于用户收件箱邮件的规则。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d5bd5cba444f03042e556906fc28e6a134f754d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021411"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="170aa-103">messageRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="170aa-103">messageRule resource type</span></span>

<span data-ttu-id="170aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="170aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="170aa-105">适用于用户收件箱邮件的规则。</span><span class="sxs-lookup"><span data-stu-id="170aa-105">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="170aa-106">在 Outlook 中，可以为收件箱中的传入邮件设置规则，以便在特定条件下执行具体操作。</span><span class="sxs-lookup"><span data-stu-id="170aa-106">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="170aa-107">可以按编程方式通过收件箱[文件夹](mailfolder.md)的 **messageRules** 导航属性来访问规则。</span><span class="sxs-lookup"><span data-stu-id="170aa-107">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="170aa-108">每个规则都由此 **messageRule** 资源表示，可用的规则操作由 [messageRuleActions](messageruleactions.md) 复杂类型表示，而可用的规则条件和例外则通过 [messageRulePredicates](messagerulepredicates.md) 复杂类型表示。</span><span class="sxs-lookup"><span data-stu-id="170aa-108">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="170aa-109">属性</span><span class="sxs-lookup"><span data-stu-id="170aa-109">Properties</span></span>
| <span data-ttu-id="170aa-110">属性</span><span class="sxs-lookup"><span data-stu-id="170aa-110">Property</span></span>     | <span data-ttu-id="170aa-111">类型</span><span class="sxs-lookup"><span data-stu-id="170aa-111">Type</span></span>   |<span data-ttu-id="170aa-112">说明</span><span class="sxs-lookup"><span data-stu-id="170aa-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="170aa-113">actions</span><span class="sxs-lookup"><span data-stu-id="170aa-113">actions</span></span> | [<span data-ttu-id="170aa-114">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="170aa-114">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="170aa-115">满足相应条件时对邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="170aa-115">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="170aa-116">conditions</span><span class="sxs-lookup"><span data-stu-id="170aa-116">conditions</span></span> | [<span data-ttu-id="170aa-117">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="170aa-117">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="170aa-118">满足条件时，将触发该规则的相应操作。</span><span class="sxs-lookup"><span data-stu-id="170aa-118">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="170aa-119">displayName</span><span class="sxs-lookup"><span data-stu-id="170aa-119">displayName</span></span> | <span data-ttu-id="170aa-120">String</span><span class="sxs-lookup"><span data-stu-id="170aa-120">String</span></span> | <span data-ttu-id="170aa-121">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="170aa-121">The display name of the rule.</span></span> |
| <span data-ttu-id="170aa-122">exceptions</span><span class="sxs-lookup"><span data-stu-id="170aa-122">exceptions</span></span> | [<span data-ttu-id="170aa-123">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="170aa-123">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="170aa-124">规则的例外情况。</span><span class="sxs-lookup"><span data-stu-id="170aa-124">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="170aa-125">hasError</span><span class="sxs-lookup"><span data-stu-id="170aa-125">hasError</span></span> | <span data-ttu-id="170aa-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="170aa-126">Boolean</span></span> | <span data-ttu-id="170aa-127">指示规则是否处于错误状态。</span><span class="sxs-lookup"><span data-stu-id="170aa-127">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="170aa-128">只读。</span><span class="sxs-lookup"><span data-stu-id="170aa-128">Read-only.</span></span> |
| <span data-ttu-id="170aa-129">id</span><span class="sxs-lookup"><span data-stu-id="170aa-129">id</span></span> |<span data-ttu-id="170aa-130">String</span><span class="sxs-lookup"><span data-stu-id="170aa-130">String</span></span>|<span data-ttu-id="170aa-131">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="170aa-131">The unique identifier of the rule.</span></span> <span data-ttu-id="170aa-132">只读。</span><span class="sxs-lookup"><span data-stu-id="170aa-132">Read-only.</span></span>|
| <span data-ttu-id="170aa-133">isEnabled</span><span class="sxs-lookup"><span data-stu-id="170aa-133">isEnabled</span></span> | <span data-ttu-id="170aa-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="170aa-134">Boolean</span></span> | <span data-ttu-id="170aa-135">指示是否启用规则以应用到邮件。</span><span class="sxs-lookup"><span data-stu-id="170aa-135">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="170aa-136">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="170aa-136">isReadOnly</span></span> | <span data-ttu-id="170aa-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="170aa-137">Boolean</span></span> | <span data-ttu-id="170aa-138">表示规则是否为只读且无法由规则 REST API 修改或删除。</span><span class="sxs-lookup"><span data-stu-id="170aa-138">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="170aa-139">Sequence</span><span class="sxs-lookup"><span data-stu-id="170aa-139">sequence</span></span> | <span data-ttu-id="170aa-140">Int32</span><span class="sxs-lookup"><span data-stu-id="170aa-140">Int32</span></span> | <span data-ttu-id="170aa-141">表示在其他规则中执行规则的顺序。</span><span class="sxs-lookup"><span data-stu-id="170aa-141">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="170aa-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="170aa-142">JSON representation</span></span>
<span data-ttu-id="170aa-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="170aa-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRule"
}-->

```json
{
  "actions": {"@odata.type": "microsoft.graph.messageRuleActions"},
  "conditions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "displayName": "String",
  "exceptions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "hasError": "Boolean",
  "id": "String",
  "isEnabled": "Boolean",
  "isReadOnly": "Boolean",
  "sequence": "Int32"
}

```

## <a name="methods"></a><span data-ttu-id="170aa-144">方法</span><span class="sxs-lookup"><span data-stu-id="170aa-144">Methods</span></span>
| <span data-ttu-id="170aa-145">方法</span><span class="sxs-lookup"><span data-stu-id="170aa-145">Method</span></span>           | <span data-ttu-id="170aa-146">返回类型</span><span class="sxs-lookup"><span data-stu-id="170aa-146">Return Type</span></span>    |<span data-ttu-id="170aa-147">说明</span><span class="sxs-lookup"><span data-stu-id="170aa-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="170aa-148">List rules</span><span class="sxs-lookup"><span data-stu-id="170aa-148">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="170aa-149">[messageRule](messagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="170aa-149">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="170aa-150">获取为用户收件箱定义的所有 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="170aa-150">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="170aa-151">Get rule</span><span class="sxs-lookup"><span data-stu-id="170aa-151">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="170aa-152">messageRule</span><span class="sxs-lookup"><span data-stu-id="170aa-152">messageRule</span></span>](messagerule.md) |<span data-ttu-id="170aa-153">读取 **messageRule** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="170aa-153">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="170aa-154">Create</span><span class="sxs-lookup"><span data-stu-id="170aa-154">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="170aa-155">messageRule</span><span class="sxs-lookup"><span data-stu-id="170aa-155">messageRule</span></span>](messagerule.md) |<span data-ttu-id="170aa-156">通过指定一组条件和操作来创建 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="170aa-156">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="170aa-157">Update</span><span class="sxs-lookup"><span data-stu-id="170aa-157">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="170aa-158">messageRule</span><span class="sxs-lookup"><span data-stu-id="170aa-158">messageRule</span></span>](messagerule.md) |<span data-ttu-id="170aa-159">为 **messageRule** 对象更改可写属性并保存更改。</span><span class="sxs-lookup"><span data-stu-id="170aa-159">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="170aa-160">删除</span><span class="sxs-lookup"><span data-stu-id="170aa-160">Delete</span></span>](../api/messagerule-delete.md) | <span data-ttu-id="170aa-161">无</span><span class="sxs-lookup"><span data-stu-id="170aa-161">None</span></span> |<span data-ttu-id="170aa-162">删除指定的 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="170aa-162">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


