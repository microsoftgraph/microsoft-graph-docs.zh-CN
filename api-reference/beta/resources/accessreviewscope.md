---
title: accessReviewScope 资源类型
description: '在 Azure AD 访问评审功能中，表示将在访问 `accessReviewScope` 评审中审阅的实体。  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8739ff822ffc6b0f2989b80a150c7d968880f532
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133439"
---
# <a name="accessreviewscope-resource-type"></a><span data-ttu-id="487f2-103">accessReviewScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="487f2-103">accessReviewScope resource type</span></span>

<span data-ttu-id="487f2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="487f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="487f2-105">**accessReviewScope** 定义在 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)中将检查哪些实体。</span><span class="sxs-lookup"><span data-stu-id="487f2-105">The **accessReviewScope** defines what entities will be reviewed in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="487f2-106">这表示为 odata 查询。</span><span class="sxs-lookup"><span data-stu-id="487f2-106">This is expressed as an odata query.</span></span> <span data-ttu-id="487f2-107">还必须表示查询类型，以便支持方案来查看 MicrosoftGraph 外部的实体，如ARM。</span><span class="sxs-lookup"><span data-stu-id="487f2-107">The query type must also be expressed so that scenarios can be supported to review entities outside of MicrosoftGraph, such as ARM.</span></span>

## <a name="properties"></a><span data-ttu-id="487f2-108">属性</span><span class="sxs-lookup"><span data-stu-id="487f2-108">Properties</span></span>
| <span data-ttu-id="487f2-109">属性</span><span class="sxs-lookup"><span data-stu-id="487f2-109">Property</span></span>   | <span data-ttu-id="487f2-110">类型</span><span class="sxs-lookup"><span data-stu-id="487f2-110">Type</span></span>  | <span data-ttu-id="487f2-111">说明</span><span class="sxs-lookup"><span data-stu-id="487f2-111">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="487f2-112">查询</span><span class="sxs-lookup"><span data-stu-id="487f2-112">query</span></span> |<span data-ttu-id="487f2-113">字符串</span><span class="sxs-lookup"><span data-stu-id="487f2-113">String</span></span>  | <span data-ttu-id="487f2-114">指定将审阅哪些项的查询。</span><span class="sxs-lookup"><span data-stu-id="487f2-114">The query specifying what will be reviewed.</span></span> <span data-ttu-id="487f2-115">有关示例，请参阅表。</span><span class="sxs-lookup"><span data-stu-id="487f2-115">See table for examples.</span></span> |
|<span data-ttu-id="487f2-116">queryType</span><span class="sxs-lookup"><span data-stu-id="487f2-116">queryType</span></span>  |<span data-ttu-id="487f2-117">字符串</span><span class="sxs-lookup"><span data-stu-id="487f2-117">String</span></span> | <span data-ttu-id="487f2-118">查询的类型。</span><span class="sxs-lookup"><span data-stu-id="487f2-118">The type of query.</span></span> <span data-ttu-id="487f2-119">示例包括 MicrosoftGraph 和 ARM。</span><span class="sxs-lookup"><span data-stu-id="487f2-119">Examples include MicrosoftGraph and ARM.</span></span> |

### <a name="supported-queries-for-accessreviewscope-as-scope"></a><span data-ttu-id="487f2-120">支持将 accessReviewScope 作为范围的查询</span><span class="sxs-lookup"><span data-stu-id="487f2-120">Supported queries for accessReviewScope as scope</span></span>
<span data-ttu-id="487f2-121">以下是在 `scope` [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)中作为属性支持的查询</span><span class="sxs-lookup"><span data-stu-id="487f2-121">The following are queries supported as the `scope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="487f2-122">应用场景</span><span class="sxs-lookup"><span data-stu-id="487f2-122">Scenario</span></span>| <span data-ttu-id="487f2-123">查询</span><span class="sxs-lookup"><span data-stu-id="487f2-123">Query</span></span> | <span data-ttu-id="487f2-124">其他注释</span><span class="sxs-lookup"><span data-stu-id="487f2-124">Additional Comments</span></span> |
|--|--|-- |
| <span data-ttu-id="487f2-125">审阅分配给组的所有用户</span><span class="sxs-lookup"><span data-stu-id="487f2-125">Review of all users assigned to a group</span></span> | <span data-ttu-id="487f2-126">/groups/{group id}/transitiveMembers</span><span class="sxs-lookup"><span data-stu-id="487f2-126">/groups/{group id}/transitiveMembers</span></span> ||
| <span data-ttu-id="487f2-127">查看分配给组的来宾用户</span><span class="sxs-lookup"><span data-stu-id="487f2-127">Review of guest users assigned to a group</span></span> | <span data-ttu-id="487f2-128">/groups/{group id}/microsoft.graph.user/？$count=true&$filter= (userType eq 'Guest') </span><span class="sxs-lookup"><span data-stu-id="487f2-128">/groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> ||
| <span data-ttu-id="487f2-129">查看分配给所有组的来宾用户</span><span class="sxs-lookup"><span data-stu-id="487f2-129">Review of guest users assigned to all groups</span></span> | <span data-ttu-id="487f2-130">./members/microsoft.graph.user/？$count=true&$filter= (userType eq 'Guest') </span><span class="sxs-lookup"><span data-stu-id="487f2-130">./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> | <span data-ttu-id="487f2-131">请注意，相应的 instanceEnumerationScope 还应传递到 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="487f2-131">Note that the corresponding instanceEnumerationScope should also be passed in to the accessReviewScheduleDefinition.</span></span> <span data-ttu-id="487f2-132">有关 instanceEnumerationScope 查询，请参阅下表。</span><span class="sxs-lookup"><span data-stu-id="487f2-132">See table below for instanceEnumerationScope query.</span></span> |
| <span data-ttu-id="487f2-133">权利管理访问包审查</span><span class="sxs-lookup"><span data-stu-id="487f2-133">Entitlement Management Access Package Assigment Reviews</span></span> | <span data-ttu-id="487f2-134">/identityGovernance/entitlementManagement/accessPackageAssignments？$filter= (accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}') </span><span class="sxs-lookup"><span data-stu-id="487f2-134">/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')</span></span>| <span data-ttu-id="487f2-135">请注意，访问包分配评审仅支持 READ</span><span class="sxs-lookup"><span data-stu-id="487f2-135">Note that only READ is supported for Access Package Assignment Reviews</span></span>|

### <a name="supported-queries-for-accessreviewscope-as-instanceenumerationscope"></a><span data-ttu-id="487f2-136">支持将 accessReviewScope 作为 instanceEnumerationScope 的查询</span><span class="sxs-lookup"><span data-stu-id="487f2-136">Supported queries for accessReviewScope as instanceEnumerationScope</span></span>
<span data-ttu-id="487f2-137">以下是在 `instanceEnumerationScope` [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)中作为属性支持的查询</span><span class="sxs-lookup"><span data-stu-id="487f2-137">The following are queries supported as the `instanceEnumerationScope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="487f2-138">应用场景</span><span class="sxs-lookup"><span data-stu-id="487f2-138">Scenario</span></span>| <span data-ttu-id="487f2-139">查询</span><span class="sxs-lookup"><span data-stu-id="487f2-139">Query</span></span> | <span data-ttu-id="487f2-140">其他注释</span><span class="sxs-lookup"><span data-stu-id="487f2-140">Additional Comments</span></span> |
|--|--|--|
| <span data-ttu-id="487f2-141">查看分配给所有组的来宾用户（不包括指定的组）</span><span class="sxs-lookup"><span data-stu-id="487f2-141">Review of guest users assigned to all groups, excluding specified groups</span></span> | <span data-ttu-id="487f2-142">/groups？$filter= (groupTypes/any (c：c+eq+'Unified') and id ne '{group id}' and id ne '{group id}' and id ne '{group id}') &$count=true</span><span class="sxs-lookup"><span data-stu-id="487f2-142">/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and id ne '{group id}' and id ne '{group id}' and id ne '{group id}')&$count=true</span></span> | <span data-ttu-id="487f2-143">请注意，相应的作用域还应传递到 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="487f2-143">Note that the corresponding scope should also be passed in to the accessReviewScheduleDefinition.</span></span> <span data-ttu-id="487f2-144">有关范围查询，请参阅上述范围属性表中的"查看分配给所有组的来宾用户"。</span><span class="sxs-lookup"><span data-stu-id="487f2-144">See "Review of guest users assigned to all groups" in scope property table above for the scope query.</span></span> |

## <a name="relationships"></a><span data-ttu-id="487f2-145">关系</span><span class="sxs-lookup"><span data-stu-id="487f2-145">Relationships</span></span>
<span data-ttu-id="487f2-146">无。</span><span class="sxs-lookup"><span data-stu-id="487f2-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="487f2-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="487f2-147">JSON representation</span></span>
<span data-ttu-id="487f2-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="487f2-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScope",
  "query": "String",
  "queryType": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
