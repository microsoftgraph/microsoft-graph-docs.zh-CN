---
title: accessReviewDecision 资源类型
description: 在 Azure AD access 评论功能中， `accessReviewDecision`表示特定实体的访问的 azure ad 访问审核决策。  在访问评审或定期访问审核实例中，每个审阅的用户都有`accessReviewDecision`一个。  例如，如果一个组有两个来宾，一个非来宾作为成员，并且对该组执行来宾的访问审核，则会有两个访问审核决策对象。  如果审阅者更改`accessReviewDecision`了他们的决定，或另一个审阅者将其覆盖，则会更新。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e92eb6b17b76ac3f8e44404dfbc776463170e0fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508476"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="2e6da-106">accessReviewDecision 资源类型</span><span class="sxs-lookup"><span data-stu-id="2e6da-106">accessReviewDecision resource type</span></span>

<span data-ttu-id="2e6da-107">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2e6da-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e6da-108">在 Azure AD [access 评论](accessreviews-root.md)功能中， `accessReviewDecision`表示特定实体的访问的 azure ad 访问审核决策。</span><span class="sxs-lookup"><span data-stu-id="2e6da-108">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="2e6da-109">在访问评审或定期访问审核实例中，每个审阅的用户都有`accessReviewDecision`一个。</span><span class="sxs-lookup"><span data-stu-id="2e6da-109">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="2e6da-110">例如，如果一个组有两个来宾，一个非来宾作为成员，并且对该组执行来宾的访问审核，则会有两个访问审核决策对象。</span><span class="sxs-lookup"><span data-stu-id="2e6da-110">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="2e6da-111">如果审阅者更改`accessReviewDecision`了他们的决定，或另一个审阅者将其覆盖，则会更新。</span><span class="sxs-lookup"><span data-stu-id="2e6da-111">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="2e6da-112">方法</span><span class="sxs-lookup"><span data-stu-id="2e6da-112">Methods</span></span>

<span data-ttu-id="2e6da-113">无。</span><span class="sxs-lookup"><span data-stu-id="2e6da-113">None.</span></span>  <span data-ttu-id="2e6da-114">此类对象将在 access 评审初始化时自动创建，并且无法删除。</span><span class="sxs-lookup"><span data-stu-id="2e6da-114">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="2e6da-115">可以使用[决策](../api/accessreview-listdecisions.md)和[mydecisions](../api/accessreview-listmydecisions.md)关系从访问审核中检索它们。</span><span class="sxs-lookup"><span data-stu-id="2e6da-115">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="2e6da-116">属性</span><span class="sxs-lookup"><span data-stu-id="2e6da-116">Properties</span></span>

<span data-ttu-id="2e6da-117">此表阐释了此类型对象的基本属性。</span><span class="sxs-lookup"><span data-stu-id="2e6da-117">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="2e6da-118">属性</span><span class="sxs-lookup"><span data-stu-id="2e6da-118">Property</span></span>                        | <span data-ttu-id="2e6da-119">类型</span><span class="sxs-lookup"><span data-stu-id="2e6da-119">Type</span></span>                         | <span data-ttu-id="2e6da-120">说明</span><span class="sxs-lookup"><span data-stu-id="2e6da-120">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="2e6da-121">访问评审中决策的 id。</span><span class="sxs-lookup"><span data-stu-id="2e6da-121">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="2e6da-122">功能生成的访问评审的 id。</span><span class="sxs-lookup"><span data-stu-id="2e6da-122">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="2e6da-123">userIdentity</span><span class="sxs-lookup"><span data-stu-id="2e6da-123">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="2e6da-124">审阅者的标识。</span><span class="sxs-lookup"><span data-stu-id="2e6da-124">The identity of the reviewer.</span></span> <span data-ttu-id="2e6da-125">如果将建议用作审阅，则 userPrincipalName 为空。</span><span class="sxs-lookup"><span data-stu-id="2e6da-125">If the recommendation was used as the review, the userPrincipalName is empty.</span></span>                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="2e6da-126">提供此访问权限最近一次审阅的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2e6da-126">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="2e6da-127">评审`NotReviewed`的结果、 `Deny`、 `DontKnow`或。 `Approve`</span><span class="sxs-lookup"><span data-stu-id="2e6da-127">The result of the review, one of `NotReviewed`, `Deny`, `DontKnow` or `Approve`.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="2e6da-128">审阅者的业务理由（如果提供）。</span><span class="sxs-lookup"><span data-stu-id="2e6da-128">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="2e6da-129">userIdentity</span><span class="sxs-lookup"><span data-stu-id="2e6da-129">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="2e6da-130">当评审完成时，如果手动应用了结果，则为应用决策的用户的用户标识。</span><span class="sxs-lookup"><span data-stu-id="2e6da-130">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span> <span data-ttu-id="2e6da-131">如果已自动应用审阅，则 userPrincipalName 为空。</span><span class="sxs-lookup"><span data-stu-id="2e6da-131">If the review was auto-applied, the userPrincipalName is empty.</span></span>                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="2e6da-132">应用评审决策的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2e6da-132">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="2e6da-133">应用`NotApplied`决策、 `Success` `Failed`、、 `NotFound`或`NotSupported`的结果。</span><span class="sxs-lookup"><span data-stu-id="2e6da-133">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="2e6da-134">向审阅者、 `Approve` `Deny`或`NotAvailable`之一显示的功能生成的建议。</span><span class="sxs-lookup"><span data-stu-id="2e6da-134">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="2e6da-135">此外，还可能会出现其他属性，具体取决于拥有所决定的访问权限的对象的对象类型。</span><span class="sxs-lookup"><span data-stu-id="2e6da-135">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="2e6da-136">例如，如果访问审核决策是特定用户的组成员身份或应用程序访问权限，则可以通过以下属性来标识可能要删除其访问权限的用户：</span><span class="sxs-lookup"><span data-stu-id="2e6da-136">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="2e6da-137">属性</span><span class="sxs-lookup"><span data-stu-id="2e6da-137">Property</span></span>                        | <span data-ttu-id="2e6da-138">类型</span><span class="sxs-lookup"><span data-stu-id="2e6da-138">Type</span></span>                         | <span data-ttu-id="2e6da-139">说明</span><span class="sxs-lookup"><span data-stu-id="2e6da-139">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="2e6da-140">已查看其访问权限的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="2e6da-140">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="2e6da-141">已查看其访问权限的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2e6da-141">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="2e6da-142">已查看其访问权限的用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="2e6da-142">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="2e6da-143">关系</span><span class="sxs-lookup"><span data-stu-id="2e6da-143">Relationships</span></span>

<span data-ttu-id="2e6da-144">无。</span><span class="sxs-lookup"><span data-stu-id="2e6da-144">None.</span></span>  <span data-ttu-id="2e6da-145">通过使用[accessReview](accessreview.md)对象的[决策](../api/accessreview-listdecisions.md)和[mydecisions](../api/accessreview-listmydecisions.md)关系，可以从访问审核中检索此类型的对象。</span><span class="sxs-lookup"><span data-stu-id="2e6da-145">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="2e6da-146">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2e6da-146">See also</span></span>

| <span data-ttu-id="2e6da-147">方法</span><span class="sxs-lookup"><span data-stu-id="2e6da-147">Method</span></span>           | <span data-ttu-id="2e6da-148">返回类型</span><span class="sxs-lookup"><span data-stu-id="2e6da-148">Return Type</span></span>    |<span data-ttu-id="2e6da-149">说明</span><span class="sxs-lookup"><span data-stu-id="2e6da-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2e6da-150">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="2e6da-150">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="2e6da-151">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="2e6da-151">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="2e6da-152">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="2e6da-152">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="2e6da-153">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="2e6da-153">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="2e6da-154">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="2e6da-154">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="2e6da-155">作为审阅者，请 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="2e6da-155">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e6da-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e6da-156">JSON representation</span></span>

<span data-ttu-id="2e6da-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e6da-157">Here is a JSON representation of the resource.</span></span>

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
