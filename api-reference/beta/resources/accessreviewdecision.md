---
title: accessReviewDecision 资源类型
description: 在 Azure AD access 评论功能中， `accessReviewDecision`表示特定实体的访问的 azure ad 访问审核决策。  在访问评审或定期访问审核实例中，每个审阅的用户都有`accessReviewDecision`一个。  例如，如果一个组有两个来宾，一个非来宾作为成员，并且对该组执行来宾的访问审核，则会有两个访问审核决策对象。  如果审阅者更改`accessReviewDecision`了他们的决定，或另一个审阅者将其覆盖，则会更新。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 08a06892892402bee063b532698beeceffd87720
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475593"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="a8f42-106">accessReviewDecision 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8f42-106">accessReviewDecision resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8f42-107">在 Azure AD [access 评论](accessreviews-root.md)功能中， `accessReviewDecision`表示特定实体的访问的 azure ad 访问审核决策。</span><span class="sxs-lookup"><span data-stu-id="a8f42-107">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="a8f42-108">在访问评审或定期访问审核实例中，每个审阅的用户都有`accessReviewDecision`一个。</span><span class="sxs-lookup"><span data-stu-id="a8f42-108">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="a8f42-109">例如，如果一个组有两个来宾，一个非来宾作为成员，并且对该组执行来宾的访问审核，则会有两个访问审核决策对象。</span><span class="sxs-lookup"><span data-stu-id="a8f42-109">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="a8f42-110">如果审阅者更改`accessReviewDecision`了他们的决定，或另一个审阅者将其覆盖，则会更新。</span><span class="sxs-lookup"><span data-stu-id="a8f42-110">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="a8f42-111">方法</span><span class="sxs-lookup"><span data-stu-id="a8f42-111">Methods</span></span>

<span data-ttu-id="a8f42-112">无。</span><span class="sxs-lookup"><span data-stu-id="a8f42-112">None.</span></span>  <span data-ttu-id="a8f42-113">此类对象将在 access 评审初始化时自动创建，并且无法删除。</span><span class="sxs-lookup"><span data-stu-id="a8f42-113">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="a8f42-114">可以使用[决策](../api/accessreview-listdecisions.md)和[mydecisions](../api/accessreview-listmydecisions.md)关系从访问审核中检索它们。</span><span class="sxs-lookup"><span data-stu-id="a8f42-114">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="a8f42-115">属性</span><span class="sxs-lookup"><span data-stu-id="a8f42-115">Properties</span></span>

<span data-ttu-id="a8f42-116">此表阐释了此类型对象的基本属性。</span><span class="sxs-lookup"><span data-stu-id="a8f42-116">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="a8f42-117">属性</span><span class="sxs-lookup"><span data-stu-id="a8f42-117">Property</span></span>                        | <span data-ttu-id="a8f42-118">类型</span><span class="sxs-lookup"><span data-stu-id="a8f42-118">Type</span></span>                         | <span data-ttu-id="a8f42-119">说明</span><span class="sxs-lookup"><span data-stu-id="a8f42-119">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="a8f42-120">访问评审中决策的 id。</span><span class="sxs-lookup"><span data-stu-id="a8f42-120">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="a8f42-121">功能生成的访问评审的 id。</span><span class="sxs-lookup"><span data-stu-id="a8f42-121">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="a8f42-122">userIdentity</span><span class="sxs-lookup"><span data-stu-id="a8f42-122">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="a8f42-123">审阅者的标识。</span><span class="sxs-lookup"><span data-stu-id="a8f42-123">The identity of the reviewer.</span></span> <span data-ttu-id="a8f42-124">如果将建议用作审阅，则 userPrincipalName 为空。</span><span class="sxs-lookup"><span data-stu-id="a8f42-124">If the recommendation was used as the review, the userPrincipalName is empty.</span></span>                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="a8f42-125">提供此访问权限最近一次审阅的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a8f42-125">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="a8f42-126">评审`NotReviewed`的结果、 `Deny`、 `DontKnow`或。 `Approve`</span><span class="sxs-lookup"><span data-stu-id="a8f42-126">The result of the review, one of `NotReviewed`, `Deny`, `DontKnow` or `Approve`.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="a8f42-127">审阅者的业务理由（如果提供）。</span><span class="sxs-lookup"><span data-stu-id="a8f42-127">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="a8f42-128">userIdentity</span><span class="sxs-lookup"><span data-stu-id="a8f42-128">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="a8f42-129">当评审完成时，如果手动应用了结果，则为应用决策的用户的用户标识。</span><span class="sxs-lookup"><span data-stu-id="a8f42-129">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span> <span data-ttu-id="a8f42-130">如果已自动应用审阅，则 userPrincipalName 为空。</span><span class="sxs-lookup"><span data-stu-id="a8f42-130">If the review was auto-applied, the userPrincipalName is empty.</span></span>                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="a8f42-131">应用评审决策的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a8f42-131">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="a8f42-132">应用`NotApplied`决策、 `Success` `Failed`、、 `NotFound`或`NotSupported`的结果。</span><span class="sxs-lookup"><span data-stu-id="a8f42-132">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="a8f42-133">向审阅者、 `Approve` `Deny`或`NotAvailable`之一显示的功能生成的建议。</span><span class="sxs-lookup"><span data-stu-id="a8f42-133">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="a8f42-134">此外，还可能会出现其他属性，具体取决于拥有所决定的访问权限的对象的对象类型。</span><span class="sxs-lookup"><span data-stu-id="a8f42-134">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="a8f42-135">例如，如果访问审核决策是特定用户的组成员身份或应用程序访问权限，则可以通过以下属性来标识可能要删除其访问权限的用户：</span><span class="sxs-lookup"><span data-stu-id="a8f42-135">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="a8f42-136">属性</span><span class="sxs-lookup"><span data-stu-id="a8f42-136">Property</span></span>                        | <span data-ttu-id="a8f42-137">类型</span><span class="sxs-lookup"><span data-stu-id="a8f42-137">Type</span></span>                         | <span data-ttu-id="a8f42-138">说明</span><span class="sxs-lookup"><span data-stu-id="a8f42-138">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="a8f42-139">已查看其访问权限的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="a8f42-139">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="a8f42-140">已查看其访问权限的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a8f42-140">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="a8f42-141">已查看其访问权限的用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="a8f42-141">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="a8f42-142">关系</span><span class="sxs-lookup"><span data-stu-id="a8f42-142">Relationships</span></span>

<span data-ttu-id="a8f42-143">无。</span><span class="sxs-lookup"><span data-stu-id="a8f42-143">None.</span></span>  <span data-ttu-id="a8f42-144">通过使用[accessReview](accessreview.md)对象的[决策](../api/accessreview-listdecisions.md)和[mydecisions](../api/accessreview-listmydecisions.md)关系，可以从访问审核中检索此类型的对象。</span><span class="sxs-lookup"><span data-stu-id="a8f42-144">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="a8f42-145">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a8f42-145">See also</span></span>

| <span data-ttu-id="a8f42-146">方法</span><span class="sxs-lookup"><span data-stu-id="a8f42-146">Method</span></span>           | <span data-ttu-id="a8f42-147">返回类型</span><span class="sxs-lookup"><span data-stu-id="a8f42-147">Return Type</span></span>    |<span data-ttu-id="a8f42-148">说明</span><span class="sxs-lookup"><span data-stu-id="a8f42-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a8f42-149">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="a8f42-149">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="a8f42-150">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="a8f42-150">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="a8f42-151">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="a8f42-151">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="a8f42-152">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="a8f42-152">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="a8f42-153">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="a8f42-153">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="a8f42-154">作为审阅者，请 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="a8f42-154">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8f42-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8f42-155">JSON representation</span></span>

<span data-ttu-id="a8f42-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8f42-156">Here is a JSON representation of the resource.</span></span>

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
