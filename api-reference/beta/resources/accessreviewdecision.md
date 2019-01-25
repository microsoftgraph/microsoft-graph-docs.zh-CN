---
title: accessReviewDecision 资源类型
description: 在 Azure AD 中访问审阅功能，`accessReviewDecision`代表 Azure AD 访问检查决策的特定实体的访问。  内访问审阅或定期访问回顾实例，还有一`accessReviewDecision`每个已审阅的用户。  例如，如果组具有两个来宾和一个非访客成员，作为来宾访问审阅执行为该组，然后将两个访问审阅决策对象。  如果审阅者更改其决策，或其他审阅者重写它们，则`accessReviewDecision`更新。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9642c8a51e4e9efe1a1748243b0e24aeff07cfa0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517398"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="6ea21-106">accessReviewDecision 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ea21-106">accessReviewDecision resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ea21-107">在 Azure AD[访问审阅](accessreviews-root.md)功能中，`accessReviewDecision`代表 Azure AD 访问检查决策的特定实体的访问。</span><span class="sxs-lookup"><span data-stu-id="6ea21-107">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="6ea21-108">内访问审阅或定期访问回顾实例，还有一`accessReviewDecision`每个已审阅的用户。</span><span class="sxs-lookup"><span data-stu-id="6ea21-108">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="6ea21-109">例如，如果组具有两个来宾和一个非访客成员，作为来宾访问审阅执行为该组，然后将两个访问审阅决策对象。</span><span class="sxs-lookup"><span data-stu-id="6ea21-109">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="6ea21-110">如果审阅者更改其决策，或其他审阅者重写它们，则`accessReviewDecision`更新。</span><span class="sxs-lookup"><span data-stu-id="6ea21-110">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="6ea21-111">方法</span><span class="sxs-lookup"><span data-stu-id="6ea21-111">Methods</span></span>

<span data-ttu-id="6ea21-112">无。</span><span class="sxs-lookup"><span data-stu-id="6ea21-112">None.</span></span>  <span data-ttu-id="6ea21-113">访问查看初始化，并不能删除时，此类型的对象会自动创建功能。</span><span class="sxs-lookup"><span data-stu-id="6ea21-113">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="6ea21-114">它们可以使用的[决策](../api/accessreview-listdecisions.md)和[mydecisions](../api/accessreview-listmydecisions.md)关系访问查看从检索。</span><span class="sxs-lookup"><span data-stu-id="6ea21-114">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="6ea21-115">属性</span><span class="sxs-lookup"><span data-stu-id="6ea21-115">Properties</span></span>

<span data-ttu-id="6ea21-116">下表说明了此类型的对象的基本属性。</span><span class="sxs-lookup"><span data-stu-id="6ea21-116">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="6ea21-117">属性</span><span class="sxs-lookup"><span data-stu-id="6ea21-117">Property</span></span>                        | <span data-ttu-id="6ea21-118">类型</span><span class="sxs-lookup"><span data-stu-id="6ea21-118">Type</span></span>                         | <span data-ttu-id="6ea21-119">说明</span><span class="sxs-lookup"><span data-stu-id="6ea21-119">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="6ea21-120">内访问审阅决策的 id。</span><span class="sxs-lookup"><span data-stu-id="6ea21-120">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="6ea21-121">功能生成访问审阅的 id。</span><span class="sxs-lookup"><span data-stu-id="6ea21-121">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="6ea21-122">userIdentity</span><span class="sxs-lookup"><span data-stu-id="6ea21-122">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="6ea21-123">审阅者的标识。</span><span class="sxs-lookup"><span data-stu-id="6ea21-123">The identity of the reviewer.</span></span>                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="6ea21-124">提供的日期和时间，此最新的审阅访问权限。</span><span class="sxs-lookup"><span data-stu-id="6ea21-124">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="6ea21-125">审阅结果。</span><span class="sxs-lookup"><span data-stu-id="6ea21-125">The result of the review.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="6ea21-126">审阅者的业务理由，如果提供。</span><span class="sxs-lookup"><span data-stu-id="6ea21-126">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="6ea21-127">userIdentity</span><span class="sxs-lookup"><span data-stu-id="6ea21-127">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="6ea21-128">审阅完成后，如果已手动应用的结果，应用决策的用户的用户标识。</span><span class="sxs-lookup"><span data-stu-id="6ea21-128">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span>                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="6ea21-129">日期和时间时应用的审阅决策。</span><span class="sxs-lookup"><span data-stu-id="6ea21-129">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="6ea21-130">应用的决策，之一的结果`NotApplied`， `Success`， `Failed`，`NotFound`或`NotSupported`。</span><span class="sxs-lookup"><span data-stu-id="6ea21-130">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="6ea21-131">显示给审阅者，之一功能-生成建议`Approve`，`Deny`或`NotAvailable`。</span><span class="sxs-lookup"><span data-stu-id="6ea21-131">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="6ea21-132">此外，其他属性可能会出现根据拥有已决定的访问权限的对象的对象类型。</span><span class="sxs-lookup"><span data-stu-id="6ea21-132">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="6ea21-133">例如，如果访问检查决策为特定用户的组成员身份或应用程序访问，可能要让他们要删除的访问权限的用户被标识通过这些属性：</span><span class="sxs-lookup"><span data-stu-id="6ea21-133">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="6ea21-134">属性</span><span class="sxs-lookup"><span data-stu-id="6ea21-134">Property</span></span>                        | <span data-ttu-id="6ea21-135">类型</span><span class="sxs-lookup"><span data-stu-id="6ea21-135">Type</span></span>                         | <span data-ttu-id="6ea21-136">说明</span><span class="sxs-lookup"><span data-stu-id="6ea21-136">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="6ea21-137">已检查其访问权限的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="6ea21-137">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="6ea21-138">已检查其访问权限的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="6ea21-138">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="6ea21-139">已检查其访问权限的用户的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="6ea21-139">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="6ea21-140">关系</span><span class="sxs-lookup"><span data-stu-id="6ea21-140">Relationships</span></span>

<span data-ttu-id="6ea21-141">无。</span><span class="sxs-lookup"><span data-stu-id="6ea21-141">None.</span></span>  <span data-ttu-id="6ea21-142">可以使用[accessReview](accessreview.md)对象的[决策](../api/accessreview-listdecisions.md)和[mydecisions](../api/accessreview-listmydecisions.md)关系访问查看从检索此类型的对象。</span><span class="sxs-lookup"><span data-stu-id="6ea21-142">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="6ea21-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6ea21-143">See also</span></span>

| <span data-ttu-id="6ea21-144">方法</span><span class="sxs-lookup"><span data-stu-id="6ea21-144">Method</span></span>           | <span data-ttu-id="6ea21-145">返回类型</span><span class="sxs-lookup"><span data-stu-id="6ea21-145">Return Type</span></span>    |<span data-ttu-id="6ea21-146">说明</span><span class="sxs-lookup"><span data-stu-id="6ea21-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6ea21-147">列表 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="6ea21-147">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="6ea21-148">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="6ea21-148">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="6ea21-149">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="6ea21-149">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="6ea21-150">列出我 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="6ea21-150">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="6ea21-151">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="6ea21-151">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="6ea21-152">审阅者，以获取 accessReview 我决策。</span><span class="sxs-lookup"><span data-stu-id="6ea21-152">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ea21-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ea21-153">JSON representation</span></span>

<span data-ttu-id="6ea21-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ea21-154">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreviewdecision.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
