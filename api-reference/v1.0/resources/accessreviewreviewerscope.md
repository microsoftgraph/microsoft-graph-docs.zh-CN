---
title: accessReviewReviewerScope 资源类型
description: 表示将审阅访问评审的人。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 85d602f72bc103b1588c3c9a76455fa2de0f8259
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030808"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="b51af-103">accessReviewReviewerScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="b51af-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="b51af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b51af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b51af-105">accessReviewReviewerScope 定义谁将审阅 [accessReviewScheduleDefinition 的实例](accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="b51af-105">The accessReviewReviewerScope defines who will review instances of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="b51af-106">它是一个 OData 查询，它允许将审阅者指定为用户 (（即特定用户、组所有者和组成员) ）的静态列表，或者动态地将审阅者指定为其经理或组所有者审阅每个用户。</span><span class="sxs-lookup"><span data-stu-id="b51af-106">It is an OData query that allows reviewers to be specified both as a static list of users (that is, specific users, group owners, and group members) or dynamically in which every user is reviewed by their manager or by group owners.</span></span> <span data-ttu-id="b51af-107">若要创建自审阅 (用户查看自己的访问权限) ，请不要在 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 创建时提供审阅者。</span><span class="sxs-lookup"><span data-stu-id="b51af-107">To create a self-review (where users review their own access), do not provide reviewers on [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) creation.</span></span>

<span data-ttu-id="b51af-108">继承自 [accessReviewScope](../resources/accessreviewscope.md)。</span><span class="sxs-lookup"><span data-stu-id="b51af-108">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b51af-109">属性</span><span class="sxs-lookup"><span data-stu-id="b51af-109">Properties</span></span>
| <span data-ttu-id="b51af-110">属性</span><span class="sxs-lookup"><span data-stu-id="b51af-110">Property</span></span> | <span data-ttu-id="b51af-111">类型</span><span class="sxs-lookup"><span data-stu-id="b51af-111">Type</span></span> | <span data-ttu-id="b51af-112">说明</span><span class="sxs-lookup"><span data-stu-id="b51af-112">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="b51af-113">查询</span><span class="sxs-lookup"><span data-stu-id="b51af-113">query</span></span> | <span data-ttu-id="b51af-114">String</span><span class="sxs-lookup"><span data-stu-id="b51af-114">String</span></span> | <span data-ttu-id="b51af-115">用于指定审阅者的查询。</span><span class="sxs-lookup"><span data-stu-id="b51af-115">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="b51af-116">有关示例，请参阅表。</span><span class="sxs-lookup"><span data-stu-id="b51af-116">See table for examples.</span></span> |
| <span data-ttu-id="b51af-117">queryType</span><span class="sxs-lookup"><span data-stu-id="b51af-117">queryType</span></span> | <span data-ttu-id="b51af-118">String</span><span class="sxs-lookup"><span data-stu-id="b51af-118">String</span></span> | <span data-ttu-id="b51af-119">查询的类型。</span><span class="sxs-lookup"><span data-stu-id="b51af-119">The type of query.</span></span> <span data-ttu-id="b51af-120">示例包括 `MicrosoftGraph` `ARM` 和 。</span><span class="sxs-lookup"><span data-stu-id="b51af-120">Examples include `MicrosoftGraph` and `ARM`.</span></span> |
| <span data-ttu-id="b51af-121">queryRoot</span><span class="sxs-lookup"><span data-stu-id="b51af-121">queryRoot</span></span> | <span data-ttu-id="b51af-122">String</span><span class="sxs-lookup"><span data-stu-id="b51af-122">String</span></span> | <span data-ttu-id="b51af-123">在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。</span><span class="sxs-lookup"><span data-stu-id="b51af-123">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="b51af-124">此属性仅在指定了相对查询（例如 ） `./manager` 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="b51af-124">This property is only required if a relative query, for example, `./manager`, is specified.</span></span> <span data-ttu-id="b51af-125">可能的值 `decisions` ：。</span><span class="sxs-lookup"><span data-stu-id="b51af-125">Possible value: `decisions`.</span></span> |

<span data-ttu-id="b51af-126">有关审阅者的 **配置选项的详细信息**，请参阅使用 Microsoft Graph API 将审阅者 [分配给你的访问Graph定义](/graph/accessreviews-reviewers-concept)。</span><span class="sxs-lookup"><span data-stu-id="b51af-126">For more about configuration options for **reviewers**, see [Assign reviewers to your access review definition using the Microsoft Graph API](/graph/accessreviews-reviewers-concept).</span></span>


## <a name="relationships"></a><span data-ttu-id="b51af-127">关系</span><span class="sxs-lookup"><span data-stu-id="b51af-127">Relationships</span></span>
<span data-ttu-id="b51af-128">无。</span><span class="sxs-lookup"><span data-stu-id="b51af-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b51af-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b51af-129">JSON representation</span></span>
<span data-ttu-id="b51af-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b51af-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewReviewerScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewerScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
