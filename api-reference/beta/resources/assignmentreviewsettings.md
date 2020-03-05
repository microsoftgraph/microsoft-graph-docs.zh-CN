---
title: assignmentReviewSettings 资源类型
description: AssignmentReviewSettings type，用于访问包分配策略的 accessReviewSettings 属性，提供了其他设置，以选择必须查看此策略中的访问包分配的用户以及必须检查的频率。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a26728fb39fccd1512a559638c595551a20c0042
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508176"
---
# <a name="assignmentreviewsettings-resource-type"></a><span data-ttu-id="64b19-103">assignmentReviewSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="64b19-103">assignmentReviewSettings resource type</span></span>

<span data-ttu-id="64b19-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="64b19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64b19-105">用于[访问包分配策略](accesspackageassignmentpolicy.md)的**accessReviewSettings**属性。</span><span class="sxs-lookup"><span data-stu-id="64b19-105">Used for the **accessReviewSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="64b19-106">提供其他设置，以选择必须查看此策略中的访问包分配的用户以及必须查看的频率。</span><span class="sxs-lookup"><span data-stu-id="64b19-106">Provides additional settings to select who must review access package assignments from this policy, and how often they must be reviewed.</span></span>  

## <a name="properties"></a><span data-ttu-id="64b19-107">属性</span><span class="sxs-lookup"><span data-stu-id="64b19-107">Properties</span></span>

<span data-ttu-id="64b19-108">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="64b19-108">This type has the following properties:</span></span>

| <span data-ttu-id="64b19-109">属性</span><span class="sxs-lookup"><span data-stu-id="64b19-109">Property</span></span>                     | <span data-ttu-id="64b19-110">类型</span><span class="sxs-lookup"><span data-stu-id="64b19-110">Type</span></span>                      | <span data-ttu-id="64b19-111">说明</span><span class="sxs-lookup"><span data-stu-id="64b19-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="64b19-112">isEnabled</span><span class="sxs-lookup"><span data-stu-id="64b19-112">isEnabled</span></span>| <span data-ttu-id="64b19-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="64b19-113">Boolean</span></span> | <span data-ttu-id="64b19-114">如果为 true，则此策略中的工作分配需要进行访问检查。</span><span class="sxs-lookup"><span data-stu-id="64b19-114">If true, access reviews are required for assignments from this policy.</span></span> |
| <span data-ttu-id="64b19-115">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="64b19-115">recurrenceType</span></span> | <span data-ttu-id="64b19-116">String</span><span class="sxs-lookup"><span data-stu-id="64b19-116">String</span></span> | <span data-ttu-id="64b19-117">定期的间隔，例如`monthly`或。 `quarterly`</span><span class="sxs-lookup"><span data-stu-id="64b19-117">The interval for recurrence, such as `monthly` or `quarterly`.</span></span> |
| <span data-ttu-id="64b19-118">reviewerType</span><span class="sxs-lookup"><span data-stu-id="64b19-118">reviewerType</span></span> | <span data-ttu-id="64b19-119">String</span><span class="sxs-lookup"><span data-stu-id="64b19-119">String</span></span> | <span data-ttu-id="64b19-120">应要求谁是`Self`或`Reviewers`，由谁来进行审阅。</span><span class="sxs-lookup"><span data-stu-id="64b19-120">Who should be asked to do the review, either `Self` or `Reviewers`.</span></span> |
| <span data-ttu-id="64b19-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="64b19-121">startDateTime</span></span> | <span data-ttu-id="64b19-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64b19-122">DateTimeOffset</span></span> | <span data-ttu-id="64b19-123">第一次审阅应开始时。</span><span class="sxs-lookup"><span data-stu-id="64b19-123">When the first review should start.</span></span> |
| <span data-ttu-id="64b19-124">durationInDays</span><span class="sxs-lookup"><span data-stu-id="64b19-124">durationInDays</span></span> | <span data-ttu-id="64b19-125">Int32</span><span class="sxs-lookup"><span data-stu-id="64b19-125">Int32</span></span> | <span data-ttu-id="64b19-126">允许来自审阅者的输入的天数。</span><span class="sxs-lookup"><span data-stu-id="64b19-126">The number of days to allow input from reviewers.</span></span>|
| <span data-ttu-id="64b19-127">审批</span><span class="sxs-lookup"><span data-stu-id="64b19-127">reviewers</span></span> | <span data-ttu-id="64b19-128">[userSet](userset.md)集合</span><span class="sxs-lookup"><span data-stu-id="64b19-128">[userSet](userset.md) collection</span></span> | <span data-ttu-id="64b19-129">如果 reviewerType 是`Reviewers`，则此集合将使用[singleUser](singleuser.md)和[groupMembers](groupmembers.md)的集合指定将成为审阅者的用户（通过 ID 或作为组的成员）。</span><span class="sxs-lookup"><span data-stu-id="64b19-129">If the reviewerType is `Reviewers`, this collection specifies the users who will be reviewers, either by ID or as members of a group, using a collection of [singleUser](singleuser.md) and [groupMembers](groupmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="64b19-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64b19-130">JSON representation</span></span>


<span data-ttu-id="64b19-131">以下是策略的 "访问评审设置" 属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64b19-131">The following is a JSON representation of the access review settings property of a policy.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignmentReviewSettings",
  "baseType": ""
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
