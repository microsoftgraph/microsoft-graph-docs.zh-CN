---
title: messageRule 资源类型
description: 适用于用户收件箱邮件的规则。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 9336f2e35d6c68d86c3e92b5f94c024eff1e49a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862123"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="6b0a5-103">messageRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b0a5-103">messageRule resource type</span></span>


<span data-ttu-id="6b0a5-104">适用于用户收件箱邮件的规则。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-104">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="6b0a5-105">在 Outlook 中，可以为收件箱中的传入邮件设置规则，以便在特定条件下执行具体操作。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-105">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="6b0a5-106">可以按编程方式通过收件箱[文件夹](mailfolder.md)的 **messageRules** 导航属性来访问规则。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-106">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="6b0a5-107">每个规则都由此 **messageRule** 资源表示，可用的规则操作由 [messageRuleActions](messageruleactions.md) 复杂类型表示，而可用的规则条件和例外则通过 [messageRulePredicates](messagerulepredicates.md) 复杂类型表示。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-107">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="6b0a5-108">属性</span><span class="sxs-lookup"><span data-stu-id="6b0a5-108">Properties</span></span>
| <span data-ttu-id="6b0a5-109">属性</span><span class="sxs-lookup"><span data-stu-id="6b0a5-109">Property</span></span>     | <span data-ttu-id="6b0a5-110">类型</span><span class="sxs-lookup"><span data-stu-id="6b0a5-110">Type</span></span>   |<span data-ttu-id="6b0a5-111">说明</span><span class="sxs-lookup"><span data-stu-id="6b0a5-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6b0a5-112">actions</span><span class="sxs-lookup"><span data-stu-id="6b0a5-112">actions</span></span> | [<span data-ttu-id="6b0a5-113">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="6b0a5-113">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="6b0a5-114">满足相应条件时对邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-114">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="6b0a5-115">conditions</span><span class="sxs-lookup"><span data-stu-id="6b0a5-115">conditions</span></span> | [<span data-ttu-id="6b0a5-116">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="6b0a5-116">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="6b0a5-117">满足条件时，将触发该规则的相应操作。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-117">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="6b0a5-118">displayName</span><span class="sxs-lookup"><span data-stu-id="6b0a5-118">displayName</span></span> | <span data-ttu-id="6b0a5-119">String</span><span class="sxs-lookup"><span data-stu-id="6b0a5-119">String</span></span> | <span data-ttu-id="6b0a5-120">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-120">The display name of the rule.</span></span> |
| <span data-ttu-id="6b0a5-121">exceptions</span><span class="sxs-lookup"><span data-stu-id="6b0a5-121">exceptions</span></span> | [<span data-ttu-id="6b0a5-122">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="6b0a5-122">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="6b0a5-123">规则的例外情况。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-123">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="6b0a5-124">hasError</span><span class="sxs-lookup"><span data-stu-id="6b0a5-124">hasError</span></span> | <span data-ttu-id="6b0a5-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b0a5-125">Boolean</span></span> | <span data-ttu-id="6b0a5-126">指示规则是否处于错误状态。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-126">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="6b0a5-127">只读。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-127">Read-only.</span></span> |
| <span data-ttu-id="6b0a5-128">id</span><span class="sxs-lookup"><span data-stu-id="6b0a5-128">id</span></span> |<span data-ttu-id="6b0a5-129">String</span><span class="sxs-lookup"><span data-stu-id="6b0a5-129">String</span></span>|<span data-ttu-id="6b0a5-130">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-130">The unique identifier of the rule.</span></span> <span data-ttu-id="6b0a5-131">只读。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-131">Read-only.</span></span>|
| <span data-ttu-id="6b0a5-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="6b0a5-132">isEnabled</span></span> | <span data-ttu-id="6b0a5-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b0a5-133">Boolean</span></span> | <span data-ttu-id="6b0a5-134">指示是否启用规则以应用到邮件。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-134">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="6b0a5-135">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="6b0a5-135">isReadOnly</span></span> | <span data-ttu-id="6b0a5-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b0a5-136">Boolean</span></span> | <span data-ttu-id="6b0a5-137">表示规则是否为只读且无法由规则 REST API 修改或删除。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-137">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="6b0a5-138">Sequence</span><span class="sxs-lookup"><span data-stu-id="6b0a5-138">sequence</span></span> | <span data-ttu-id="6b0a5-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6b0a5-139">Int32</span></span> | <span data-ttu-id="6b0a5-140">表示在其他规则中执行规则的顺序。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-140">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="6b0a5-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b0a5-141">JSON representation</span></span>
<span data-ttu-id="6b0a5-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
   "baseType": "microsoft.graph.entity",
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

## <a name="methods"></a><span data-ttu-id="6b0a5-143">方法</span><span class="sxs-lookup"><span data-stu-id="6b0a5-143">Methods</span></span>
| <span data-ttu-id="6b0a5-144">方法</span><span class="sxs-lookup"><span data-stu-id="6b0a5-144">Method</span></span>           | <span data-ttu-id="6b0a5-145">返回类型</span><span class="sxs-lookup"><span data-stu-id="6b0a5-145">Return Type</span></span>    |<span data-ttu-id="6b0a5-146">说明</span><span class="sxs-lookup"><span data-stu-id="6b0a5-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6b0a5-147">List rules</span><span class="sxs-lookup"><span data-stu-id="6b0a5-147">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="6b0a5-148">[messageRule](messagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b0a5-148">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="6b0a5-149">获取为用户收件箱定义的所有 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-149">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="6b0a5-150">Get rule</span><span class="sxs-lookup"><span data-stu-id="6b0a5-150">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="6b0a5-151">messageRule</span><span class="sxs-lookup"><span data-stu-id="6b0a5-151">messageRule</span></span>](messagerule.md) |<span data-ttu-id="6b0a5-152">读取 **messageRule** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-152">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="6b0a5-153">Create</span><span class="sxs-lookup"><span data-stu-id="6b0a5-153">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="6b0a5-154">messageRule</span><span class="sxs-lookup"><span data-stu-id="6b0a5-154">messageRule</span></span>](messagerule.md) |<span data-ttu-id="6b0a5-155">通过指定一组条件和操作来创建 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-155">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="6b0a5-156">Update</span><span class="sxs-lookup"><span data-stu-id="6b0a5-156">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="6b0a5-157">messageRule</span><span class="sxs-lookup"><span data-stu-id="6b0a5-157">messageRule</span></span>](messagerule.md) |<span data-ttu-id="6b0a5-158">为 **messageRule** 对象更改可写属性并保存更改。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-158">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="6b0a5-159">Delete</span><span class="sxs-lookup"><span data-stu-id="6b0a5-159">Delete</span></span>](../api/messagerule-delete.md) | <span data-ttu-id="6b0a5-160">无</span><span class="sxs-lookup"><span data-stu-id="6b0a5-160">None</span></span> |<span data-ttu-id="6b0a5-161">删除指定的 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="6b0a5-161">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
