---
title: outlookCategory 资源类型
description: 表示用户可以对 Outlook 项目（如邮件和事件）进行分组的类别依据。 用户定义主列表中的类别，并可应用用户定义的一个或多个
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: da65d6f2445a037ae4fcbbc8aaf05906bc0ae5c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534117"
---
# <a name="outlookcategory-resource-type"></a><span data-ttu-id="1cb3f-104">outlookCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="1cb3f-104">outlookCategory resource type</span></span>

<span data-ttu-id="1cb3f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cb3f-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="1cb3f-106">表示用户可以对 Outlook 项目（如邮件和事件）进行分组的类别依据。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-106">Represents a category by which a user can group Outlook items such as messages and events.</span></span> <span data-ttu-id="1cb3f-107">用户在主列表中定义类别，并且可以将这些用户定义的一个或多个类别应用到项目中。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-107">The user defines categories in a master list, and can apply one or more of these user-defined categories to an item.</span></span> 

<span data-ttu-id="1cb3f-108">使用 REST API，可以在用户类别的主列表中[创建](../api/outlookuser-post-mastercategories.md)和定义类别。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-108">Using the REST API, you can [create](../api/outlookuser-post-mastercategories.md) and define categories in the master list of categories for a user.</span></span> <span data-ttu-id="1cb3f-109">还可以[获取主类别列表](../api/outlookuser-list-mastercategories.md)、[获取特定类别](../api/outlookcategory-get.md)、[更新](../api/outlookcategory-update.md)与类别相关联的颜色，或[删除](../api/outlookcategory-delete.md)类别。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-109">You can also [get this master list of categories](../api/outlookuser-list-mastercategories.md), [get a specific category](../api/outlookcategory-get.md), [update](../api/outlookcategory-update.md) the color associated with a category, or [delete](../api/outlookcategory-delete.md) a category.</span></span> <span data-ttu-id="1cb3f-110">可以通过将类别的 **displayName** 属性分配给项目的 **categories** 集合，将类别应用到项目。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-110">You can apply a category to an item by assigning the **displayName** property of the category to the **categories** collection of the item.</span></span>
<span data-ttu-id="1cb3f-111">可以为资源分配以下类别：[联系人](contact.md)、[事件](event.md)、[邮件](message.md)和[帖子](post.md)。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-111">Resources that can be assigned categories include [contact](contact.md), [event](event.md), [message](message.md), and [post](post.md).</span></span>   

<span data-ttu-id="1cb3f-112">每个类别都有 2 个属性：**displayName** 和 **color**。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-112">Each category is attributed by 2 properties: **displayName** and **color**.</span></span> <span data-ttu-id="1cb3f-113">**displayName** 值在用户的主列表中必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-113">The **displayName** value must be unique in a user's master list.</span></span> <span data-ttu-id="1cb3f-114">然而，**color** 不一定是唯一的；主列表中的多个类别可以映射到相同颜色。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-114">The **color** however does not have to be unique; multiple categories in the master list can be mapped to the same color.</span></span> <span data-ttu-id="1cb3f-115">可以在用户的主列表中将多达 25 种不同的颜色映射到类别。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-115">You can map up to 25 different colors to categories in a user's master list.</span></span>

## <a name="properties"></a><span data-ttu-id="1cb3f-116">属性</span><span class="sxs-lookup"><span data-stu-id="1cb3f-116">Properties</span></span>
| <span data-ttu-id="1cb3f-117">属性</span><span class="sxs-lookup"><span data-stu-id="1cb3f-117">Property</span></span>     | <span data-ttu-id="1cb3f-118">类型</span><span class="sxs-lookup"><span data-stu-id="1cb3f-118">Type</span></span>   |<span data-ttu-id="1cb3f-119">说明</span><span class="sxs-lookup"><span data-stu-id="1cb3f-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cb3f-120">displayName</span><span class="sxs-lookup"><span data-stu-id="1cb3f-120">displayName</span></span>|<span data-ttu-id="1cb3f-121">String</span><span class="sxs-lookup"><span data-stu-id="1cb3f-121">String</span></span>|<span data-ttu-id="1cb3f-122">标识用户邮箱中的类别的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-122">A unique name that identifies a category in the user's mailbox.</span></span> <span data-ttu-id="1cb3f-123">在创建类别后，名称将无法更改。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-123">After a category is created, the name cannot be changed.</span></span> <span data-ttu-id="1cb3f-124">只读。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-124">Read-only.</span></span>|
|<span data-ttu-id="1cb3f-125">color</span><span class="sxs-lookup"><span data-stu-id="1cb3f-125">color</span></span>|<span data-ttu-id="1cb3f-126">categoryColor</span><span class="sxs-lookup"><span data-stu-id="1cb3f-126">categoryColor</span></span>|<span data-ttu-id="1cb3f-127">预先设定的颜色常数，它表示类别的特征，并映射到 25 种预定义颜色中的一种。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-127">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> <span data-ttu-id="1cb3f-128">请参阅下面的备注。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-128">See the note below.</span></span> |

> <span data-ttu-id="1cb3f-129">**注意**：**color** 的可能值为预设的常数，如 `None`、`preset0` 和 `preset1`。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-129">**Note** The possible values for **color** are pre-set constants such as `None`, `preset0` and `preset1`.</span></span> <span data-ttu-id="1cb3f-130">每个预设定的常数会被进一步映射到一种颜色；实际颜色取决于显示类别的 Outlook 客户端。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-130">Each pre-set constant is further mapped to a color; the actual color is dependent on the Outlook client that the categories are being displayed in.</span></span> <span data-ttu-id="1cb3f-131">下表显示了 Outlook（桌面客户端）中映射到每个预设常数的颜色。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-131">The following table shows the colors mapped to each pre-set constant for Outlook (desktop client).</span></span> 

| <span data-ttu-id="1cb3f-132">预设常数</span><span class="sxs-lookup"><span data-stu-id="1cb3f-132">Pre-set constant</span></span>  | <span data-ttu-id="1cb3f-133">Outlook 中映射的颜色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-133">Color mapped to in Outlook</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1cb3f-134">None</span><span class="sxs-lookup"><span data-stu-id="1cb3f-134">None</span></span> | <span data-ttu-id="1cb3f-135">没有映射的颜色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-135">No color mapped</span></span> |
| <span data-ttu-id="1cb3f-136">Preset0</span><span class="sxs-lookup"><span data-stu-id="1cb3f-136">Preset0</span></span> | <span data-ttu-id="1cb3f-137">红色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-137">Red</span></span> |
| <span data-ttu-id="1cb3f-138">Preset1</span><span class="sxs-lookup"><span data-stu-id="1cb3f-138">Preset1</span></span> | <span data-ttu-id="1cb3f-139">橙色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-139">Orange</span></span> |
| <span data-ttu-id="1cb3f-140">Preset2</span><span class="sxs-lookup"><span data-stu-id="1cb3f-140">Preset2</span></span> | <span data-ttu-id="1cb3f-141">褐色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-141">Brown</span></span> |
| <span data-ttu-id="1cb3f-142">Preset3</span><span class="sxs-lookup"><span data-stu-id="1cb3f-142">Preset3</span></span> | <span data-ttu-id="1cb3f-143">黄色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-143">Yellow</span></span> |
| <span data-ttu-id="1cb3f-144">Preset4</span><span class="sxs-lookup"><span data-stu-id="1cb3f-144">Preset4</span></span> | <span data-ttu-id="1cb3f-145">绿色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-145">Green</span></span> |
| <span data-ttu-id="1cb3f-146">Preset5</span><span class="sxs-lookup"><span data-stu-id="1cb3f-146">Preset5</span></span> | <span data-ttu-id="1cb3f-147">青色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-147">Teal</span></span> |
| <span data-ttu-id="1cb3f-148">Preset6</span><span class="sxs-lookup"><span data-stu-id="1cb3f-148">Preset6</span></span> | <span data-ttu-id="1cb3f-149">橄榄绿</span><span class="sxs-lookup"><span data-stu-id="1cb3f-149">Olive</span></span> |
| <span data-ttu-id="1cb3f-150">Preset7</span><span class="sxs-lookup"><span data-stu-id="1cb3f-150">Preset7</span></span> | <span data-ttu-id="1cb3f-151">蓝色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-151">Blue</span></span> |
| <span data-ttu-id="1cb3f-152">Preset8</span><span class="sxs-lookup"><span data-stu-id="1cb3f-152">Preset8</span></span> | <span data-ttu-id="1cb3f-153">紫色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-153">Purple</span></span> |
| <span data-ttu-id="1cb3f-154">Preset9</span><span class="sxs-lookup"><span data-stu-id="1cb3f-154">Preset9</span></span> | <span data-ttu-id="1cb3f-155">蔓越橘色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-155">Cranberry</span></span> |
| <span data-ttu-id="1cb3f-156">Preset10</span><span class="sxs-lookup"><span data-stu-id="1cb3f-156">Preset10</span></span> | <span data-ttu-id="1cb3f-157">青灰色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-157">Steel</span></span> |
| <span data-ttu-id="1cb3f-158">Preset11</span><span class="sxs-lookup"><span data-stu-id="1cb3f-158">Preset11</span></span> | <span data-ttu-id="1cb3f-159">深青灰</span><span class="sxs-lookup"><span data-stu-id="1cb3f-159">DarkSteel</span></span> |
| <span data-ttu-id="1cb3f-160">Preset12</span><span class="sxs-lookup"><span data-stu-id="1cb3f-160">Preset12</span></span> | <span data-ttu-id="1cb3f-161">灰色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-161">Gray</span></span> |
| <span data-ttu-id="1cb3f-162">Preset13</span><span class="sxs-lookup"><span data-stu-id="1cb3f-162">Preset13</span></span> | <span data-ttu-id="1cb3f-163">深灰</span><span class="sxs-lookup"><span data-stu-id="1cb3f-163">DarkGray</span></span> |
| <span data-ttu-id="1cb3f-164">Preset14</span><span class="sxs-lookup"><span data-stu-id="1cb3f-164">Preset14</span></span> | <span data-ttu-id="1cb3f-165">黑色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-165">Black</span></span> |
| <span data-ttu-id="1cb3f-166">Preset15</span><span class="sxs-lookup"><span data-stu-id="1cb3f-166">Preset15</span></span> | <span data-ttu-id="1cb3f-167">深红</span><span class="sxs-lookup"><span data-stu-id="1cb3f-167">DarkRed</span></span> |
| <span data-ttu-id="1cb3f-168">Preset16</span><span class="sxs-lookup"><span data-stu-id="1cb3f-168">Preset16</span></span> | <span data-ttu-id="1cb3f-169">暗橙</span><span class="sxs-lookup"><span data-stu-id="1cb3f-169">DarkOrange</span></span> |
| <span data-ttu-id="1cb3f-170">Preset17</span><span class="sxs-lookup"><span data-stu-id="1cb3f-170">Preset17</span></span> | <span data-ttu-id="1cb3f-171">深褐</span><span class="sxs-lookup"><span data-stu-id="1cb3f-171">DarkBrown</span></span> |
| <span data-ttu-id="1cb3f-172">Preset18</span><span class="sxs-lookup"><span data-stu-id="1cb3f-172">Preset18</span></span> | <span data-ttu-id="1cb3f-173">深黄</span><span class="sxs-lookup"><span data-stu-id="1cb3f-173">DarkYellow</span></span> |
| <span data-ttu-id="1cb3f-174">Preset19</span><span class="sxs-lookup"><span data-stu-id="1cb3f-174">Preset19</span></span> | <span data-ttu-id="1cb3f-175">深绿</span><span class="sxs-lookup"><span data-stu-id="1cb3f-175">DarkGreen</span></span> |
| <span data-ttu-id="1cb3f-176">Preset20</span><span class="sxs-lookup"><span data-stu-id="1cb3f-176">Preset20</span></span> | <span data-ttu-id="1cb3f-177">深青</span><span class="sxs-lookup"><span data-stu-id="1cb3f-177">DarkTeal</span></span> |
| <span data-ttu-id="1cb3f-178">Preset21</span><span class="sxs-lookup"><span data-stu-id="1cb3f-178">Preset21</span></span> | <span data-ttu-id="1cb3f-179">深橄榄色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-179">DarkOlive</span></span> |
| <span data-ttu-id="1cb3f-180">Preset22</span><span class="sxs-lookup"><span data-stu-id="1cb3f-180">Preset22</span></span> | <span data-ttu-id="1cb3f-181">深蓝</span><span class="sxs-lookup"><span data-stu-id="1cb3f-181">DarkBlue</span></span> |
| <span data-ttu-id="1cb3f-182">Preset23</span><span class="sxs-lookup"><span data-stu-id="1cb3f-182">Preset23</span></span> | <span data-ttu-id="1cb3f-183">深紫</span><span class="sxs-lookup"><span data-stu-id="1cb3f-183">DarkPurple</span></span> |
| <span data-ttu-id="1cb3f-184">Preset24</span><span class="sxs-lookup"><span data-stu-id="1cb3f-184">Preset24</span></span> | <span data-ttu-id="1cb3f-185">深蔓越橘色</span><span class="sxs-lookup"><span data-stu-id="1cb3f-185">DarkCranberry</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1cb3f-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1cb3f-186">JSON representation</span></span>
<span data-ttu-id="1cb3f-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-187">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="1cb3f-188">Methods</span><span class="sxs-lookup"><span data-stu-id="1cb3f-188">Methods</span></span>
| <span data-ttu-id="1cb3f-189">方法</span><span class="sxs-lookup"><span data-stu-id="1cb3f-189">Method</span></span>           | <span data-ttu-id="1cb3f-190">返回类型</span><span class="sxs-lookup"><span data-stu-id="1cb3f-190">Return Type</span></span>    |<span data-ttu-id="1cb3f-191">说明</span><span class="sxs-lookup"><span data-stu-id="1cb3f-191">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1cb3f-192">List categories</span><span class="sxs-lookup"><span data-stu-id="1cb3f-192">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="1cb3f-193">[outlookCategory](../resources/outlookcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1cb3f-193">[outlookCategory](../resources/outlookcategory.md) collection</span></span> |<span data-ttu-id="1cb3f-194">获取为用户定义的所有类别。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-194">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="1cb3f-195">Get category</span><span class="sxs-lookup"><span data-stu-id="1cb3f-195">Get category</span></span>](../api/outlookcategory-get.md) | [<span data-ttu-id="1cb3f-196">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="1cb3f-196">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="1cb3f-197">获取指定的 **outlookCategory** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-197">Get the properties and relationships of the specified **outlookCategory** object.</span></span>|
|[<span data-ttu-id="1cb3f-198">Create</span><span class="sxs-lookup"><span data-stu-id="1cb3f-198">Create</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="1cb3f-199">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="1cb3f-199">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="1cb3f-200">在用户主类别列表中创建 **outlookCategory** 对象。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-200">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="1cb3f-201">Update</span><span class="sxs-lookup"><span data-stu-id="1cb3f-201">Update</span></span>](../api/outlookcategory-update.md) | [<span data-ttu-id="1cb3f-202">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="1cb3f-202">outlookCategory</span></span>](../resources/outlookcategory.md) |<span data-ttu-id="1cb3f-203">更新指定 **outlookCategory** 对象的可写属性 **color**。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-203">Update the writable property, **color**, of the specified **outlookCategory** object.</span></span> |
|[<span data-ttu-id="1cb3f-204">删除</span><span class="sxs-lookup"><span data-stu-id="1cb3f-204">Delete</span></span>](../api/outlookcategory-delete.md) | <span data-ttu-id="1cb3f-205">无</span><span class="sxs-lookup"><span data-stu-id="1cb3f-205">None</span></span> |<span data-ttu-id="1cb3f-206">删除指定的 **outlookCategory** 对象。</span><span class="sxs-lookup"><span data-stu-id="1cb3f-206">Delete the specified **outlookCategory** object.</span></span> |


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
 
