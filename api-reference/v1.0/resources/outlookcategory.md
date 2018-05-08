# <a name="outlookcategory-resource-type"></a><span data-ttu-id="1427d-101">outlookCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="1427d-101">outlookCategory resource type</span></span>


<span data-ttu-id="1427d-102">表示用户可以对 Outlook 项目（如邮件和事件）进行分组的类别依据。</span><span class="sxs-lookup"><span data-stu-id="1427d-102">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="1427d-103">用户在主列表中定义类别，并且可以将这些用户定义的一个或多个类别应用到项目中。</span><span class="sxs-lookup"><span data-stu-id="1427d-103">The user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="1427d-104">使用 REST API，可以在用户类别的主列表中[创建](../api/outlookuser_post_mastercategories.md)和定义类别。</span><span class="sxs-lookup"><span data-stu-id="1427d-104">Using the REST API, you can [create](../api/outlookuser_post_mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="1427d-105">还可以[获取主类别列表](../api/outlookuser_list_mastercategories.md)、[获取特定类别](../api/outlookcategory_get.md)、[更新](../api/outlookcategory_update.md)与类别相关联的颜色，或[删除](../api/outlookcategory_delete.md)类别。</span><span class="sxs-lookup"><span data-stu-id="1427d-105">You can also [get this master list of categories](../api/outlookuser_list_mastercategories.md), [get a specific category](../api/outlookcategory_get.md), [update](../api/outlookcategory_update.md) the color associated with a category, or [delete](../api/outlookcategory_delete.md) a category.</span></span> <span data-ttu-id="1427d-106">可以通过将类别的 **displayName** 属性分配给项目的 **categories** 集合，将类别应用到项目。</span><span class="sxs-lookup"><span data-stu-id="1427d-106">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="1427d-107">可以为资源分配以下类别：[联系人](contact.md)、[事件](event.md)、[邮件](message.md)和[帖子](post.md)。</span><span class="sxs-lookup"><span data-stu-id="1427d-107">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), and [post](post.md).</span></span>   

<span data-ttu-id="1427d-108">每个类别都有 2 个属性：**displayName** 和 **color**。</span><span class="sxs-lookup"><span data-stu-id="1427d-108">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="1427d-109">**displayName** 值在用户的主列表中必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="1427d-109">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="1427d-110">然而，**color** 不一定是唯一的；主列表中的多个类别可以映射到相同颜色。</span><span class="sxs-lookup"><span data-stu-id="1427d-110">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="1427d-111">可以在用户的主列表中将多达 25 种不同的颜色映射到类别。</span><span class="sxs-lookup"><span data-stu-id="1427d-111">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="1427d-112">属性</span><span class="sxs-lookup"><span data-stu-id="1427d-112">Properties</span></span>
| <span data-ttu-id="1427d-113">属性</span><span class="sxs-lookup"><span data-stu-id="1427d-113">Property</span></span>     | <span data-ttu-id="1427d-114">类型</span><span class="sxs-lookup"><span data-stu-id="1427d-114">Type</span></span>   |<span data-ttu-id="1427d-115">说明</span><span class="sxs-lookup"><span data-stu-id="1427d-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1427d-116">displayName</span><span class="sxs-lookup"><span data-stu-id="1427d-116">displayName</span></span>|<span data-ttu-id="1427d-117">String</span><span class="sxs-lookup"><span data-stu-id="1427d-117">String</span></span>|<span data-ttu-id="1427d-118">标识用户邮箱中的类别的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="1427d-118">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="1427d-119">在创建类别后，名称将无法更改。</span><span class="sxs-lookup"><span data-stu-id="1427d-119">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="1427d-120">只读。</span><span class="sxs-lookup"><span data-stu-id="1427d-120">Read-only.</span></span>|
|<span data-ttu-id="1427d-121">color</span><span class="sxs-lookup"><span data-stu-id="1427d-121">color</span></span>|<span data-ttu-id="1427d-122">String</span><span class="sxs-lookup"><span data-stu-id="1427d-122">String</span></span>|<span data-ttu-id="1427d-123">预先设定的颜色常数，它表示类别的特征，并映射到 25 种预定义颜色中的一种。</span><span class="sxs-lookup"><span data-stu-id="1427d-123">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="1427d-124">请参阅下面的备注。</span><span class="sxs-lookup"><span data-stu-id="1427d-124">See the note below.</span></span> |

> <span data-ttu-id="1427d-125">**注意**：**color** 的可能值为预设的常数，如 `None`、`preset0` 和 `preset1`。</span><span class="sxs-lookup"><span data-stu-id="1427d-125">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="1427d-126">每个预设定的常数会被进一步映射到一种颜色；实际颜色取决于显示类别的 Outlook 客户端。</span><span class="sxs-lookup"><span data-stu-id="1427d-126">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="1427d-127">下表显示了 Outlook（桌面客户端）中映射到每个预设常数的颜色。</span><span class="sxs-lookup"><span data-stu-id="1427d-127">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 


| <span data-ttu-id="1427d-128">预设常数</span><span class="sxs-lookup"><span data-stu-id="1427d-128">Pre-set constant</span></span>  | <span data-ttu-id="1427d-129">Outlook 中映射的颜色</span><span class="sxs-lookup"><span data-stu-id="1427d-129">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1427d-130">None</span><span class="sxs-lookup"><span data-stu-id="1427d-130">None</span></span> | <span data-ttu-id="1427d-131">没有映射的颜色</span><span class="sxs-lookup"><span data-stu-id="1427d-131">No color mapped</span></span> |
| <span data-ttu-id="1427d-132">Preset0</span><span class="sxs-lookup"><span data-stu-id="1427d-132">Preset0</span></span> | <span data-ttu-id="1427d-133">红色</span><span class="sxs-lookup"><span data-stu-id="1427d-133">Red</span></span> |
| <span data-ttu-id="1427d-134">Preset1</span><span class="sxs-lookup"><span data-stu-id="1427d-134">Preset1</span></span> | <span data-ttu-id="1427d-135">橙色</span><span class="sxs-lookup"><span data-stu-id="1427d-135">Orange</span></span> |
| <span data-ttu-id="1427d-136">Preset2</span><span class="sxs-lookup"><span data-stu-id="1427d-136">Preset2</span></span> | <span data-ttu-id="1427d-137">褐色</span><span class="sxs-lookup"><span data-stu-id="1427d-137">Brown</span></span> |
| <span data-ttu-id="1427d-138">Preset3</span><span class="sxs-lookup"><span data-stu-id="1427d-138">Preset3</span></span> | <span data-ttu-id="1427d-139">黄色</span><span class="sxs-lookup"><span data-stu-id="1427d-139">Yellow</span></span> |
| <span data-ttu-id="1427d-140">Preset4</span><span class="sxs-lookup"><span data-stu-id="1427d-140">Preset4</span></span> | <span data-ttu-id="1427d-141">绿色</span><span class="sxs-lookup"><span data-stu-id="1427d-141">Green</span></span> |
| <span data-ttu-id="1427d-142">Preset5</span><span class="sxs-lookup"><span data-stu-id="1427d-142">Preset5</span></span> | <span data-ttu-id="1427d-143">青色</span><span class="sxs-lookup"><span data-stu-id="1427d-143">Teal</span></span> |
| <span data-ttu-id="1427d-144">Preset6</span><span class="sxs-lookup"><span data-stu-id="1427d-144">Preset6</span></span> | <span data-ttu-id="1427d-145">橄榄绿</span><span class="sxs-lookup"><span data-stu-id="1427d-145">Olive</span></span> |
| <span data-ttu-id="1427d-146">Preset7</span><span class="sxs-lookup"><span data-stu-id="1427d-146">Preset7</span></span> | <span data-ttu-id="1427d-147">蓝色</span><span class="sxs-lookup"><span data-stu-id="1427d-147">Blue</span></span> |
| <span data-ttu-id="1427d-148">Preset8</span><span class="sxs-lookup"><span data-stu-id="1427d-148">Preset8</span></span> | <span data-ttu-id="1427d-149">紫色</span><span class="sxs-lookup"><span data-stu-id="1427d-149">Purple</span></span> |
| <span data-ttu-id="1427d-150">Preset9</span><span class="sxs-lookup"><span data-stu-id="1427d-150">Preset9</span></span> | <span data-ttu-id="1427d-151">蔓越橘色</span><span class="sxs-lookup"><span data-stu-id="1427d-151">Cranberry</span></span> |
| <span data-ttu-id="1427d-152">Preset10</span><span class="sxs-lookup"><span data-stu-id="1427d-152">Preset10</span></span> | <span data-ttu-id="1427d-153">青灰色</span><span class="sxs-lookup"><span data-stu-id="1427d-153">Steel</span></span> |
| <span data-ttu-id="1427d-154">Preset11</span><span class="sxs-lookup"><span data-stu-id="1427d-154">Preset11</span></span> | <span data-ttu-id="1427d-155">深青灰</span><span class="sxs-lookup"><span data-stu-id="1427d-155">DarkSteel</span></span> |
| <span data-ttu-id="1427d-156">Preset12</span><span class="sxs-lookup"><span data-stu-id="1427d-156">Preset12</span></span> | <span data-ttu-id="1427d-157">灰色</span><span class="sxs-lookup"><span data-stu-id="1427d-157">Gray</span></span> |
| <span data-ttu-id="1427d-158">Preset13</span><span class="sxs-lookup"><span data-stu-id="1427d-158">Preset13</span></span> | <span data-ttu-id="1427d-159">深灰</span><span class="sxs-lookup"><span data-stu-id="1427d-159">DarkGray</span></span> |
| <span data-ttu-id="1427d-160">Preset14</span><span class="sxs-lookup"><span data-stu-id="1427d-160">Preset14</span></span> | <span data-ttu-id="1427d-161">黑色</span><span class="sxs-lookup"><span data-stu-id="1427d-161">Black</span></span> |
| <span data-ttu-id="1427d-162">Preset15</span><span class="sxs-lookup"><span data-stu-id="1427d-162">Preset15</span></span> | <span data-ttu-id="1427d-163">深红</span><span class="sxs-lookup"><span data-stu-id="1427d-163">DarkRed</span></span> |
| <span data-ttu-id="1427d-164">Preset16</span><span class="sxs-lookup"><span data-stu-id="1427d-164">Preset16</span></span> | <span data-ttu-id="1427d-165">暗橙</span><span class="sxs-lookup"><span data-stu-id="1427d-165">DarkOrange</span></span> |
| <span data-ttu-id="1427d-166">Preset17</span><span class="sxs-lookup"><span data-stu-id="1427d-166">Preset17</span></span> | <span data-ttu-id="1427d-167">深褐</span><span class="sxs-lookup"><span data-stu-id="1427d-167">DarkBrown</span></span> |
| <span data-ttu-id="1427d-168">Preset18</span><span class="sxs-lookup"><span data-stu-id="1427d-168">Preset18</span></span> | <span data-ttu-id="1427d-169">深黄</span><span class="sxs-lookup"><span data-stu-id="1427d-169">DarkYellow</span></span> |
| <span data-ttu-id="1427d-170">Preset19</span><span class="sxs-lookup"><span data-stu-id="1427d-170">Preset19</span></span> | <span data-ttu-id="1427d-171">深绿</span><span class="sxs-lookup"><span data-stu-id="1427d-171">DarkGreen</span></span> |
| <span data-ttu-id="1427d-172">Preset20</span><span class="sxs-lookup"><span data-stu-id="1427d-172">Preset20</span></span> | <span data-ttu-id="1427d-173">深青</span><span class="sxs-lookup"><span data-stu-id="1427d-173">DarkTeal</span></span> |
| <span data-ttu-id="1427d-174">Preset21</span><span class="sxs-lookup"><span data-stu-id="1427d-174">Preset21</span></span> | <span data-ttu-id="1427d-175">深橄榄色</span><span class="sxs-lookup"><span data-stu-id="1427d-175">DarkOlive</span></span> |
| <span data-ttu-id="1427d-176">Preset22</span><span class="sxs-lookup"><span data-stu-id="1427d-176">Preset22</span></span> | <span data-ttu-id="1427d-177">深蓝</span><span class="sxs-lookup"><span data-stu-id="1427d-177">DarkBlue</span></span> |
| <span data-ttu-id="1427d-178">Preset23</span><span class="sxs-lookup"><span data-stu-id="1427d-178">Preset23</span></span> | <span data-ttu-id="1427d-179">深紫</span><span class="sxs-lookup"><span data-stu-id="1427d-179">DarkPurple</span></span> |
| <span data-ttu-id="1427d-180">Preset24</span><span class="sxs-lookup"><span data-stu-id="1427d-180">Preset24</span></span> | <span data-ttu-id="1427d-181">深蔓越橘色</span><span class="sxs-lookup"><span data-stu-id="1427d-181">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1427d-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1427d-182">JSON representation</span></span>
<span data-ttu-id="1427d-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1427d-183">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookCategory"
}-->

```json
{
  "color": "String",
  "displayName": "String"
}

```

## <a name="methods"></a><span data-ttu-id="1427d-184">方法</span><span class="sxs-lookup"><span data-stu-id="1427d-184">Methods</span></span>
| <span data-ttu-id="1427d-185">方法</span><span class="sxs-lookup"><span data-stu-id="1427d-185">Method</span></span>           | <span data-ttu-id="1427d-186">返回类型</span><span class="sxs-lookup"><span data-stu-id="1427d-186">Return Type</span></span>    |<span data-ttu-id="1427d-187">说明</span><span class="sxs-lookup"><span data-stu-id="1427d-187">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1427d-188">List categories</span><span class="sxs-lookup"><span data-stu-id="1427d-188">List categories</span></span>](../api/outlookuser_list_mastercategories.md) | <span data-ttu-id="1427d-189">[outlookCategory](../resources/outlookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1427d-189">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="1427d-190">获取为用户定义的所有类别。</span><span class="sxs-lookup"><span data-stu-id="1427d-190">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="1427d-191">Get category</span><span class="sxs-lookup"><span data-stu-id="1427d-191">Get category</span></span>](../api/outlookcategory_get.md) | [<span data-ttu-id="1427d-192">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="1427d-192">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="1427d-193">获取指定的 **outlookCategory** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1427d-193">Get the properties and relationships of the specified **event** object.</span></span>|
|[<span data-ttu-id="1427d-194">Create</span><span class="sxs-lookup"><span data-stu-id="1427d-194">Create</span></span>](../api/outlookuser_post_mastercategories.md) | [<span data-ttu-id="1427d-195">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="1427d-195">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="1427d-196">在用户主类别列表中创建 **outlookCategory** 对象。</span><span class="sxs-lookup"><span data-stu-id="1427d-196">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="1427d-197">Update</span><span class="sxs-lookup"><span data-stu-id="1427d-197">Update</span></span>](../api/outlookcategory_update.md) | [<span data-ttu-id="1427d-198">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="1427d-198">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="1427d-199">更新指定 **outlookCategory** 对象的可写属性 **color**。</span><span class="sxs-lookup"><span data-stu-id="1427d-199">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="1427d-200">Delete</span><span class="sxs-lookup"><span data-stu-id="1427d-200">Delete</span></span>](../api/outlookcategory_delete.md) | <span data-ttu-id="1427d-201">None</span><span class="sxs-lookup"><span data-stu-id="1427d-201">None</span></span> |<span data-ttu-id="1427d-202">删除指定的 **outlookCategory** 对象。</span><span class="sxs-lookup"><span data-stu-id="1427d-202">Delete the specified **outlookCategory** object.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
 