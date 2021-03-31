---
title: accessReviewInstanceDecisionItemResource 资源类型
description: 访问评审中的每个决策项表示主体对资源的访问权限。 accessReviewInstanceDecisionItemResource 表示与决策项关联的资源。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 879a0b1f74fa08e0ae66e5aaf5ab45b9d96de397
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469743"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a><span data-ttu-id="23dc0-104">accessReviewInstanceDecisionItemResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="23dc0-104">accessReviewInstanceDecisionItemResource resource type</span></span>

<span data-ttu-id="23dc0-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23dc0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="23dc0-106">访问评审中的每个决策项表示主体对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="23dc0-106">Every decision item in an access review represents a principal's access to a resource.</span></span> <span data-ttu-id="23dc0-107">accessReviewInstanceDecisionItemResource 表示与决策项关联的资源。</span><span class="sxs-lookup"><span data-stu-id="23dc0-107">accessReviewInstanceDecisionItemResource represents the resource associated with the decision item.</span></span>

## <a name="properties"></a><span data-ttu-id="23dc0-108">属性</span><span class="sxs-lookup"><span data-stu-id="23dc0-108">Properties</span></span>
|<span data-ttu-id="23dc0-109">属性</span><span class="sxs-lookup"><span data-stu-id="23dc0-109">Property</span></span>|<span data-ttu-id="23dc0-110">类型</span><span class="sxs-lookup"><span data-stu-id="23dc0-110">Type</span></span>|<span data-ttu-id="23dc0-111">说明</span><span class="sxs-lookup"><span data-stu-id="23dc0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23dc0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="23dc0-112">displayName</span></span>|<span data-ttu-id="23dc0-113">String</span><span class="sxs-lookup"><span data-stu-id="23dc0-113">String</span></span>|<span data-ttu-id="23dc0-114">资源的显示名称</span><span class="sxs-lookup"><span data-stu-id="23dc0-114">Display name of the resource</span></span>|
|<span data-ttu-id="23dc0-115">id</span><span class="sxs-lookup"><span data-stu-id="23dc0-115">id</span></span>|<span data-ttu-id="23dc0-116">String</span><span class="sxs-lookup"><span data-stu-id="23dc0-116">String</span></span>|<span data-ttu-id="23dc0-117">资源 ID</span><span class="sxs-lookup"><span data-stu-id="23dc0-117">Resource ID</span></span>|
|<span data-ttu-id="23dc0-118">type</span><span class="sxs-lookup"><span data-stu-id="23dc0-118">type</span></span>|<span data-ttu-id="23dc0-119">String</span><span class="sxs-lookup"><span data-stu-id="23dc0-119">String</span></span>|<span data-ttu-id="23dc0-120">资源的类型。</span><span class="sxs-lookup"><span data-stu-id="23dc0-120">Type of resource.</span></span> <span data-ttu-id="23dc0-121">类型包括：Group、ServicePrincipal、DirectoryRole、AzureRole、AccessPackageAssignmentPolicy。</span><span class="sxs-lookup"><span data-stu-id="23dc0-121">Types include: Group, ServicePrincipal, DirectoryRole, AzureRole, AccessPackageAssignmentPolicy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23dc0-122">关系</span><span class="sxs-lookup"><span data-stu-id="23dc0-122">Relationships</span></span>
<span data-ttu-id="23dc0-123">无。</span><span class="sxs-lookup"><span data-stu-id="23dc0-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23dc0-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23dc0-124">JSON representation</span></span>
<span data-ttu-id="23dc0-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23dc0-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemResource",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String"
}
```
