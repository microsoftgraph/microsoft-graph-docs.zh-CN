---
title: messageRule 资源类型
description: 适用于用户收件箱邮件的规则。
author: angelgolfer-ms
ms.openlocfilehash: 1824e9a8d840da824efb79eff4b98bac02a8c187
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307726"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="e0cf3-103">messageRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0cf3-103">messageRule resource type</span></span>

> <span data-ttu-id="e0cf3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0cf3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e0cf3-106">适用于用户收件箱邮件的规则。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-106">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="e0cf3-107">在 Outlook 中，可以为收件箱中的传入邮件设置规则，以便在特定条件下执行具体操作。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-107">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="e0cf3-108">可以按编程方式通过收件箱[文件夹](mailfolder.md)的 **messageRules** 导航属性来访问规则。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-108">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="e0cf3-109">每个规则都由此 **messageRule** 资源表示，可用的规则操作由 [messageRuleActions](messageruleactions.md) 复杂类型表示，而可用的规则条件和例外则通过 [messageRulePredicates](messagerulepredicates.md) 复杂类型表示。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-109">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="e0cf3-110">属性</span><span class="sxs-lookup"><span data-stu-id="e0cf3-110">Properties</span></span>
| <span data-ttu-id="e0cf3-111">属性</span><span class="sxs-lookup"><span data-stu-id="e0cf3-111">Property</span></span>     | <span data-ttu-id="e0cf3-112">类型</span><span class="sxs-lookup"><span data-stu-id="e0cf3-112">Type</span></span>   |<span data-ttu-id="e0cf3-113">说明</span><span class="sxs-lookup"><span data-stu-id="e0cf3-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e0cf3-114">actions</span><span class="sxs-lookup"><span data-stu-id="e0cf3-114">actions</span></span> | [<span data-ttu-id="e0cf3-115">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="e0cf3-115">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="e0cf3-116">满足相应条件时对邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-116">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="e0cf3-117">conditions</span><span class="sxs-lookup"><span data-stu-id="e0cf3-117">conditions</span></span> | [<span data-ttu-id="e0cf3-118">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="e0cf3-118">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="e0cf3-119">满足条件时，将触发该规则的相应操作。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-119">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="e0cf3-120">displayName</span><span class="sxs-lookup"><span data-stu-id="e0cf3-120">displayName</span></span> | <span data-ttu-id="e0cf3-121">String</span><span class="sxs-lookup"><span data-stu-id="e0cf3-121">String</span></span> | <span data-ttu-id="e0cf3-122">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-122">The display name of the rule.</span></span> |
| <span data-ttu-id="e0cf3-123">exceptions</span><span class="sxs-lookup"><span data-stu-id="e0cf3-123">exceptions</span></span> | [<span data-ttu-id="e0cf3-124">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="e0cf3-124">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="e0cf3-125">规则的例外情况。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-125">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="e0cf3-126">hasError</span><span class="sxs-lookup"><span data-stu-id="e0cf3-126">hasError</span></span> | <span data-ttu-id="e0cf3-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0cf3-127">Boolean</span></span> | <span data-ttu-id="e0cf3-128">指示规则是否处于错误状态。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-128">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="e0cf3-129">只读。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-129">Read-only.</span></span> |
| <span data-ttu-id="e0cf3-130">id</span><span class="sxs-lookup"><span data-stu-id="e0cf3-130">id</span></span> |<span data-ttu-id="e0cf3-131">String</span><span class="sxs-lookup"><span data-stu-id="e0cf3-131">String</span></span>|<span data-ttu-id="e0cf3-132">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-132">The unique identifier of the rule.</span></span> <span data-ttu-id="e0cf3-133">只读。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-133">Read-only.</span></span>|
| <span data-ttu-id="e0cf3-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e0cf3-134">isEnabled</span></span> | <span data-ttu-id="e0cf3-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0cf3-135">Boolean</span></span> | <span data-ttu-id="e0cf3-136">指示是否启用规则以应用到邮件。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-136">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="e0cf3-137">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="e0cf3-137">isReadOnly</span></span> | <span data-ttu-id="e0cf3-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0cf3-138">Boolean</span></span> | <span data-ttu-id="e0cf3-139">表示规则是否为只读且无法由规则 REST API 修改或删除。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-139">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="e0cf3-140">Sequence</span><span class="sxs-lookup"><span data-stu-id="e0cf3-140">sequence</span></span> | <span data-ttu-id="e0cf3-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e0cf3-141">Int32</span></span> | <span data-ttu-id="e0cf3-142">表示在其他规则中执行规则的顺序。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-142">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="e0cf3-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0cf3-143">JSON representation</span></span>
<span data-ttu-id="e0cf3-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-144">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="e0cf3-145">方法</span><span class="sxs-lookup"><span data-stu-id="e0cf3-145">Methods</span></span>
| <span data-ttu-id="e0cf3-146">方法</span><span class="sxs-lookup"><span data-stu-id="e0cf3-146">Method</span></span>           | <span data-ttu-id="e0cf3-147">返回类型</span><span class="sxs-lookup"><span data-stu-id="e0cf3-147">Return Type</span></span>    |<span data-ttu-id="e0cf3-148">说明</span><span class="sxs-lookup"><span data-stu-id="e0cf3-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e0cf3-149">List rules</span><span class="sxs-lookup"><span data-stu-id="e0cf3-149">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="e0cf3-150">[messageRule](messagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0cf3-150">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="e0cf3-151">获取为用户收件箱定义的所有 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-151">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="e0cf3-152">Get rule</span><span class="sxs-lookup"><span data-stu-id="e0cf3-152">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="e0cf3-153">messageRule</span><span class="sxs-lookup"><span data-stu-id="e0cf3-153">messageRule</span></span>](messagerule.md) |<span data-ttu-id="e0cf3-154">读取 **messageRule** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-154">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="e0cf3-155">Create</span><span class="sxs-lookup"><span data-stu-id="e0cf3-155">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="e0cf3-156">messageRule</span><span class="sxs-lookup"><span data-stu-id="e0cf3-156">messageRule</span></span>](messagerule.md) |<span data-ttu-id="e0cf3-157">通过指定一组条件和操作来创建 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-157">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="e0cf3-158">Update</span><span class="sxs-lookup"><span data-stu-id="e0cf3-158">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="e0cf3-159">messageRule</span><span class="sxs-lookup"><span data-stu-id="e0cf3-159">messageRule</span></span>](messagerule.md) |<span data-ttu-id="e0cf3-160">为 **messageRule** 对象更改可写属性并保存更改。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-160">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="e0cf3-161">Delete</span><span class="sxs-lookup"><span data-stu-id="e0cf3-161">Delete</span></span>](../api/messagerule-delete.md) | <span data-ttu-id="e0cf3-162">无</span><span class="sxs-lookup"><span data-stu-id="e0cf3-162">None</span></span> |<span data-ttu-id="e0cf3-163">删除指定的 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="e0cf3-163">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->