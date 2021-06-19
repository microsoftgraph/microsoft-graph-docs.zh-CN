---
title: principalResourceMembershipsScope 资源类型
description: 允许选择访问评审作用域，以检查所选主体对选定资源的访问权限。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d2706246089bcc6a26e2ec8ca3cd115edd18e10a
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030843"
---
# <a name="principalresourcemembershipsscope-resource-type"></a><span data-ttu-id="891ff-103">principalResourceMembershipsScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="891ff-103">principalResourceMembershipsScope resource type</span></span>

<span data-ttu-id="891ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="891ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="891ff-105">principalResourceMembershipsScope 是 [accessReviewScope](accessreviewscope.md) 的一种类型，它允许您选择主体作用域的集合和资源作用域的集合，并查看所选主体对选定资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="891ff-105">The principalResourceMembershipsScope is a type of [accessReviewScope](accessreviewscope.md) which allows you to select a collection of principal scopes and a collection of resource scopes and review access of selected principals to selected resources.</span></span> <span data-ttu-id="891ff-106">它用于配置[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)的 scope 属性。 </span><span class="sxs-lookup"><span data-stu-id="891ff-106">It is used to configure the **scope** property of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span>

<span data-ttu-id="891ff-107">继承自 [accessReviewScope](../resources/accessreviewscope.md)。</span><span class="sxs-lookup"><span data-stu-id="891ff-107">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="891ff-108">属性</span><span class="sxs-lookup"><span data-stu-id="891ff-108">Properties</span></span>
|<span data-ttu-id="891ff-109">属性</span><span class="sxs-lookup"><span data-stu-id="891ff-109">Property</span></span>|<span data-ttu-id="891ff-110">类型</span><span class="sxs-lookup"><span data-stu-id="891ff-110">Type</span></span>|<span data-ttu-id="891ff-111">说明</span><span class="sxs-lookup"><span data-stu-id="891ff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="891ff-112">principalScopes</span><span class="sxs-lookup"><span data-stu-id="891ff-112">principalScopes</span></span>|<span data-ttu-id="891ff-113">[accessReviewScope](../resources/accessreviewscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="891ff-113">[accessReviewScope](../resources/accessreviewscope.md) collection</span></span>|<span data-ttu-id="891ff-114">定义访问评审中审查其资源访问权限的主体的范围。</span><span class="sxs-lookup"><span data-stu-id="891ff-114">Defines the scopes of the principals whose access to resources are reviewed in the access review.</span></span>|
|<span data-ttu-id="891ff-115">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="891ff-115">resourceScopes</span></span>|<span data-ttu-id="891ff-116">[accessReviewScope](../resources/accessreviewscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="891ff-116">[accessReviewScope](../resources/accessreviewscope.md) collection</span></span>|<span data-ttu-id="891ff-117">定义审查其访问权限的资源的范围。</span><span class="sxs-lookup"><span data-stu-id="891ff-117">Defines the scopes of the resources for which access is reviewed.</span></span>|

<span data-ttu-id="891ff-118">还必须使用值 **指定 @odata.type** 类型属性 `#microsoft.graph.principalResourceMembershipsScope` 。</span><span class="sxs-lookup"><span data-stu-id="891ff-118">You must also specify the **@odata.type** type property with the value `#microsoft.graph.principalResourceMembershipsScope`.</span></span> <span data-ttu-id="891ff-119">有关使用 **principalResourceMembershipsScope** 的范围配置选项的详细信息，请参阅使用 Microsoft Graph API 配置访问 [评审定义的范围](/graph/accessreviews-scope-concept)。 </span><span class="sxs-lookup"><span data-stu-id="891ff-119">For more about configuration options for **scope** using **principalResourceMembershipsScope**, see [Configure the scope of your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span></span>

## <a name="relationships"></a><span data-ttu-id="891ff-120">关系</span><span class="sxs-lookup"><span data-stu-id="891ff-120">Relationships</span></span>
<span data-ttu-id="891ff-121">无。</span><span class="sxs-lookup"><span data-stu-id="891ff-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="891ff-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="891ff-122">JSON representation</span></span>
<span data-ttu-id="891ff-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="891ff-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.principalResourceMembershipsScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
  "principalScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ],
  "resourceScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ]
}
```
