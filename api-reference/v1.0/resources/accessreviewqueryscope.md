---
title: accessReviewQueryScope 资源类型
description: 定义在访问评审中需要审阅哪些项。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5217524105fd5dcca0248b331f5cc5d0584784aa
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031043"
---
# <a name="accessreviewqueryscope-resource-type"></a><span data-ttu-id="313d6-103">accessReviewQueryScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="313d6-103">accessReviewQueryScope resource type</span></span>

<span data-ttu-id="313d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="313d6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="313d6-105">accessReviewQueryScope 对象定义在访问评审中 [审阅的对象](../resources/accessreviewsv2-root.md)。</span><span class="sxs-lookup"><span data-stu-id="313d6-105">An accessReviewQueryScope object defines what is reviewed in an [access review](../resources/accessreviewsv2-root.md).</span></span> <span data-ttu-id="313d6-106">若要将访问评审的范围确定为非活动用户，请参阅 [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="313d6-106">To scope an access review to inactive users, see [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span></span> 

<span data-ttu-id="313d6-107">继承自 [accessReviewScope](../resources/accessreviewscope.md)。</span><span class="sxs-lookup"><span data-stu-id="313d6-107">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="313d6-108">属性</span><span class="sxs-lookup"><span data-stu-id="313d6-108">Properties</span></span>
|<span data-ttu-id="313d6-109">属性</span><span class="sxs-lookup"><span data-stu-id="313d6-109">Property</span></span>|<span data-ttu-id="313d6-110">类型</span><span class="sxs-lookup"><span data-stu-id="313d6-110">Type</span></span>|<span data-ttu-id="313d6-111">说明</span><span class="sxs-lookup"><span data-stu-id="313d6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="313d6-112">查询</span><span class="sxs-lookup"><span data-stu-id="313d6-112">query</span></span>|<span data-ttu-id="313d6-113">String</span><span class="sxs-lookup"><span data-stu-id="313d6-113">String</span></span>|<span data-ttu-id="313d6-114">表示将在访问评审中审阅哪些内容的查询。</span><span class="sxs-lookup"><span data-stu-id="313d6-114">The query representing what will be reviewed in an access review.</span></span>|
|<span data-ttu-id="313d6-115">queryRoot</span><span class="sxs-lookup"><span data-stu-id="313d6-115">queryRoot</span></span>|<span data-ttu-id="313d6-116">String</span><span class="sxs-lookup"><span data-stu-id="313d6-116">String</span></span>|<span data-ttu-id="313d6-117">在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。</span><span class="sxs-lookup"><span data-stu-id="313d6-117">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="313d6-118">此属性仅在指定了相对查询时是必需的。</span><span class="sxs-lookup"><span data-stu-id="313d6-118">This property is only required if a relative query is specified.</span></span> <span data-ttu-id="313d6-119">例如，`./manager`。</span><span class="sxs-lookup"><span data-stu-id="313d6-119">For example, `./manager`.</span></span>|
|<span data-ttu-id="313d6-120">queryType</span><span class="sxs-lookup"><span data-stu-id="313d6-120">queryType</span></span>|<span data-ttu-id="313d6-121">String</span><span class="sxs-lookup"><span data-stu-id="313d6-121">String</span></span>|<span data-ttu-id="313d6-122">指示查询的类型。</span><span class="sxs-lookup"><span data-stu-id="313d6-122">Indicates the type of query.</span></span> <span data-ttu-id="313d6-123">类型包括 `MicrosoftGraph` `ARM` 和 。</span><span class="sxs-lookup"><span data-stu-id="313d6-123">Types include `MicrosoftGraph` and `ARM`.</span></span>|

<span data-ttu-id="313d6-124">强烈建议@odata值指定 **@odata.type** `#microsoft.graph.accessReviewQueryScope` 属性。</span><span class="sxs-lookup"><span data-stu-id="313d6-124">Specifying the **@odata.type** type property with the value `#microsoft.graph.accessReviewQueryScope` is highly recommended.</span></span> <span data-ttu-id="313d6-125">有关使用 **accessReviewQueryScope** 的范围配置选项的详细信息，请参阅使用 Microsoft Graph [API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)。 </span><span class="sxs-lookup"><span data-stu-id="313d6-125">For more about configuration options for **scope** using **accessReviewQueryScope**, see [Configure the scope of your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span></span>

## <a name="relationships"></a><span data-ttu-id="313d6-126">关系</span><span class="sxs-lookup"><span data-stu-id="313d6-126">Relationships</span></span>
<span data-ttu-id="313d6-127">无。</span><span class="sxs-lookup"><span data-stu-id="313d6-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="313d6-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="313d6-128">JSON representation</span></span>
<span data-ttu-id="313d6-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="313d6-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
