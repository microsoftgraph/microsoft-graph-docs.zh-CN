---
title: accessReviewDecision 资源类型
description: 在 Azure AD 中访问审阅功能，`accessReviewDecision`代表 Azure AD 访问检查决策的特定实体的访问。  内访问审阅或定期访问回顾实例，还有一`accessReviewDecision`每个已审阅的用户。  例如，如果组具有两个来宾和一个非访客成员，作为来宾访问审阅执行为该组，然后将两个访问审阅决策对象。  如果审阅者更改其决策，或其他审阅者重写它们，则`accessReviewDecision`更新。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b6b10a53726e12c37a598f8df735a3f70174c807
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977554"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="d3584-106">accessReviewDecision 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3584-106">accessReviewDecision resource type</span></span>

> <span data-ttu-id="d3584-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d3584-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3584-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d3584-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d3584-109">在 Azure AD[访问审阅](accessreviews-root.md)功能中，`accessReviewDecision`代表 Azure AD 访问检查决策的特定实体的访问。</span><span class="sxs-lookup"><span data-stu-id="d3584-109">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="d3584-110">内访问审阅或定期访问回顾实例，还有一`accessReviewDecision`每个已审阅的用户。</span><span class="sxs-lookup"><span data-stu-id="d3584-110">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="d3584-111">例如，如果组具有两个来宾和一个非访客成员，作为来宾访问审阅执行为该组，然后将两个访问审阅决策对象。</span><span class="sxs-lookup"><span data-stu-id="d3584-111">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="d3584-112">如果审阅者更改其决策，或其他审阅者重写它们，则`accessReviewDecision`更新。</span><span class="sxs-lookup"><span data-stu-id="d3584-112">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="d3584-113">方法</span><span class="sxs-lookup"><span data-stu-id="d3584-113">Methods</span></span>

<span data-ttu-id="d3584-114">无。</span><span class="sxs-lookup"><span data-stu-id="d3584-114">None.</span></span>  <span data-ttu-id="d3584-115">访问查看初始化，并不能删除时，此类型的对象会自动创建功能。</span><span class="sxs-lookup"><span data-stu-id="d3584-115">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="d3584-116">它们可以使用的[决策](../api/accessreview-listdecisions.md)和[mydecisions](../api/accessreview-listmydecisions.md)关系访问查看从检索。</span><span class="sxs-lookup"><span data-stu-id="d3584-116">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="d3584-117">属性</span><span class="sxs-lookup"><span data-stu-id="d3584-117">Properties</span></span>

<span data-ttu-id="d3584-118">下表说明了此类型的对象的基本属性。</span><span class="sxs-lookup"><span data-stu-id="d3584-118">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="d3584-119">属性</span><span class="sxs-lookup"><span data-stu-id="d3584-119">Property</span></span>                        | <span data-ttu-id="d3584-120">类型</span><span class="sxs-lookup"><span data-stu-id="d3584-120">Type</span></span>                         | <span data-ttu-id="d3584-121">Description</span><span class="sxs-lookup"><span data-stu-id="d3584-121">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="d3584-122">内访问审阅决策的 id。</span><span class="sxs-lookup"><span data-stu-id="d3584-122">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="d3584-123">功能生成访问审阅的 id。</span><span class="sxs-lookup"><span data-stu-id="d3584-123">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="d3584-124">userIdentity</span><span class="sxs-lookup"><span data-stu-id="d3584-124">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="d3584-125">审阅者的标识。</span><span class="sxs-lookup"><span data-stu-id="d3584-125">The identity of the reviewer.</span></span>                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="d3584-126">提供的日期和时间，此最新的审阅访问权限。</span><span class="sxs-lookup"><span data-stu-id="d3584-126">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="d3584-127">审阅结果。</span><span class="sxs-lookup"><span data-stu-id="d3584-127">The result of the review.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="d3584-128">审阅者的业务理由，如果提供。</span><span class="sxs-lookup"><span data-stu-id="d3584-128">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="d3584-129">userIdentity</span><span class="sxs-lookup"><span data-stu-id="d3584-129">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="d3584-130">审阅完成后，如果已手动应用的结果，应用决策的用户的用户标识。</span><span class="sxs-lookup"><span data-stu-id="d3584-130">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span>                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="d3584-131">日期和时间时应用的审阅决策。</span><span class="sxs-lookup"><span data-stu-id="d3584-131">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="d3584-132">应用的决策，之一的结果`NotApplied`， `Success`， `Failed`，`NotFound`或`NotSupported`。</span><span class="sxs-lookup"><span data-stu-id="d3584-132">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="d3584-133">显示给审阅者，之一功能-生成建议`Approve`，`Deny`或`NotAvailable`。</span><span class="sxs-lookup"><span data-stu-id="d3584-133">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="d3584-134">此外，其他属性可能会出现根据拥有已决定的访问权限的对象的对象类型。</span><span class="sxs-lookup"><span data-stu-id="d3584-134">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="d3584-135">例如，如果访问检查决策为特定用户的组成员身份或应用程序访问，可能要让他们要删除的访问权限的用户被标识通过这些属性：</span><span class="sxs-lookup"><span data-stu-id="d3584-135">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="d3584-136">属性</span><span class="sxs-lookup"><span data-stu-id="d3584-136">Property</span></span>                        | <span data-ttu-id="d3584-137">类型</span><span class="sxs-lookup"><span data-stu-id="d3584-137">Type</span></span>                         | <span data-ttu-id="d3584-138">Description</span><span class="sxs-lookup"><span data-stu-id="d3584-138">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="d3584-139">已检查其访问权限的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="d3584-139">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="d3584-140">已检查其访问权限的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d3584-140">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="d3584-141">已检查其访问权限的用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="d3584-141">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="d3584-142">Relationships</span><span class="sxs-lookup"><span data-stu-id="d3584-142">Relationships</span></span>

<span data-ttu-id="d3584-143">无。</span><span class="sxs-lookup"><span data-stu-id="d3584-143">None.</span></span>  <span data-ttu-id="d3584-144">可以使用[accessReview](accessreview.md)对象的[决策](../api/accessreview-listdecisions.md)和[mydecisions](../api/accessreview-listmydecisions.md)关系访问查看从检索此类型的对象。</span><span class="sxs-lookup"><span data-stu-id="d3584-144">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="d3584-145">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d3584-145">See also</span></span>

| <span data-ttu-id="d3584-146">方法</span><span class="sxs-lookup"><span data-stu-id="d3584-146">Method</span></span>           | <span data-ttu-id="d3584-147">返回类型</span><span class="sxs-lookup"><span data-stu-id="d3584-147">Return Type</span></span>    |<span data-ttu-id="d3584-148">说明</span><span class="sxs-lookup"><span data-stu-id="d3584-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d3584-149">列表 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="d3584-149">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="d3584-150">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="d3584-150">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="d3584-151">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="d3584-151">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="d3584-152">列出我 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="d3584-152">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="d3584-153">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="d3584-153">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="d3584-154">审阅者，以获取 accessReview 我决策。</span><span class="sxs-lookup"><span data-stu-id="d3584-154">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3584-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3584-155">JSON representation</span></span>

<span data-ttu-id="d3584-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3584-156">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
