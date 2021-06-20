---
title: accessReviewInactiveUsersQueryScope 资源类型
description: 一种 accessReviewQueryScope 类型，只允许在访问评审范围内选择非活动用户。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b0e28deb57a84ac9d1a7072ebc2e351a704d1142
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031051"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a><span data-ttu-id="7ebd5-103">accessReviewInactiveUsersQueryScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ebd5-103">accessReviewInactiveUsersQueryScope resource type</span></span>

<span data-ttu-id="7ebd5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ebd5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ebd5-105">一种 [accessReviewQueryScope](../resources/accessreviewqueryscope.md) 类型，只允许在访问评审范围内选择非活动用户。</span><span class="sxs-lookup"><span data-stu-id="7ebd5-105">A type of [accessReviewQueryScope](../resources/accessreviewqueryscope.md) that allows only inactive users to be selected in the scope of an access review.</span></span> <span data-ttu-id="7ebd5-106">不活动持续时间根据[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)的 settings 属性中定义的访问评审实例的开始日期，根据用户的上次登录日期计算。</span><span class="sxs-lookup"><span data-stu-id="7ebd5-106">The duration of inactivity is calculated based on the user's last sign-in date against the access review instance's start date as defined in the **settings** property of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).</span></span>

<span data-ttu-id="7ebd5-107">继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="7ebd5-107">Inherits from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7ebd5-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ebd5-108">Properties</span></span>
|<span data-ttu-id="7ebd5-109">属性</span><span class="sxs-lookup"><span data-stu-id="7ebd5-109">Property</span></span>|<span data-ttu-id="7ebd5-110">类型</span><span class="sxs-lookup"><span data-stu-id="7ebd5-110">Type</span></span>|<span data-ttu-id="7ebd5-111">说明</span><span class="sxs-lookup"><span data-stu-id="7ebd5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ebd5-112">inactiveDuration</span><span class="sxs-lookup"><span data-stu-id="7ebd5-112">inactiveDuration</span></span>|<span data-ttu-id="7ebd5-113">期限</span><span class="sxs-lookup"><span data-stu-id="7ebd5-113">Duration</span></span>|<span data-ttu-id="7ebd5-114">定义不活动持续时间。</span><span class="sxs-lookup"><span data-stu-id="7ebd5-114">Defines the duration of inactivity.</span></span> <span data-ttu-id="7ebd5-115">与访问评审实例的开始日期相比，不活动基于用户的最后登录日期。</span><span class="sxs-lookup"><span data-stu-id="7ebd5-115">Inactivity is based on the last sign in date of the user compared to the access review instance's start date.</span></span> <span data-ttu-id="7ebd5-116">如果未指定此属性，则为其分配默认值 `PT0S` 。</span><span class="sxs-lookup"><span data-stu-id="7ebd5-116">If this property is not specified, it's assigned the default value `PT0S`.</span></span>|
|<span data-ttu-id="7ebd5-117">查询</span><span class="sxs-lookup"><span data-stu-id="7ebd5-117">query</span></span>|<span data-ttu-id="7ebd5-118">String</span><span class="sxs-lookup"><span data-stu-id="7ebd5-118">String</span></span>|<span data-ttu-id="7ebd5-119">继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="7ebd5-119">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|
|<span data-ttu-id="7ebd5-120">queryRoot</span><span class="sxs-lookup"><span data-stu-id="7ebd5-120">queryRoot</span></span>|<span data-ttu-id="7ebd5-121">String</span><span class="sxs-lookup"><span data-stu-id="7ebd5-121">String</span></span>|<span data-ttu-id="7ebd5-122">继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="7ebd5-122">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|
|<span data-ttu-id="7ebd5-123">queryType</span><span class="sxs-lookup"><span data-stu-id="7ebd5-123">queryType</span></span>|<span data-ttu-id="7ebd5-124">String</span><span class="sxs-lookup"><span data-stu-id="7ebd5-124">String</span></span>|<span data-ttu-id="7ebd5-125">继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="7ebd5-125">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|

<span data-ttu-id="7ebd5-126">还必须使用值 **指定 @odata.type** 类型属性 `#microsoft.graph.accessReviewInactiveUsersQueryScope` 。</span><span class="sxs-lookup"><span data-stu-id="7ebd5-126">You must also specify the **@odata.type** type property with the value `#microsoft.graph.accessReviewInactiveUsersQueryScope`.</span></span> <span data-ttu-id="7ebd5-127">有关使用 **accessReviewInactiveUsersQueryScope** 的范围配置选项的详细信息，请参阅使用 Microsoft Graph [API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)。 </span><span class="sxs-lookup"><span data-stu-id="7ebd5-127">For more about configuration options for **scope** using **accessReviewInactiveUsersQueryScope**, see [Configure the scope of your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).</span></span>

## <a name="relationships"></a><span data-ttu-id="7ebd5-128">关系</span><span class="sxs-lookup"><span data-stu-id="7ebd5-128">Relationships</span></span>
<span data-ttu-id="7ebd5-129">无。</span><span class="sxs-lookup"><span data-stu-id="7ebd5-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ebd5-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ebd5-130">JSON representation</span></span>
<span data-ttu-id="7ebd5-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ebd5-131">The following is a JSON representation of the resource.</span></span>
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
