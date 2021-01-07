---
title: assignmentReviewSettings 资源类型
description: assignmentReviewSettings 类型（用于访问包分配策略的 accessReviewSettings 属性）提供了其他设置，用于选择必须从此策略查看访问包分配以及必须查看访问包分配多久查看一次。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0bbc595395fbe7995b8ce7dfb7fa8e575faf58e8
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777692"
---
# <a name="assignmentreviewsettings-resource-type"></a><span data-ttu-id="b323d-103">assignmentReviewSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b323d-103">assignmentReviewSettings resource type</span></span>

<span data-ttu-id="b323d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b323d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b323d-105">用于 **访问包分配策略的 accessReviewSettings** [属性](accesspackageassignmentpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="b323d-105">Used for the **accessReviewSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="b323d-106">提供其他设置，以选择必须从此策略查看访问包分配以及必须查看访问包分配多久。</span><span class="sxs-lookup"><span data-stu-id="b323d-106">Provides additional settings to select who must review access package assignments from this policy, and how often they must be reviewed.</span></span>  

## <a name="properties"></a><span data-ttu-id="b323d-107">属性</span><span class="sxs-lookup"><span data-stu-id="b323d-107">Properties</span></span>

<span data-ttu-id="b323d-108">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="b323d-108">This type has the following properties:</span></span>

| <span data-ttu-id="b323d-109">属性</span><span class="sxs-lookup"><span data-stu-id="b323d-109">Property</span></span>                     | <span data-ttu-id="b323d-110">类型</span><span class="sxs-lookup"><span data-stu-id="b323d-110">Type</span></span>                      | <span data-ttu-id="b323d-111">说明</span><span class="sxs-lookup"><span data-stu-id="b323d-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="b323d-112">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b323d-112">isEnabled</span></span>| <span data-ttu-id="b323d-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="b323d-113">Boolean</span></span> | <span data-ttu-id="b323d-114">如果为 true，则此策略中的分配需要访问评审。</span><span class="sxs-lookup"><span data-stu-id="b323d-114">If true, access reviews are required for assignments from this policy.</span></span> |
| <span data-ttu-id="b323d-115">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="b323d-115">recurrenceType</span></span> | <span data-ttu-id="b323d-116">String</span><span class="sxs-lookup"><span data-stu-id="b323d-116">String</span></span> | <span data-ttu-id="b323d-117">定期的间隔，例如或 `monthly` `quarterly` 。</span><span class="sxs-lookup"><span data-stu-id="b323d-117">The interval for recurrence, such as `monthly` or `quarterly`.</span></span> |
| <span data-ttu-id="b323d-118">reviewerType</span><span class="sxs-lookup"><span data-stu-id="b323d-118">reviewerType</span></span> | <span data-ttu-id="b323d-119">String</span><span class="sxs-lookup"><span data-stu-id="b323d-119">String</span></span> | <span data-ttu-id="b323d-120">应要求谁执行审阅，或 `Self` `Reviewers` 。</span><span class="sxs-lookup"><span data-stu-id="b323d-120">Who should be asked to do the review, either `Self` or `Reviewers`.</span></span> |
| <span data-ttu-id="b323d-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b323d-121">startDateTime</span></span> | <span data-ttu-id="b323d-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b323d-122">DateTimeOffset</span></span> | <span data-ttu-id="b323d-123">第一次审阅应何时开始。</span><span class="sxs-lookup"><span data-stu-id="b323d-123">When the first review should start.</span></span> |
| <span data-ttu-id="b323d-124">durationInDays</span><span class="sxs-lookup"><span data-stu-id="b323d-124">durationInDays</span></span> | <span data-ttu-id="b323d-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b323d-125">Int32</span></span> | <span data-ttu-id="b323d-126">允许审阅者输入的天数。</span><span class="sxs-lookup"><span data-stu-id="b323d-126">The number of days to allow input from reviewers.</span></span>|
| <span data-ttu-id="b323d-127">审阅者</span><span class="sxs-lookup"><span data-stu-id="b323d-127">reviewers</span></span> | <span data-ttu-id="b323d-128">[userSet](userset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b323d-128">[userSet](userset.md) collection</span></span> | <span data-ttu-id="b323d-129">如果 reviewerType 为，则此集合使用 `Reviewers` [singleUser](singleuser.md) 和 [groupMembers](groupmembers.md)集合指定将按 ID 或作为组的成员成为审阅者的用户。</span><span class="sxs-lookup"><span data-stu-id="b323d-129">If the reviewerType is `Reviewers`, this collection specifies the users who will be reviewers, either by ID or as members of a group, using a collection of [singleUser](singleuser.md) and [groupMembers](groupmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b323d-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b323d-130">JSON representation</span></span>


<span data-ttu-id="b323d-131">下面是策略的访问评审设置属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b323d-131">The following is a JSON representation of the access review settings property of a policy.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignmentReviewSettings"
}-->

```json
{
  "isEnabled": true,
  "recurrenceType": "quarterly",
  "reviewerType": "Self",
  "startDateTime": "2020-01-23T07:59:59.998Z",
  "durationInDays": 25,
  "reviewers": []
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignmentReviewSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


