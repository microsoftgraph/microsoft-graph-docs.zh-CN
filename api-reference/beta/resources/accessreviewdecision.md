---
title: accessReviewDecision 资源类型
description: accessReviewDecision 表示对特定实体的访问的 Azure AD 访问评审决定。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c33849920a06154f0c2a0ac781dcd5cdf64fa51f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133509"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="6d058-103">accessReviewDecision 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d058-103">accessReviewDecision resource type</span></span>

<span data-ttu-id="6d058-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d058-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d058-105">在 Azure AD [访问评审](accessreviews-root.md) 功能中，表示特定实体访问权限的 `accessReviewDecision` Azure AD 访问评审决定。</span><span class="sxs-lookup"><span data-stu-id="6d058-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="6d058-106">在访问评审或定期访问评审的实例中，每个审阅的用户有 `accessReviewDecision` 一个。</span><span class="sxs-lookup"><span data-stu-id="6d058-106">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="6d058-107">例如，如果一个组有两个来宾和一个非来宾作为成员，并且对该组执行了来宾的访问评审，则存在两个访问评审决策对象。</span><span class="sxs-lookup"><span data-stu-id="6d058-107">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="6d058-108">如果审阅者更改其决定，或者另一个审阅者替代他们，则更新 `accessReviewDecision` 。</span><span class="sxs-lookup"><span data-stu-id="6d058-108">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="6d058-109">方法</span><span class="sxs-lookup"><span data-stu-id="6d058-109">Methods</span></span>

<span data-ttu-id="6d058-110">无。</span><span class="sxs-lookup"><span data-stu-id="6d058-110">None.</span></span>  <span data-ttu-id="6d058-111">此类型的对象在访问评审初始化时由功能自动创建，并且无法删除。</span><span class="sxs-lookup"><span data-stu-id="6d058-111">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="6d058-112">可以使用决策和决策关系从访问评审中[检索](../api/accessreview-listmydecisions.md)它们[](../api/accessreview-listdecisions.md)。</span><span class="sxs-lookup"><span data-stu-id="6d058-112">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="6d058-113">属性</span><span class="sxs-lookup"><span data-stu-id="6d058-113">Properties</span></span>

<span data-ttu-id="6d058-114">此表说明了此类型的对象的基本属性。</span><span class="sxs-lookup"><span data-stu-id="6d058-114">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="6d058-115">属性</span><span class="sxs-lookup"><span data-stu-id="6d058-115">Property</span></span>                        | <span data-ttu-id="6d058-116">类型</span><span class="sxs-lookup"><span data-stu-id="6d058-116">Type</span></span>                         | <span data-ttu-id="6d058-117">说明</span><span class="sxs-lookup"><span data-stu-id="6d058-117">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="6d058-118">访问评审中决策的 ID。</span><span class="sxs-lookup"><span data-stu-id="6d058-118">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="6d058-119">访问评审的功能生成 ID。</span><span class="sxs-lookup"><span data-stu-id="6d058-119">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="6d058-120">userIdentity</span><span class="sxs-lookup"><span data-stu-id="6d058-120">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="6d058-121">审阅者的标识。</span><span class="sxs-lookup"><span data-stu-id="6d058-121">The identity of the reviewer.</span></span> <span data-ttu-id="6d058-122">如果将建议用作评论，则 userPrincipalName 为空。</span><span class="sxs-lookup"><span data-stu-id="6d058-122">If the recommendation was used as the review, the userPrincipalName is empty.</span></span>                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="6d058-123">提供了此访问权限的最新审阅日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6d058-123">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="6d058-124">审阅的结果，其中一个 `NotReviewed` ， `Deny` 或 `DontKnow` `Approve` 。</span><span class="sxs-lookup"><span data-stu-id="6d058-124">The result of the review, one of `NotReviewed`, `Deny`, `DontKnow` or `Approve`.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="6d058-125">审阅者的业务理由（如果提供）。</span><span class="sxs-lookup"><span data-stu-id="6d058-125">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="6d058-126">userIdentity</span><span class="sxs-lookup"><span data-stu-id="6d058-126">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="6d058-127">审阅完成后，如果手动应用了结果，则应用了该决策的用户的用户标识。</span><span class="sxs-lookup"><span data-stu-id="6d058-127">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span> <span data-ttu-id="6d058-128">如果自动应用评价，则 userPrincipalName 为空。</span><span class="sxs-lookup"><span data-stu-id="6d058-128">If the review was auto-applied, the userPrincipalName is empty.</span></span>                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="6d058-129">应用审阅决策的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6d058-129">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="6d058-130">应用决策的结果，其中一个 ， `NotApplied` `Success` ， `Failed` 或 `NotFound` `NotSupported` 。</span><span class="sxs-lookup"><span data-stu-id="6d058-130">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="6d058-131">功能生成的建议向审阅者显示，其中一 `Approve` 个或 `Deny` `NotAvailable` 。</span><span class="sxs-lookup"><span data-stu-id="6d058-131">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="6d058-132">此外，可能会存在其他属性，具体取决于对象类型所决定访问权限的对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6d058-132">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="6d058-133">例如，如果访问评审决定是特定用户的组成员身份或应用程序访问权限，则可能会删除其访问权限的用户通过以下属性进行标识：</span><span class="sxs-lookup"><span data-stu-id="6d058-133">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="6d058-134">属性</span><span class="sxs-lookup"><span data-stu-id="6d058-134">Property</span></span>                        | <span data-ttu-id="6d058-135">类型</span><span class="sxs-lookup"><span data-stu-id="6d058-135">Type</span></span>                         | <span data-ttu-id="6d058-136">说明</span><span class="sxs-lookup"><span data-stu-id="6d058-136">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="6d058-137">已审阅其访问权限的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="6d058-137">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="6d058-138">已显示名称访问权限的用户的登录名。</span><span class="sxs-lookup"><span data-stu-id="6d058-138">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="6d058-139">已审阅其访问权限的用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="6d058-139">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="6d058-140">关系</span><span class="sxs-lookup"><span data-stu-id="6d058-140">Relationships</span></span>

<span data-ttu-id="6d058-141">无。</span><span class="sxs-lookup"><span data-stu-id="6d058-141">None.</span></span>  <span data-ttu-id="6d058-142">可以使用[accessReview](accessreview.md)对象的决策和决策关系从访问评审[](../api/accessreview-listdecisions.md)中检索[](../api/accessreview-listmydecisions.md)此类型的对象。</span><span class="sxs-lookup"><span data-stu-id="6d058-142">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="6d058-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6d058-143">See also</span></span>

| <span data-ttu-id="6d058-144">方法</span><span class="sxs-lookup"><span data-stu-id="6d058-144">Method</span></span>           | <span data-ttu-id="6d058-145">返回类型</span><span class="sxs-lookup"><span data-stu-id="6d058-145">Return Type</span></span>    |<span data-ttu-id="6d058-146">说明</span><span class="sxs-lookup"><span data-stu-id="6d058-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6d058-147">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="6d058-147">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="6d058-148">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6d058-148">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="6d058-149">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="6d058-149">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="6d058-150">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="6d058-150">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="6d058-151">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6d058-151">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="6d058-152">作为审阅者，获取我有关 accessReview 的决定。</span><span class="sxs-lookup"><span data-stu-id="6d058-152">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d058-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d058-153">JSON representation</span></span>

<span data-ttu-id="6d058-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d058-154">Here is a JSON representation of the resource.</span></span>

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


