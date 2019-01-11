---
title: outlookCategory 资源类型
description: 表示用户可以对 Outlook 项目（如邮件和事件）进行分组的类别依据。 在 Outlook 中，用户定义类别中的主控形状的列表，并可以将一个或多个这些用户定义的应用
localization_priority: Normal
ms.openlocfilehash: b9c1a3a1813195a36dd1f1cf587cf69d2ddb5f1b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816756"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="0ee76-104">outlookCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ee76-104">outlookCategory resource type</span></span>

> <span data-ttu-id="0ee76-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0ee76-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0ee76-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0ee76-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ee76-107">表示用户可以对 Outlook 项目（如邮件和事件）进行分组的类别依据。</span><span class="sxs-lookup"><span data-stu-id="0ee76-107">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="0ee76-108">在 Outlook 中，用户定义类别中的主控形状的列表，并可以将一个或多个这些用户定义的类别应用于项目。</span><span class="sxs-lookup"><span data-stu-id="0ee76-108">In Outlook, the user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="0ee76-109">使用 REST API，可以在用户类别的主列表中[创建](../api/outlookuser-post-mastercategories.md)和定义类别。</span><span class="sxs-lookup"><span data-stu-id="0ee76-109">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="0ee76-110">还可以[获取主类别列表](../api/outlookuser-list-mastercategories.md)、[获取特定类别](../api/outlookcategory-get.md)、[更新](../api/outlookcategory-update.md)与类别相关联的颜色，或[删除](../api/outlookcategory-delete.md)类别。</span><span class="sxs-lookup"><span data-stu-id="0ee76-110">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="0ee76-111">可以通过将类别的 **displayName** 属性分配给项目的 **categories** 集合，将类别应用到项目。</span><span class="sxs-lookup"><span data-stu-id="0ee76-111">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="0ee76-112">资源可分配类别包括[联系人](contact.md)、[事件](event.md)、[消息](message.md)、 [outlookTask](outlooktask.md)，和[文章](post.md)。</span><span class="sxs-lookup"><span data-stu-id="0ee76-112">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), [outlookTask](outlooktask.md), and [post](post.md).</span></span>   

<span data-ttu-id="0ee76-113">每个类别都有 2 个属性：**displayName** 和 **color**。</span><span class="sxs-lookup"><span data-stu-id="0ee76-113">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="0ee76-114">**displayName** 值在用户的主列表中必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="0ee76-114">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="0ee76-115">然而，**color** 不一定是唯一的；主列表中的多个类别可以映射到相同颜色。</span><span class="sxs-lookup"><span data-stu-id="0ee76-115">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="0ee76-116">可以在用户的主列表中将多达 25 种不同的颜色映射到类别。</span><span class="sxs-lookup"><span data-stu-id="0ee76-116">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="0ee76-117">属性</span><span class="sxs-lookup"><span data-stu-id="0ee76-117">Properties</span></span>
| <span data-ttu-id="0ee76-118">属性</span><span class="sxs-lookup"><span data-stu-id="0ee76-118">Property</span></span>     | <span data-ttu-id="0ee76-119">类型</span><span class="sxs-lookup"><span data-stu-id="0ee76-119">Type</span></span>   |<span data-ttu-id="0ee76-120">说明</span><span class="sxs-lookup"><span data-stu-id="0ee76-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ee76-121">displayName</span><span class="sxs-lookup"><span data-stu-id="0ee76-121">displayName</span></span>|<span data-ttu-id="0ee76-122">String</span><span class="sxs-lookup"><span data-stu-id="0ee76-122">String</span></span>|<span data-ttu-id="0ee76-123">标识用户邮箱中的类别的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="0ee76-123">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="0ee76-124">在创建类别后，名称将无法更改。</span><span class="sxs-lookup"><span data-stu-id="0ee76-124">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="0ee76-125">只读。</span><span class="sxs-lookup"><span data-stu-id="0ee76-125">Read-only.</span></span>|
|<span data-ttu-id="0ee76-126">color</span><span class="sxs-lookup"><span data-stu-id="0ee76-126">color</span></span>|<span data-ttu-id="0ee76-127">String</span><span class="sxs-lookup"><span data-stu-id="0ee76-127">String</span></span>|<span data-ttu-id="0ee76-128">预先设定的颜色常数，它表示类别的特征，并映射到 25 种预定义颜色中的一种。</span><span class="sxs-lookup"><span data-stu-id="0ee76-128">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="0ee76-129">请参阅下面的备注。</span><span class="sxs-lookup"><span data-stu-id="0ee76-129">See the note below.</span></span> |

> <span data-ttu-id="0ee76-130">**注意**：**color** 的可能值为预设的常数，如 `None`、`preset0` 和 `preset1`。</span><span class="sxs-lookup"><span data-stu-id="0ee76-130">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="0ee76-131">每个预设定的常数会被进一步映射到一种颜色；实际颜色取决于显示类别的 Outlook 客户端。</span><span class="sxs-lookup"><span data-stu-id="0ee76-131">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="0ee76-132">下表显示了 Outlook（桌面客户端）中映射到每个预设常数的颜色。</span><span class="sxs-lookup"><span data-stu-id="0ee76-132">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 


| <span data-ttu-id="0ee76-133">预设常数</span><span class="sxs-lookup"><span data-stu-id="0ee76-133">Pre-set constant</span></span>  | <span data-ttu-id="0ee76-134">Outlook 中映射的颜色</span><span class="sxs-lookup"><span data-stu-id="0ee76-134">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0ee76-135">None</span><span class="sxs-lookup"><span data-stu-id="0ee76-135">None</span></span> | <span data-ttu-id="0ee76-136">没有映射的颜色</span><span class="sxs-lookup"><span data-stu-id="0ee76-136">No color mapped</span></span> |
| <span data-ttu-id="0ee76-137">Preset0</span><span class="sxs-lookup"><span data-stu-id="0ee76-137">Preset0</span></span> | <span data-ttu-id="0ee76-138">红色</span><span class="sxs-lookup"><span data-stu-id="0ee76-138">Red</span></span> |
| <span data-ttu-id="0ee76-139">Preset1</span><span class="sxs-lookup"><span data-stu-id="0ee76-139">Preset1</span></span> | <span data-ttu-id="0ee76-140">橙色</span><span class="sxs-lookup"><span data-stu-id="0ee76-140">Orange</span></span> |
| <span data-ttu-id="0ee76-141">Preset2</span><span class="sxs-lookup"><span data-stu-id="0ee76-141">Preset2</span></span> | <span data-ttu-id="0ee76-142">褐色</span><span class="sxs-lookup"><span data-stu-id="0ee76-142">Brown</span></span> |
| <span data-ttu-id="0ee76-143">Preset3</span><span class="sxs-lookup"><span data-stu-id="0ee76-143">Preset3</span></span> | <span data-ttu-id="0ee76-144">黄色</span><span class="sxs-lookup"><span data-stu-id="0ee76-144">Yellow</span></span> |
| <span data-ttu-id="0ee76-145">Preset4</span><span class="sxs-lookup"><span data-stu-id="0ee76-145">Preset4</span></span> | <span data-ttu-id="0ee76-146">绿色</span><span class="sxs-lookup"><span data-stu-id="0ee76-146">Green</span></span> |
| <span data-ttu-id="0ee76-147">Preset5</span><span class="sxs-lookup"><span data-stu-id="0ee76-147">Preset5</span></span> | <span data-ttu-id="0ee76-148">青色</span><span class="sxs-lookup"><span data-stu-id="0ee76-148">Teal</span></span> |
| <span data-ttu-id="0ee76-149">Preset6</span><span class="sxs-lookup"><span data-stu-id="0ee76-149">Preset6</span></span> | <span data-ttu-id="0ee76-150">橄榄绿</span><span class="sxs-lookup"><span data-stu-id="0ee76-150">Olive</span></span> |
| <span data-ttu-id="0ee76-151">Preset7</span><span class="sxs-lookup"><span data-stu-id="0ee76-151">Preset7</span></span> | <span data-ttu-id="0ee76-152">蓝色</span><span class="sxs-lookup"><span data-stu-id="0ee76-152">Blue</span></span> |
| <span data-ttu-id="0ee76-153">Preset8</span><span class="sxs-lookup"><span data-stu-id="0ee76-153">Preset8</span></span> | <span data-ttu-id="0ee76-154">紫色</span><span class="sxs-lookup"><span data-stu-id="0ee76-154">Purple</span></span> |
| <span data-ttu-id="0ee76-155">Preset9</span><span class="sxs-lookup"><span data-stu-id="0ee76-155">Preset9</span></span> | <span data-ttu-id="0ee76-156">蔓越橘色</span><span class="sxs-lookup"><span data-stu-id="0ee76-156">Cranberry</span></span> |
| <span data-ttu-id="0ee76-157">Preset10</span><span class="sxs-lookup"><span data-stu-id="0ee76-157">Preset10</span></span> | <span data-ttu-id="0ee76-158">青灰色</span><span class="sxs-lookup"><span data-stu-id="0ee76-158">Steel</span></span> |
| <span data-ttu-id="0ee76-159">Preset11</span><span class="sxs-lookup"><span data-stu-id="0ee76-159">Preset11</span></span> | <span data-ttu-id="0ee76-160">深青灰</span><span class="sxs-lookup"><span data-stu-id="0ee76-160">DarkSteel</span></span> |
| <span data-ttu-id="0ee76-161">Preset12</span><span class="sxs-lookup"><span data-stu-id="0ee76-161">Preset12</span></span> | <span data-ttu-id="0ee76-162">灰色</span><span class="sxs-lookup"><span data-stu-id="0ee76-162">Gray</span></span> |
| <span data-ttu-id="0ee76-163">Preset13</span><span class="sxs-lookup"><span data-stu-id="0ee76-163">Preset13</span></span> | <span data-ttu-id="0ee76-164">深灰</span><span class="sxs-lookup"><span data-stu-id="0ee76-164">DarkGray</span></span> |
| <span data-ttu-id="0ee76-165">Preset14</span><span class="sxs-lookup"><span data-stu-id="0ee76-165">Preset14</span></span> | <span data-ttu-id="0ee76-166">黑色</span><span class="sxs-lookup"><span data-stu-id="0ee76-166">Black</span></span> |
| <span data-ttu-id="0ee76-167">Preset15</span><span class="sxs-lookup"><span data-stu-id="0ee76-167">Preset15</span></span> | <span data-ttu-id="0ee76-168">深红</span><span class="sxs-lookup"><span data-stu-id="0ee76-168">DarkRed</span></span> |
| <span data-ttu-id="0ee76-169">Preset16</span><span class="sxs-lookup"><span data-stu-id="0ee76-169">Preset16</span></span> | <span data-ttu-id="0ee76-170">暗橙</span><span class="sxs-lookup"><span data-stu-id="0ee76-170">DarkOrange</span></span> |
| <span data-ttu-id="0ee76-171">Preset17</span><span class="sxs-lookup"><span data-stu-id="0ee76-171">Preset17</span></span> | <span data-ttu-id="0ee76-172">深褐</span><span class="sxs-lookup"><span data-stu-id="0ee76-172">DarkBrown</span></span> |
| <span data-ttu-id="0ee76-173">Preset18</span><span class="sxs-lookup"><span data-stu-id="0ee76-173">Preset18</span></span> | <span data-ttu-id="0ee76-174">深黄</span><span class="sxs-lookup"><span data-stu-id="0ee76-174">DarkYellow</span></span> |
| <span data-ttu-id="0ee76-175">Preset19</span><span class="sxs-lookup"><span data-stu-id="0ee76-175">Preset19</span></span> | <span data-ttu-id="0ee76-176">深绿</span><span class="sxs-lookup"><span data-stu-id="0ee76-176">DarkGreen</span></span> |
| <span data-ttu-id="0ee76-177">Preset20</span><span class="sxs-lookup"><span data-stu-id="0ee76-177">Preset20</span></span> | <span data-ttu-id="0ee76-178">深青</span><span class="sxs-lookup"><span data-stu-id="0ee76-178">DarkTeal</span></span> |
| <span data-ttu-id="0ee76-179">Preset21</span><span class="sxs-lookup"><span data-stu-id="0ee76-179">Preset21</span></span> | <span data-ttu-id="0ee76-180">深橄榄色</span><span class="sxs-lookup"><span data-stu-id="0ee76-180">DarkOlive</span></span> |
| <span data-ttu-id="0ee76-181">Preset22</span><span class="sxs-lookup"><span data-stu-id="0ee76-181">Preset22</span></span> | <span data-ttu-id="0ee76-182">深蓝</span><span class="sxs-lookup"><span data-stu-id="0ee76-182">DarkBlue</span></span> |
| <span data-ttu-id="0ee76-183">Preset23</span><span class="sxs-lookup"><span data-stu-id="0ee76-183">Preset23</span></span> | <span data-ttu-id="0ee76-184">深紫</span><span class="sxs-lookup"><span data-stu-id="0ee76-184">DarkPurple</span></span> |
| <span data-ttu-id="0ee76-185">Preset24</span><span class="sxs-lookup"><span data-stu-id="0ee76-185">Preset24</span></span> | <span data-ttu-id="0ee76-186">深蔓越橘色</span><span class="sxs-lookup"><span data-stu-id="0ee76-186">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0ee76-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ee76-187">JSON representation</span></span>
<span data-ttu-id="0ee76-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ee76-188">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="0ee76-189">方法</span><span class="sxs-lookup"><span data-stu-id="0ee76-189">Methods</span></span>
| <span data-ttu-id="0ee76-190">方法</span><span class="sxs-lookup"><span data-stu-id="0ee76-190">Method</span></span>           | <span data-ttu-id="0ee76-191">返回类型</span><span class="sxs-lookup"><span data-stu-id="0ee76-191">Return Type</span></span>    |<span data-ttu-id="0ee76-192">说明</span><span class="sxs-lookup"><span data-stu-id="0ee76-192">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0ee76-193">List categories</span><span class="sxs-lookup"><span data-stu-id="0ee76-193">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="0ee76-194">[outlookCategory](../resources/outlookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ee76-194">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="0ee76-195">获取为用户定义的所有类别。</span><span class="sxs-lookup"><span data-stu-id="0ee76-195">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="0ee76-196">Get category</span><span class="sxs-lookup"><span data-stu-id="0ee76-196">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="0ee76-197">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="0ee76-197">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="0ee76-198">获取指定的 **outlookCategory** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0ee76-198">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="0ee76-199">Create</span><span class="sxs-lookup"><span data-stu-id="0ee76-199">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="0ee76-200">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="0ee76-200">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="0ee76-201">在用户主类别列表中创建 **outlookCategory** 对象。</span><span class="sxs-lookup"><span data-stu-id="0ee76-201">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="0ee76-202">Update</span><span class="sxs-lookup"><span data-stu-id="0ee76-202">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="0ee76-203">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="0ee76-203">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="0ee76-204">更新指定 **outlookCategory** 对象的可写属性 **color**。</span><span class="sxs-lookup"><span data-stu-id="0ee76-204">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="0ee76-205">Delete</span><span class="sxs-lookup"><span data-stu-id="0ee76-205">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="0ee76-206">None</span><span class="sxs-lookup"><span data-stu-id="0ee76-206">None</span></span> |<span data-ttu-id="0ee76-207">删除指定的 **outlookCategory** 对象。</span><span class="sxs-lookup"><span data-stu-id="0ee76-207">Delete the specified **outlookCategory** object.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/beta/resources/outlookcategory.md:
      Failed to parse any rows out of table with headers: |Pre-set constant|Color mapped to in Outlook|"
  ],
  "tocPath": ""
}-->
 
