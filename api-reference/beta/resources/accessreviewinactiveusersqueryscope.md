---
title: accessReviewInactiveUsersQueryScope 资源类型
description: 一种 accessReviewQueryScope 类型，只允许在访问评审范围内选择非活动用户。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 80d415125679ddbb44a08fe75f33b115e4ba1f04
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579744"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a><span data-ttu-id="39781-103">accessReviewInactiveUsersQueryScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="39781-103">accessReviewInactiveUsersQueryScope resource type</span></span>

<span data-ttu-id="39781-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39781-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="39781-105">一种 [accessReviewQueryScope](../resources/accessreviewqueryscope.md) 类型，只允许在访问评审范围内选择非活动用户。</span><span class="sxs-lookup"><span data-stu-id="39781-105">A type of [accessReviewQueryScope](../resources/accessreviewqueryscope.md) that allows only inactive users to be selected in the scope of an access review.</span></span> <span data-ttu-id="39781-106">不活动持续时间根据[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)的 settings 属性中定义的访问评审实例的开始日期，根据用户的上次登录日期计算。</span><span class="sxs-lookup"><span data-stu-id="39781-106">The duration of inactivity is calculated based on the user's last sign-in date against the access review instance's start date as defined in the **settings** property of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span>

<span data-ttu-id="39781-107">继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="39781-107">Inherits from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="39781-108">属性</span><span class="sxs-lookup"><span data-stu-id="39781-108">Properties</span></span>
|<span data-ttu-id="39781-109">属性</span><span class="sxs-lookup"><span data-stu-id="39781-109">Property</span></span>|<span data-ttu-id="39781-110">类型</span><span class="sxs-lookup"><span data-stu-id="39781-110">Type</span></span>|<span data-ttu-id="39781-111">说明</span><span class="sxs-lookup"><span data-stu-id="39781-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39781-112">inactiveDuration</span><span class="sxs-lookup"><span data-stu-id="39781-112">inactiveDuration</span></span>|<span data-ttu-id="39781-113">期限</span><span class="sxs-lookup"><span data-stu-id="39781-113">Duration</span></span>|<span data-ttu-id="39781-114">定义不活动持续时间。</span><span class="sxs-lookup"><span data-stu-id="39781-114">Defines the duration of inactivity.</span></span> <span data-ttu-id="39781-115">与访问评审实例的开始日期相比，不活动基于用户的最后登录日期。</span><span class="sxs-lookup"><span data-stu-id="39781-115">Inactivity is based on the last sign in date of the user compared to the access review instance's start date.</span></span> <span data-ttu-id="39781-116">如果未指定此属性，则为其分配默认值 `PT0S` 。</span><span class="sxs-lookup"><span data-stu-id="39781-116">If this property is not specified, it's assigned the default value `PT0S`.</span></span>|
|<span data-ttu-id="39781-117">查询</span><span class="sxs-lookup"><span data-stu-id="39781-117">query</span></span>|<span data-ttu-id="39781-118">String</span><span class="sxs-lookup"><span data-stu-id="39781-118">String</span></span>|<span data-ttu-id="39781-119">继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="39781-119">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|
|<span data-ttu-id="39781-120">queryRoot</span><span class="sxs-lookup"><span data-stu-id="39781-120">queryRoot</span></span>|<span data-ttu-id="39781-121">String</span><span class="sxs-lookup"><span data-stu-id="39781-121">String</span></span>|<span data-ttu-id="39781-122">继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="39781-122">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|
|<span data-ttu-id="39781-123">queryType</span><span class="sxs-lookup"><span data-stu-id="39781-123">queryType</span></span>|<span data-ttu-id="39781-124">String</span><span class="sxs-lookup"><span data-stu-id="39781-124">String</span></span>|<span data-ttu-id="39781-125">继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="39781-125">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|

<span data-ttu-id="39781-126">还必须使用值 **指定 @odata.type** 类型属性 `#microsoft.graph.accessReviewInactiveUsersQueryScope` 。</span><span class="sxs-lookup"><span data-stu-id="39781-126">You must also specify the **@odata.type** type property with the value `#microsoft.graph.accessReviewInactiveUsersQueryScope`.</span></span> <span data-ttu-id="39781-127">有关使用 **accessReviewInactiveUsersQueryScope** 的范围配置选项的详细信息，请参阅使用 Microsoft Graph [API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)。 </span><span class="sxs-lookup"><span data-stu-id="39781-127">For more about configuration options for **scope** using **accessReviewInactiveUsersQueryScope**, see [Configure the scope of your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span></span>

## <a name="relationships"></a><span data-ttu-id="39781-128">关系</span><span class="sxs-lookup"><span data-stu-id="39781-128">Relationships</span></span>
<span data-ttu-id="39781-129">无。</span><span class="sxs-lookup"><span data-stu-id="39781-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="39781-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39781-130">JSON representation</span></span>
<span data-ttu-id="39781-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39781-131">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInactiveUsersQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String",
  "inactiveDuration": "String (duration)"
}
```
