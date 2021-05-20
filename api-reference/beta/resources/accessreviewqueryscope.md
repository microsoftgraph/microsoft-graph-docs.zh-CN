---
title: accessReviewQueryScope 资源类型
description: 定义在访问评审中将审阅哪些项。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 07a13d12b821d055c8200da2fa5450958a8f53ee
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579276"
---
# <a name="accessreviewqueryscope-resource-type"></a><span data-ttu-id="4eed2-103">accessReviewQueryScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="4eed2-103">accessReviewQueryScope resource type</span></span>

<span data-ttu-id="4eed2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4eed2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="4eed2-105">accessReviewQueryScope 对象定义将在访问评审中 [审阅哪些项](../resources/accessreviewsv2-root.md)。</span><span class="sxs-lookup"><span data-stu-id="4eed2-105">An accessReviewQueryScope object defines what will be reviewed in an [access review](../resources/accessreviewsv2-root.md).</span></span> <span data-ttu-id="4eed2-106">若要将访问评审的范围确定为非活动用户，请参阅 [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="4eed2-106">To scope an access review to inactive users, see [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span></span> 

<span data-ttu-id="4eed2-107">继承自 [accessReviewScope](../resources/accessreviewscope.md)。</span><span class="sxs-lookup"><span data-stu-id="4eed2-107">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4eed2-108">属性</span><span class="sxs-lookup"><span data-stu-id="4eed2-108">Properties</span></span>
|<span data-ttu-id="4eed2-109">属性</span><span class="sxs-lookup"><span data-stu-id="4eed2-109">Property</span></span>|<span data-ttu-id="4eed2-110">类型</span><span class="sxs-lookup"><span data-stu-id="4eed2-110">Type</span></span>|<span data-ttu-id="4eed2-111">说明</span><span class="sxs-lookup"><span data-stu-id="4eed2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eed2-112">查询</span><span class="sxs-lookup"><span data-stu-id="4eed2-112">query</span></span>|<span data-ttu-id="4eed2-113">String</span><span class="sxs-lookup"><span data-stu-id="4eed2-113">String</span></span>|<span data-ttu-id="4eed2-114">表示将在访问评审中审阅哪些内容的查询。</span><span class="sxs-lookup"><span data-stu-id="4eed2-114">The query representing what will be reviewed in an access review.</span></span>|
|<span data-ttu-id="4eed2-115">queryRoot</span><span class="sxs-lookup"><span data-stu-id="4eed2-115">queryRoot</span></span>|<span data-ttu-id="4eed2-116">String</span><span class="sxs-lookup"><span data-stu-id="4eed2-116">String</span></span>|<span data-ttu-id="4eed2-117">在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。</span><span class="sxs-lookup"><span data-stu-id="4eed2-117">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="4eed2-118">此属性仅在指定了相对查询时是必需的。</span><span class="sxs-lookup"><span data-stu-id="4eed2-118">This property is only required if a relative query is specified.</span></span> <span data-ttu-id="4eed2-119">例如，`./manager`。</span><span class="sxs-lookup"><span data-stu-id="4eed2-119">For example, `./manager`.</span></span>|
|<span data-ttu-id="4eed2-120">queryType</span><span class="sxs-lookup"><span data-stu-id="4eed2-120">queryType</span></span>|<span data-ttu-id="4eed2-121">String</span><span class="sxs-lookup"><span data-stu-id="4eed2-121">String</span></span>|<span data-ttu-id="4eed2-122">指示查询的类型。</span><span class="sxs-lookup"><span data-stu-id="4eed2-122">Indicates the type of query.</span></span> <span data-ttu-id="4eed2-123">类型包括 `MicrosoftGraph` `ARM` 和 。</span><span class="sxs-lookup"><span data-stu-id="4eed2-123">Types include `MicrosoftGraph` and `ARM`.</span></span>|

<span data-ttu-id="4eed2-124">强烈建议@odata值指定 **@odata.type** `#microsoft.graph.accessReviewQueryScope` 属性。</span><span class="sxs-lookup"><span data-stu-id="4eed2-124">Specifying the **@odata.type** type property with the value `#microsoft.graph.accessReviewQueryScope` is highly recommended.</span></span> <span data-ttu-id="4eed2-125">有关使用 **accessReviewQueryScope** 的范围配置选项的详细信息，请参阅使用 Microsoft Graph [API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)。 </span><span class="sxs-lookup"><span data-stu-id="4eed2-125">For more about configuration options for **scope** using **accessReviewQueryScope**, see [Configure the scope of your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span></span>

## <a name="relationships"></a><span data-ttu-id="4eed2-126">关系</span><span class="sxs-lookup"><span data-stu-id="4eed2-126">Relationships</span></span>
<span data-ttu-id="4eed2-127">无。</span><span class="sxs-lookup"><span data-stu-id="4eed2-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4eed2-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4eed2-128">JSON representation</span></span>
<span data-ttu-id="4eed2-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4eed2-129">The following is a JSON representation of the resource.</span></span>
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
