# <a name="messagerule-resource-type"></a><span data-ttu-id="0b6a7-101">messageRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b6a7-101">messageRule resource type</span></span>


<span data-ttu-id="0b6a7-102">适用于用户收件箱邮件的规则。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-102">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="0b6a7-103">在 Outlook 中，可以为收件箱中的传入邮件设置规则，以便在特定条件下执行具体操作。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-103">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="0b6a7-104">可以按编程方式通过收件箱[文件夹](mailfolder.md)的 **messageRules** 导航属性来访问规则。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-104">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="0b6a7-105">每个规则都由此 **messageRule** 资源表示，可用的规则操作由 [messageRuleActions](messageruleactions.md) 复杂类型表示，而可用的规则条件和例外则通过 [messageRulePredicates](messagerulepredicates.md) 复杂类型表示。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-105">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="0b6a7-106">属性</span><span class="sxs-lookup"><span data-stu-id="0b6a7-106">Properties</span></span>
| <span data-ttu-id="0b6a7-107">属性</span><span class="sxs-lookup"><span data-stu-id="0b6a7-107">Property</span></span>     | <span data-ttu-id="0b6a7-108">类型</span><span class="sxs-lookup"><span data-stu-id="0b6a7-108">Type</span></span>   |<span data-ttu-id="0b6a7-109">说明</span><span class="sxs-lookup"><span data-stu-id="0b6a7-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0b6a7-110">actions</span><span class="sxs-lookup"><span data-stu-id="0b6a7-110">Actions</span></span> | [<span data-ttu-id="0b6a7-111">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="0b6a7-111">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="0b6a7-112">满足相应条件时对邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-112">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="0b6a7-113">conditions</span><span class="sxs-lookup"><span data-stu-id="0b6a7-113">Conditions</span></span> | [<span data-ttu-id="0b6a7-114">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="0b6a7-114">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="0b6a7-115">满足条件时，将触发该规则的相应操作。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-115">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="0b6a7-116">displayName</span><span class="sxs-lookup"><span data-stu-id="0b6a7-116">displayName</span></span> | <span data-ttu-id="0b6a7-117">String</span><span class="sxs-lookup"><span data-stu-id="0b6a7-117">String</span></span> | <span data-ttu-id="0b6a7-118">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-118">The name of the new formatting rule.</span></span> |
| <span data-ttu-id="0b6a7-119">exceptions</span><span class="sxs-lookup"><span data-stu-id="0b6a7-119">exceptions</span></span> | [<span data-ttu-id="0b6a7-120">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="0b6a7-120">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="0b6a7-121">规则的例外情况。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-121">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="0b6a7-122">hasError</span><span class="sxs-lookup"><span data-stu-id="0b6a7-122">hasError</span></span> | <span data-ttu-id="0b6a7-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6a7-123">Boolean</span></span> | <span data-ttu-id="0b6a7-124">指示规则是否处于错误状态。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-124">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="0b6a7-125">只读。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-125">Read-only.</span></span> |
| <span data-ttu-id="0b6a7-126">id</span><span class="sxs-lookup"><span data-stu-id="0b6a7-126">id</span></span> |<span data-ttu-id="0b6a7-127">String</span><span class="sxs-lookup"><span data-stu-id="0b6a7-127">String</span></span>|<span data-ttu-id="0b6a7-128">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-128">The unique identifier of the rule.</span></span> <span data-ttu-id="0b6a7-129">只读。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-129">Read-only.</span></span>|
| <span data-ttu-id="0b6a7-130">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0b6a7-130">isEnabled</span></span> | <span data-ttu-id="0b6a7-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6a7-131">Boolean</span></span> | <span data-ttu-id="0b6a7-132">指示是否启用规则以应用到邮件。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-132">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="0b6a7-133">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="0b6a7-133">IsReadOnly</span></span> | <span data-ttu-id="0b6a7-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b6a7-134">Boolean</span></span> | <span data-ttu-id="0b6a7-135">表示规则是否为只读且无法由规则 REST API 修改或删除。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-135">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="0b6a7-136">Sequence</span><span class="sxs-lookup"><span data-stu-id="0b6a7-136">Sequence</span></span> | <span data-ttu-id="0b6a7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0b6a7-137">Int32</span></span> | <span data-ttu-id="0b6a7-138">表示在其他规则中执行规则的顺序。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-138">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="0b6a7-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b6a7-139">JSON representation</span></span>
<span data-ttu-id="0b6a7-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-140">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="0b6a7-141">方法</span><span class="sxs-lookup"><span data-stu-id="0b6a7-141">Methods</span></span>
| <span data-ttu-id="0b6a7-142">方法</span><span class="sxs-lookup"><span data-stu-id="0b6a7-142">Method</span></span>           | <span data-ttu-id="0b6a7-143">返回类型</span><span class="sxs-lookup"><span data-stu-id="0b6a7-143">Return Type</span></span>    |<span data-ttu-id="0b6a7-144">说明</span><span class="sxs-lookup"><span data-stu-id="0b6a7-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0b6a7-145">List rules</span><span class="sxs-lookup"><span data-stu-id="0b6a7-145">List rules</span></span>](../api/mailfolder_list_messagerules.md) | <span data-ttu-id="0b6a7-146">[messageRule](messagerule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0b6a7-146">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="0b6a7-147">获取为用户收件箱定义的所有 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-147">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="0b6a7-148">Get rule</span><span class="sxs-lookup"><span data-stu-id="0b6a7-148">Get rule</span></span>](../api/messagerule_get.md) | [<span data-ttu-id="0b6a7-149">messageRule</span><span class="sxs-lookup"><span data-stu-id="0b6a7-149">messageRule</span></span>](messagerule.md) |<span data-ttu-id="0b6a7-150">读取 **messageRule** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-150">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="0b6a7-151">Create</span><span class="sxs-lookup"><span data-stu-id="0b6a7-151">Create</span></span>](../api/mailfolder_post_messagerules.md) | [<span data-ttu-id="0b6a7-152">messageRule</span><span class="sxs-lookup"><span data-stu-id="0b6a7-152">messageRule</span></span>](messagerule.md) |<span data-ttu-id="0b6a7-153">通过指定一组条件和操作来创建 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-153">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="0b6a7-154">Update</span><span class="sxs-lookup"><span data-stu-id="0b6a7-154">Update</span></span>](../api/messagerule_update.md) | [<span data-ttu-id="0b6a7-155">messageRule</span><span class="sxs-lookup"><span data-stu-id="0b6a7-155">messageRule</span></span>](messagerule.md) |<span data-ttu-id="0b6a7-156">为 **messageRule** 对象更改可写属性并保存更改。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-156">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="0b6a7-157">Delete</span><span class="sxs-lookup"><span data-stu-id="0b6a7-157">Delete</span></span>](../api/messagerule_delete.md) | <span data-ttu-id="0b6a7-158">无</span><span class="sxs-lookup"><span data-stu-id="0b6a7-158">None</span></span> |<span data-ttu-id="0b6a7-159">删除指定的 **messageRule** 对象。</span><span class="sxs-lookup"><span data-stu-id="0b6a7-159">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->