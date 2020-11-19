---
title: 更新 accessReviewInstanceDecisionItem
description: 更新调用 user 的现有 accessReviewInstanceDecisionItem 对象是的审阅者。
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2f14ed26169c659354af16963e03e449f246421c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214367"
---
# <a name="update-accessreviewinstancedecisionitem"></a><span data-ttu-id="d5b83-103">更新 accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="d5b83-103">Update accessReviewInstanceDecisionItem</span></span>

<span data-ttu-id="d5b83-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5b83-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5b83-105">更新用户为其审阅者的访问决策（称为 " [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md)"）。</span><span class="sxs-lookup"><span data-stu-id="d5b83-105">Update access decisions, known as [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md), for which the user is the reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="d5b83-106">对 **accessReviewInstanceDecisionItem** 所做的任何更新只能通过呼叫作为父 [accessReviewInstance](../resources/accessreviewinstance.md)的审阅者列出的用户来完成。</span><span class="sxs-lookup"><span data-stu-id="d5b83-106">Any updates made to an **accessReviewInstanceDecisionItem** can only be made by calling users who are listed as reviewer for the parent [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5b83-107">权限</span><span class="sxs-lookup"><span data-stu-id="d5b83-107">Permissions</span></span>
<span data-ttu-id="d5b83-108">若要调用此 API，必须有以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="d5b83-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d5b83-109">不支持对个人 Microsoft 帐户的委派权限。</span><span class="sxs-lookup"><span data-stu-id="d5b83-109">Delegated permissions to personal Microsoft accounts are not supported.</span></span> <span data-ttu-id="d5b83-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5b83-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5b83-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5b83-111">Permission type</span></span>                        | <span data-ttu-id="d5b83-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5b83-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5b83-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5b83-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5b83-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5b83-114">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="d5b83-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5b83-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5b83-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5b83-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5b83-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5b83-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/pendingAccessReviewInstances/{instance-id}/decisions/{decision-id}
```
## <a name="request-headers"></a><span data-ttu-id="d5b83-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5b83-118">Request headers</span></span>
| <span data-ttu-id="d5b83-119">名称</span><span class="sxs-lookup"><span data-stu-id="d5b83-119">Name</span></span>         | <span data-ttu-id="d5b83-120">说明</span><span class="sxs-lookup"><span data-stu-id="d5b83-120">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="d5b83-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5b83-121">Authorization</span></span>|<span data-ttu-id="d5b83-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5b83-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="d5b83-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="d5b83-124">Content-type</span></span> | <span data-ttu-id="d5b83-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d5b83-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5b83-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5b83-127">Request body</span></span>
<span data-ttu-id="d5b83-128">下表显示了接受更新的属性 `accessReviewInstanceDecisionItem` 。</span><span class="sxs-lookup"><span data-stu-id="d5b83-128">The following table shows the properties accepted to update an `accessReviewInstanceDecisionItem`.</span></span>

| <span data-ttu-id="d5b83-129">属性</span><span class="sxs-lookup"><span data-stu-id="d5b83-129">Property</span></span>     | <span data-ttu-id="d5b83-130">类型</span><span class="sxs-lookup"><span data-stu-id="d5b83-130">Type</span></span>       | <span data-ttu-id="d5b83-131">说明</span><span class="sxs-lookup"><span data-stu-id="d5b83-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d5b83-132">权</span><span class="sxs-lookup"><span data-stu-id="d5b83-132">decision</span></span>  | <span data-ttu-id="d5b83-133">String</span><span class="sxs-lookup"><span data-stu-id="d5b83-133">String</span></span> | <span data-ttu-id="d5b83-134">正在审阅的实体的访问决定。</span><span class="sxs-lookup"><span data-stu-id="d5b83-134">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="d5b83-135">可能的值是： `Approve` `Deny` `NotReviewed` `DontKnow` 。</span><span class="sxs-lookup"><span data-stu-id="d5b83-135">Possible values are: `Approve` `Deny` `NotReviewed` `DontKnow`.</span></span> <span data-ttu-id="d5b83-136">必需。</span><span class="sxs-lookup"><span data-stu-id="d5b83-136">Required.</span></span>  |
|  <span data-ttu-id="d5b83-137">合理化</span><span class="sxs-lookup"><span data-stu-id="d5b83-137">justification</span></span> | <span data-ttu-id="d5b83-138">String</span><span class="sxs-lookup"><span data-stu-id="d5b83-138">String</span></span> | <span data-ttu-id="d5b83-139">向管理员提供的审阅的上下文。</span><span class="sxs-lookup"><span data-stu-id="d5b83-139">Context of the review provided to admins.</span></span> <span data-ttu-id="d5b83-140">如果 justificationRequiredOnApproval 在 accessReviewScheduleDefinition 上为 True，则为必需项。</span><span class="sxs-lookup"><span data-stu-id="d5b83-140">Required if justificationRequiredOnApproval is True on the accessReviewScheduleDefinition.</span></span>  |

## <a name="response"></a><span data-ttu-id="d5b83-141">响应</span><span class="sxs-lookup"><span data-stu-id="d5b83-141">Response</span></span>
<span data-ttu-id="d5b83-142">如果成功，此方法将返回 `204, NoContent` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="d5b83-142">If successful, this method returns a `204, NoContent` response code and no response body.</span></span>

### <a name="request"></a><span data-ttu-id="d5b83-143">请求</span><span class="sxs-lookup"><span data-stu-id="d5b83-143">Request</span></span>
## <a name="examples"></a><span data-ttu-id="d5b83-144">示例</span><span class="sxs-lookup"><span data-stu-id="d5b83-144">Examples</span></span>

<span data-ttu-id="d5b83-145">下面的示例展示了如何为由获取的用户审批访问 `accessReviewInstanceDecisionItem` 。</span><span class="sxs-lookup"><span data-stu-id="d5b83-145">This is an example of approving access for a user represented by an `accessReviewInstanceDecisionItem`.</span></span>


# <a name="http"></a>[<span data-ttu-id="d5b83-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5b83-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/654b34e7-b48f-4772-a2d4-08f1d0dd014c

{
  "decision": "Approve",
  "justification": "I trust this person"
}
```
# <a name="c"></a>[<span data-ttu-id="d5b83-147">C#</span><span class="sxs-lookup"><span data-stu-id="d5b83-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5b83-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5b83-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5b83-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5b83-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5b83-150">Java</span><span class="sxs-lookup"><span data-stu-id="d5b83-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="d5b83-151">响应</span><span class="sxs-lookup"><span data-stu-id="d5b83-151">Response</span></span>
><span data-ttu-id="d5b83-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d5b83-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 Accepted
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewInstanceDecisionItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
