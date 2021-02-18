---
title: accessReviewDecision 资源类型
description: accessReviewDecision 表示对特定实体的访问的 Azure AD 访问评审决定。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 52d4e2a262d3a90010cc0e254e11f2d723a5e550
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292691"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="26463-103">accessReviewDecision 资源类型</span><span class="sxs-lookup"><span data-stu-id="26463-103">accessReviewDecision resource type</span></span>

<span data-ttu-id="26463-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26463-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

<span data-ttu-id="26463-105">在 Azure AD [访问评审](accessreviews-root.md) 功能中，表示特定实体访问权限的 `accessReviewDecision` Azure AD 访问评审决定。</span><span class="sxs-lookup"><span data-stu-id="26463-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="26463-106">在访问评审或定期访问评审的实例中，每个审阅的用户 `accessReviewDecision` 有一个。</span><span class="sxs-lookup"><span data-stu-id="26463-106">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="26463-107">例如，如果一个组有两个来宾和一个非来宾作为成员，并且对该组执行来宾的访问评审，则有两个访问评审决策对象。</span><span class="sxs-lookup"><span data-stu-id="26463-107">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="26463-108">如果审阅者更改其决定，或者另一个审阅者替代他们，则更新 `accessReviewDecision` 。</span><span class="sxs-lookup"><span data-stu-id="26463-108">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="26463-109">方法</span><span class="sxs-lookup"><span data-stu-id="26463-109">Methods</span></span>

<span data-ttu-id="26463-110">无。</span><span class="sxs-lookup"><span data-stu-id="26463-110">None.</span></span>  <span data-ttu-id="26463-111">当访问评审初始化时，此功能会自动创建此类型的对象，并且无法删除。</span><span class="sxs-lookup"><span data-stu-id="26463-111">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="26463-112">可以使用决策和决定关系从访问评审[中检索](../api/accessreview-listmydecisions.md)它们[](../api/accessreview-listdecisions.md)。</span><span class="sxs-lookup"><span data-stu-id="26463-112">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="26463-113">属性</span><span class="sxs-lookup"><span data-stu-id="26463-113">Properties</span></span>

<span data-ttu-id="26463-114">此表说明了此类型对象的基本属性。</span><span class="sxs-lookup"><span data-stu-id="26463-114">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="26463-115">属性</span><span class="sxs-lookup"><span data-stu-id="26463-115">Property</span></span>                        | <span data-ttu-id="26463-116">类型</span><span class="sxs-lookup"><span data-stu-id="26463-116">Type</span></span>                         | <span data-ttu-id="26463-117">说明</span><span class="sxs-lookup"><span data-stu-id="26463-117">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="26463-118">访问评审中决策的 ID。</span><span class="sxs-lookup"><span data-stu-id="26463-118">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="26463-119">访问评审的功能生成 ID。</span><span class="sxs-lookup"><span data-stu-id="26463-119">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="26463-120">userIdentity</span><span class="sxs-lookup"><span data-stu-id="26463-120">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="26463-121">审阅者的标识。</span><span class="sxs-lookup"><span data-stu-id="26463-121">The identity of the reviewer.</span></span> <span data-ttu-id="26463-122">如果将建议用作审阅，则 userPrincipalName 为空。</span><span class="sxs-lookup"><span data-stu-id="26463-122">If the recommendation was used as the review, the userPrincipalName is empty.</span></span>                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="26463-123">提供了此访问权限的最新审阅日期和时间。</span><span class="sxs-lookup"><span data-stu-id="26463-123">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="26463-124">审阅的结果，其中一个 `NotReviewed` ， `Deny` 或 `DontKnow` `Approve` 。</span><span class="sxs-lookup"><span data-stu-id="26463-124">The result of the review, one of `NotReviewed`, `Deny`, `DontKnow` or `Approve`.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="26463-125">审阅者的业务理由（如果提供）。</span><span class="sxs-lookup"><span data-stu-id="26463-125">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="26463-126">userIdentity</span><span class="sxs-lookup"><span data-stu-id="26463-126">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="26463-127">审阅完成后，如果手动应用了结果，则应用该决定的用户的用户标识。</span><span class="sxs-lookup"><span data-stu-id="26463-127">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span> <span data-ttu-id="26463-128">如果自动应用评价，则 userPrincipalName 为空。</span><span class="sxs-lookup"><span data-stu-id="26463-128">If the review was auto-applied, the userPrincipalName is empty.</span></span>                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="26463-129">应用审阅决策的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="26463-129">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="26463-130">应用决策的结果，其中一个 ， `NotApplied` `Success` 或 `Failed` `NotFound` `NotSupported` 。</span><span class="sxs-lookup"><span data-stu-id="26463-130">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="26463-131">向审阅者显示的功能生成的建议，其中一 `Approve` 个或 `Deny` `NotAvailable` 。</span><span class="sxs-lookup"><span data-stu-id="26463-131">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="26463-132">此外，根据拥有已对象类型访问权限的对象的属性，可能会存在其他属性。</span><span class="sxs-lookup"><span data-stu-id="26463-132">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="26463-133">例如，如果访问评审决策是特定用户的组成员身份或应用程序访问权限，则可能会删除其访问权限的用户通过以下属性进行标识：</span><span class="sxs-lookup"><span data-stu-id="26463-133">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="26463-134">属性</span><span class="sxs-lookup"><span data-stu-id="26463-134">Property</span></span>                        | <span data-ttu-id="26463-135">类型</span><span class="sxs-lookup"><span data-stu-id="26463-135">Type</span></span>                         | <span data-ttu-id="26463-136">说明</span><span class="sxs-lookup"><span data-stu-id="26463-136">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="26463-137">已审阅其访问权限的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="26463-137">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="26463-138">已显示名称访问权限的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="26463-138">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="26463-139">已审阅其访问权限的用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="26463-139">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="26463-140">关系</span><span class="sxs-lookup"><span data-stu-id="26463-140">Relationships</span></span>

<span data-ttu-id="26463-141">无。</span><span class="sxs-lookup"><span data-stu-id="26463-141">None.</span></span>  <span data-ttu-id="26463-142">可以使用[accessReview](accessreview.md)对象的决策和决定关系从访问评审[](../api/accessreview-listdecisions.md)中检索[](../api/accessreview-listmydecisions.md)此类型的对象。</span><span class="sxs-lookup"><span data-stu-id="26463-142">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="26463-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="26463-143">See also</span></span>

| <span data-ttu-id="26463-144">方法</span><span class="sxs-lookup"><span data-stu-id="26463-144">Method</span></span>           | <span data-ttu-id="26463-145">返回类型</span><span class="sxs-lookup"><span data-stu-id="26463-145">Return Type</span></span>    |<span data-ttu-id="26463-146">说明</span><span class="sxs-lookup"><span data-stu-id="26463-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26463-147">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="26463-147">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="26463-148">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26463-148">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="26463-149">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="26463-149">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="26463-150">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="26463-150">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="26463-151">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26463-151">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="26463-152">作为审阅者，获取我关于 accessReview 的决定。</span><span class="sxs-lookup"><span data-stu-id="26463-152">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26463-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26463-153">JSON representation</span></span>

<span data-ttu-id="26463-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26463-154">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReviewDecision"
}-->

```json
{
"id": "string (identifier)",
"accessReviewId": "string (identifier)",
"reviewedBy": "microsoft.graph.userIdentity",
"reviewedDate": "string (timestamp)",
"reviewResult": "string",
"justification": "string",
"appliedBy": "microsoft.graph.userIdentity",
"appliedDateTime": "string (timestamp)",
"applyResult": "string",
"accessRecommendation": "string",
"userId": "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


