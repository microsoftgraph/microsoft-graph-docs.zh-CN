---
title: outlookCategory 资源类型
description: 表示用户可以对 Outlook 项目（如邮件和事件）进行分组的类别依据。 用户定义类别中的主控形状的列表，并可以将一个或多个这些用户定义的应用
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 490ecaf2e6303cc943646dbed99b3202b8d57525
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953124"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="42392-104">outlookCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="42392-104">outlookCategory resource type</span></span>


<span data-ttu-id="42392-105">表示用户可以对 Outlook 项目（如邮件和事件）进行分组的类别依据。</span><span class="sxs-lookup"><span data-stu-id="42392-105">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="42392-106">用户在主列表中定义类别，并且可以将这些用户定义的一个或多个类别应用到项目中。</span><span class="sxs-lookup"><span data-stu-id="42392-106">The user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="42392-107">使用 REST API，可以在用户类别的主列表中[创建](../api/outlookuser-post-mastercategories.md)和定义类别。</span><span class="sxs-lookup"><span data-stu-id="42392-107">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="42392-108">还可以[获取主类别列表](../api/outlookuser-list-mastercategories.md)、[获取特定类别](../api/outlookcategory-get.md)、[更新](../api/outlookcategory-update.md)与类别相关联的颜色，或[删除](../api/outlookcategory-delete.md)类别。</span><span class="sxs-lookup"><span data-stu-id="42392-108">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="42392-109">可以通过将类别的 **displayName** 属性分配给项目的 **categories** 集合，将类别应用到项目。</span><span class="sxs-lookup"><span data-stu-id="42392-109">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="42392-110">可以为资源分配以下类别：[联系人](contact.md)、[事件](event.md)、[邮件](message.md)和[帖子](post.md)。</span><span class="sxs-lookup"><span data-stu-id="42392-110">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), and [post](post.md).</span></span>   

<span data-ttu-id="42392-111">每个类别都有 2 个属性：**displayName** 和 **color**。</span><span class="sxs-lookup"><span data-stu-id="42392-111">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="42392-112">**displayName** 值在用户的主列表中必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="42392-112">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="42392-113">然而，**color** 不一定是唯一的；主列表中的多个类别可以映射到相同颜色。</span><span class="sxs-lookup"><span data-stu-id="42392-113">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="42392-114">可以在用户的主列表中将多达 25 种不同的颜色映射到类别。</span><span class="sxs-lookup"><span data-stu-id="42392-114">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="42392-115">属性</span><span class="sxs-lookup"><span data-stu-id="42392-115">Properties</span></span>
| <span data-ttu-id="42392-116">属性</span><span class="sxs-lookup"><span data-stu-id="42392-116">Property</span></span>     | <span data-ttu-id="42392-117">类型</span><span class="sxs-lookup"><span data-stu-id="42392-117">Type</span></span>   |<span data-ttu-id="42392-118">说明</span><span class="sxs-lookup"><span data-stu-id="42392-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42392-119">displayName</span><span class="sxs-lookup"><span data-stu-id="42392-119">displayName</span></span>|<span data-ttu-id="42392-120">String</span><span class="sxs-lookup"><span data-stu-id="42392-120">String</span></span>|<span data-ttu-id="42392-121">标识用户邮箱中的类别的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="42392-121">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="42392-122">在创建类别后，名称将无法更改。</span><span class="sxs-lookup"><span data-stu-id="42392-122">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="42392-123">只读。</span><span class="sxs-lookup"><span data-stu-id="42392-123">Read-only.</span></span>|
|<span data-ttu-id="42392-124">color</span><span class="sxs-lookup"><span data-stu-id="42392-124">color</span></span>|<span data-ttu-id="42392-125">categoryColor</span><span class="sxs-lookup"><span data-stu-id="42392-125">categoryColor</span></span>|<span data-ttu-id="42392-126">预先设定的颜色常数，它表示类别的特征，并映射到 25 种预定义颜色中的一种。</span><span class="sxs-lookup"><span data-stu-id="42392-126">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="42392-127">请参阅下面的备注。</span><span class="sxs-lookup"><span data-stu-id="42392-127">See the note below.</span></span> |

> <span data-ttu-id="42392-128">**注意**：**color** 的可能值为预设的常数，如 `None`、`preset0` 和 `preset1`。</span><span class="sxs-lookup"><span data-stu-id="42392-128">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="42392-129">每个预设定的常数会被进一步映射到一种颜色；实际颜色取决于显示类别的 Outlook 客户端。</span><span class="sxs-lookup"><span data-stu-id="42392-129">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="42392-130">下表显示了 Outlook（桌面客户端）中映射到每个预设常数的颜色。</span><span class="sxs-lookup"><span data-stu-id="42392-130">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 

| <span data-ttu-id="42392-131">预设常数</span><span class="sxs-lookup"><span data-stu-id="42392-131">Pre-set constant</span></span>  | <span data-ttu-id="42392-132">Outlook 中映射的颜色</span><span class="sxs-lookup"><span data-stu-id="42392-132">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="42392-133">None</span><span class="sxs-lookup"><span data-stu-id="42392-133">None</span></span> | <span data-ttu-id="42392-134">没有映射的颜色</span><span class="sxs-lookup"><span data-stu-id="42392-134">No color mapped</span></span> |
| <span data-ttu-id="42392-135">Preset0</span><span class="sxs-lookup"><span data-stu-id="42392-135">Preset0</span></span> | <span data-ttu-id="42392-136">红色</span><span class="sxs-lookup"><span data-stu-id="42392-136">Red</span></span> |
| <span data-ttu-id="42392-137">Preset1</span><span class="sxs-lookup"><span data-stu-id="42392-137">Preset1</span></span> | <span data-ttu-id="42392-138">橙色</span><span class="sxs-lookup"><span data-stu-id="42392-138">Orange</span></span> |
| <span data-ttu-id="42392-139">Preset2</span><span class="sxs-lookup"><span data-stu-id="42392-139">Preset2</span></span> | <span data-ttu-id="42392-140">褐色</span><span class="sxs-lookup"><span data-stu-id="42392-140">Brown</span></span> |
| <span data-ttu-id="42392-141">Preset3</span><span class="sxs-lookup"><span data-stu-id="42392-141">Preset3</span></span> | <span data-ttu-id="42392-142">黄色</span><span class="sxs-lookup"><span data-stu-id="42392-142">Yellow</span></span> |
| <span data-ttu-id="42392-143">Preset4</span><span class="sxs-lookup"><span data-stu-id="42392-143">Preset4</span></span> | <span data-ttu-id="42392-144">绿色</span><span class="sxs-lookup"><span data-stu-id="42392-144">Green</span></span> |
| <span data-ttu-id="42392-145">Preset5</span><span class="sxs-lookup"><span data-stu-id="42392-145">Preset5</span></span> | <span data-ttu-id="42392-146">青色</span><span class="sxs-lookup"><span data-stu-id="42392-146">Teal</span></span> |
| <span data-ttu-id="42392-147">Preset6</span><span class="sxs-lookup"><span data-stu-id="42392-147">Preset6</span></span> | <span data-ttu-id="42392-148">橄榄绿</span><span class="sxs-lookup"><span data-stu-id="42392-148">Olive</span></span> |
| <span data-ttu-id="42392-149">Preset7</span><span class="sxs-lookup"><span data-stu-id="42392-149">Preset7</span></span> | <span data-ttu-id="42392-150">蓝色</span><span class="sxs-lookup"><span data-stu-id="42392-150">Blue</span></span> |
| <span data-ttu-id="42392-151">Preset8</span><span class="sxs-lookup"><span data-stu-id="42392-151">Preset8</span></span> | <span data-ttu-id="42392-152">紫色</span><span class="sxs-lookup"><span data-stu-id="42392-152">Purple</span></span> |
| <span data-ttu-id="42392-153">Preset9</span><span class="sxs-lookup"><span data-stu-id="42392-153">Preset9</span></span> | <span data-ttu-id="42392-154">蔓越橘色</span><span class="sxs-lookup"><span data-stu-id="42392-154">Cranberry</span></span> |
| <span data-ttu-id="42392-155">Preset10</span><span class="sxs-lookup"><span data-stu-id="42392-155">Preset10</span></span> | <span data-ttu-id="42392-156">青灰色</span><span class="sxs-lookup"><span data-stu-id="42392-156">Steel</span></span> |
| <span data-ttu-id="42392-157">Preset11</span><span class="sxs-lookup"><span data-stu-id="42392-157">Preset11</span></span> | <span data-ttu-id="42392-158">深青灰</span><span class="sxs-lookup"><span data-stu-id="42392-158">DarkSteel</span></span> |
| <span data-ttu-id="42392-159">Preset12</span><span class="sxs-lookup"><span data-stu-id="42392-159">Preset12</span></span> | <span data-ttu-id="42392-160">灰色</span><span class="sxs-lookup"><span data-stu-id="42392-160">Gray</span></span> |
| <span data-ttu-id="42392-161">Preset13</span><span class="sxs-lookup"><span data-stu-id="42392-161">Preset13</span></span> | <span data-ttu-id="42392-162">深灰</span><span class="sxs-lookup"><span data-stu-id="42392-162">DarkGray</span></span> |
| <span data-ttu-id="42392-163">Preset14</span><span class="sxs-lookup"><span data-stu-id="42392-163">Preset14</span></span> | <span data-ttu-id="42392-164">黑色</span><span class="sxs-lookup"><span data-stu-id="42392-164">Black</span></span> |
| <span data-ttu-id="42392-165">Preset15</span><span class="sxs-lookup"><span data-stu-id="42392-165">Preset15</span></span> | <span data-ttu-id="42392-166">深红</span><span class="sxs-lookup"><span data-stu-id="42392-166">DarkRed</span></span> |
| <span data-ttu-id="42392-167">Preset16</span><span class="sxs-lookup"><span data-stu-id="42392-167">Preset16</span></span> | <span data-ttu-id="42392-168">暗橙</span><span class="sxs-lookup"><span data-stu-id="42392-168">DarkOrange</span></span> |
| <span data-ttu-id="42392-169">Preset17</span><span class="sxs-lookup"><span data-stu-id="42392-169">Preset17</span></span> | <span data-ttu-id="42392-170">深褐</span><span class="sxs-lookup"><span data-stu-id="42392-170">DarkBrown</span></span> |
| <span data-ttu-id="42392-171">Preset18</span><span class="sxs-lookup"><span data-stu-id="42392-171">Preset18</span></span> | <span data-ttu-id="42392-172">深黄</span><span class="sxs-lookup"><span data-stu-id="42392-172">DarkYellow</span></span> |
| <span data-ttu-id="42392-173">Preset19</span><span class="sxs-lookup"><span data-stu-id="42392-173">Preset19</span></span> | <span data-ttu-id="42392-174">深绿</span><span class="sxs-lookup"><span data-stu-id="42392-174">DarkGreen</span></span> |
| <span data-ttu-id="42392-175">Preset20</span><span class="sxs-lookup"><span data-stu-id="42392-175">Preset20</span></span> | <span data-ttu-id="42392-176">深青</span><span class="sxs-lookup"><span data-stu-id="42392-176">DarkTeal</span></span> |
| <span data-ttu-id="42392-177">Preset21</span><span class="sxs-lookup"><span data-stu-id="42392-177">Preset21</span></span> | <span data-ttu-id="42392-178">深橄榄色</span><span class="sxs-lookup"><span data-stu-id="42392-178">DarkOlive</span></span> |
| <span data-ttu-id="42392-179">Preset22</span><span class="sxs-lookup"><span data-stu-id="42392-179">Preset22</span></span> | <span data-ttu-id="42392-180">深蓝</span><span class="sxs-lookup"><span data-stu-id="42392-180">DarkBlue</span></span> |
| <span data-ttu-id="42392-181">Preset23</span><span class="sxs-lookup"><span data-stu-id="42392-181">Preset23</span></span> | <span data-ttu-id="42392-182">深紫</span><span class="sxs-lookup"><span data-stu-id="42392-182">DarkPurple</span></span> |
| <span data-ttu-id="42392-183">Preset24</span><span class="sxs-lookup"><span data-stu-id="42392-183">Preset24</span></span> | <span data-ttu-id="42392-184">深蔓越橘色</span><span class="sxs-lookup"><span data-stu-id="42392-184">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="42392-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42392-185">JSON representation</span></span>
<span data-ttu-id="42392-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42392-186">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookCategory"
}-->

```json
{
  "color": "String",
  "displayName": "String"
}

```

## <a name="methods"></a><span data-ttu-id="42392-187">方法</span><span class="sxs-lookup"><span data-stu-id="42392-187">Methods</span></span>
| <span data-ttu-id="42392-188">方法</span><span class="sxs-lookup"><span data-stu-id="42392-188">Method</span></span>           | <span data-ttu-id="42392-189">返回类型</span><span class="sxs-lookup"><span data-stu-id="42392-189">Return Type</span></span>    |<span data-ttu-id="42392-190">说明</span><span class="sxs-lookup"><span data-stu-id="42392-190">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="42392-191">List categories</span><span class="sxs-lookup"><span data-stu-id="42392-191">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="42392-192">[outlookCategory](../resources/outlookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42392-192">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="42392-193">获取为用户定义的所有类别。</span><span class="sxs-lookup"><span data-stu-id="42392-193">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="42392-194">Get category</span><span class="sxs-lookup"><span data-stu-id="42392-194">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="42392-195">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="42392-195">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="42392-196">获取指定的 **outlookCategory** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="42392-196">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="42392-197">Create</span><span class="sxs-lookup"><span data-stu-id="42392-197">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="42392-198">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="42392-198">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="42392-199">在用户主类别列表中创建 **outlookCategory** 对象。</span><span class="sxs-lookup"><span data-stu-id="42392-199">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="42392-200">Update</span><span class="sxs-lookup"><span data-stu-id="42392-200">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="42392-201">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="42392-201">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="42392-202">更新指定 **outlookCategory** 对象的可写属性 **color**。</span><span class="sxs-lookup"><span data-stu-id="42392-202">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="42392-203">Delete</span><span class="sxs-lookup"><span data-stu-id="42392-203">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="42392-204">None</span><span class="sxs-lookup"><span data-stu-id="42392-204">None</span></span> |<span data-ttu-id="42392-205">删除指定的 **outlookCategory** 对象。</span><span class="sxs-lookup"><span data-stu-id="42392-205">Delete the specified **outlookCategory** object.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/resources/outlookcategory.md:
      Failed to parse any rows out of table with headers: |Pre-set constant|Color mapped to in Outlook|"
  ],
  "tocPath": ""
}-->
 
