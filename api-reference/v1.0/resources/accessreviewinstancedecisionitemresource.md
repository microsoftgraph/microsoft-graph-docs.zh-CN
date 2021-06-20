---
title: accessReviewInstanceDecisionItemResource 资源类型
description: 表示与决策项关联的资源。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d75fb2f2b2fd4338f63d2c71893f2dab17524bc8
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031044"
---
# <a name="accessreviewinstancedecisionitemresource-resource-type"></a><span data-ttu-id="9d0a8-103">accessReviewInstanceDecisionItemResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d0a8-103">accessReviewInstanceDecisionItemResource resource type</span></span>

<span data-ttu-id="9d0a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d0a8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d0a8-105">访问评审中的每个决策项表示主体对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="9d0a8-105">Every decision item in an access review represents a principal's access to a resource.</span></span> <span data-ttu-id="9d0a8-106">accessReviewInstanceDecisionItemResource 对象表示与决策项关联的资源。</span><span class="sxs-lookup"><span data-stu-id="9d0a8-106">The accessReviewInstanceDecisionItemResource object represents the resource associated with the decision item.</span></span>

## <a name="properties"></a><span data-ttu-id="9d0a8-107">属性</span><span class="sxs-lookup"><span data-stu-id="9d0a8-107">Properties</span></span>
|<span data-ttu-id="9d0a8-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d0a8-108">Property</span></span>|<span data-ttu-id="9d0a8-109">类型</span><span class="sxs-lookup"><span data-stu-id="9d0a8-109">Type</span></span>|<span data-ttu-id="9d0a8-110">说明</span><span class="sxs-lookup"><span data-stu-id="9d0a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d0a8-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9d0a8-111">displayName</span></span>|<span data-ttu-id="9d0a8-112">String</span><span class="sxs-lookup"><span data-stu-id="9d0a8-112">String</span></span>|<span data-ttu-id="9d0a8-113">资源的显示名称</span><span class="sxs-lookup"><span data-stu-id="9d0a8-113">Display name of the resource</span></span>|
|<span data-ttu-id="9d0a8-114">id</span><span class="sxs-lookup"><span data-stu-id="9d0a8-114">id</span></span>|<span data-ttu-id="9d0a8-115">String</span><span class="sxs-lookup"><span data-stu-id="9d0a8-115">String</span></span>|<span data-ttu-id="9d0a8-116">资源的标识符</span><span class="sxs-lookup"><span data-stu-id="9d0a8-116">Identifier of the resource</span></span>|
|<span data-ttu-id="9d0a8-117">type</span><span class="sxs-lookup"><span data-stu-id="9d0a8-117">type</span></span>|<span data-ttu-id="9d0a8-118">String</span><span class="sxs-lookup"><span data-stu-id="9d0a8-118">String</span></span>|<span data-ttu-id="9d0a8-119">资源的类型。</span><span class="sxs-lookup"><span data-stu-id="9d0a8-119">Type of resource.</span></span> <span data-ttu-id="9d0a8-120">类型包括 `Group` `ServicePrincipal` `DirectoryRole` ：、、、、。 `AzureRole` `AccessPackageAssignmentPolicy`</span><span class="sxs-lookup"><span data-stu-id="9d0a8-120">Types include: `Group`, `ServicePrincipal`, `DirectoryRole`, `AzureRole`, `AccessPackageAssignmentPolicy`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d0a8-121">关系</span><span class="sxs-lookup"><span data-stu-id="9d0a8-121">Relationships</span></span>
<span data-ttu-id="9d0a8-122">无。</span><span class="sxs-lookup"><span data-stu-id="9d0a8-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d0a8-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d0a8-123">JSON representation</span></span>
<span data-ttu-id="9d0a8-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d0a8-124">The following is a JSON representation of the resource.</span></span>
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
