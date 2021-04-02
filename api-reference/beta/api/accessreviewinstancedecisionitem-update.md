---
title: 更新 accessReviewInstanceDecisionItem
description: 更新调用用户是审阅者的现有 accessReviewInstanceDecisionItem 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 913c53927ecc8e436c8d3c63e73d827af5eb4271
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507196"
---
# <a name="update-accessreviewinstancedecisionitem"></a><span data-ttu-id="fc686-103">更新 accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="fc686-103">Update accessReviewInstanceDecisionItem</span></span>

<span data-ttu-id="fc686-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc686-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc686-105">更新访问决策，称为 [accessReviewInstanceDecisionItems，](../resources/accessreviewinstancedecisionitem.md)用户是审阅者。</span><span class="sxs-lookup"><span data-stu-id="fc686-105">Update access decisions, known as [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md), for which the user is the reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="fc686-106">对 **accessReviewInstanceDecisionItem** 进行的任何更新都只能通过调用列为父 [accessReviewInstance](../resources/accessreviewinstance.md)的审阅者的用户进行。</span><span class="sxs-lookup"><span data-stu-id="fc686-106">Any updates made to an **accessReviewInstanceDecisionItem** can only be made by calling users who are listed as reviewer for the parent [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fc686-107">权限</span><span class="sxs-lookup"><span data-stu-id="fc686-107">Permissions</span></span>
<span data-ttu-id="fc686-108">若要调用此 API，需要以下权限之一。</span><span class="sxs-lookup"><span data-stu-id="fc686-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fc686-109">不支持向个人 Microsoft 帐户委派权限。</span><span class="sxs-lookup"><span data-stu-id="fc686-109">Delegated permissions to personal Microsoft accounts are not supported.</span></span> <span data-ttu-id="fc686-110">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc686-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc686-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc686-111">Permission type</span></span>                        | <span data-ttu-id="fc686-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc686-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc686-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc686-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc686-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc686-114">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="fc686-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc686-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc686-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc686-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc686-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc686-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/pendingAccessReviewInstances/{instance-id}/decisions/{decision-id}
```
## <a name="request-headers"></a><span data-ttu-id="fc686-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc686-118">Request headers</span></span>
| <span data-ttu-id="fc686-119">名称</span><span class="sxs-lookup"><span data-stu-id="fc686-119">Name</span></span>         | <span data-ttu-id="fc686-120">说明</span><span class="sxs-lookup"><span data-stu-id="fc686-120">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="fc686-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc686-121">Authorization</span></span>|<span data-ttu-id="fc686-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fc686-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="fc686-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="fc686-124">Content-type</span></span> | <span data-ttu-id="fc686-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="fc686-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc686-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc686-127">Request body</span></span>
<span data-ttu-id="fc686-128">下表显示接受更新 的属性 `accessReviewInstanceDecisionItem` 。</span><span class="sxs-lookup"><span data-stu-id="fc686-128">The following table shows the properties accepted to update an `accessReviewInstanceDecisionItem`.</span></span>

| <span data-ttu-id="fc686-129">属性</span><span class="sxs-lookup"><span data-stu-id="fc686-129">Property</span></span>     | <span data-ttu-id="fc686-130">类型</span><span class="sxs-lookup"><span data-stu-id="fc686-130">Type</span></span>       | <span data-ttu-id="fc686-131">说明</span><span class="sxs-lookup"><span data-stu-id="fc686-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fc686-132">decision</span><span class="sxs-lookup"><span data-stu-id="fc686-132">decision</span></span>  | <span data-ttu-id="fc686-133">字符串</span><span class="sxs-lookup"><span data-stu-id="fc686-133">String</span></span> | <span data-ttu-id="fc686-134">被审阅实体的访问决策。</span><span class="sxs-lookup"><span data-stu-id="fc686-134">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="fc686-135">可能的值是 `Approve` `Deny` `NotReviewed` `DontKnow` ：。</span><span class="sxs-lookup"><span data-stu-id="fc686-135">Possible values are: `Approve` `Deny` `NotReviewed` `DontKnow`.</span></span> <span data-ttu-id="fc686-136">必填。</span><span class="sxs-lookup"><span data-stu-id="fc686-136">Required.</span></span>  |
|  <span data-ttu-id="fc686-137">justification</span><span class="sxs-lookup"><span data-stu-id="fc686-137">justification</span></span> | <span data-ttu-id="fc686-138">字符串</span><span class="sxs-lookup"><span data-stu-id="fc686-138">String</span></span> | <span data-ttu-id="fc686-139">提供给管理员评价的上下文。</span><span class="sxs-lookup"><span data-stu-id="fc686-139">Context of the review provided to admins.</span></span> <span data-ttu-id="fc686-140">如果 accessReviewScheduleDefinition 上的 justificationRequiredOnApproval 为 True，则必需。</span><span class="sxs-lookup"><span data-stu-id="fc686-140">Required if justificationRequiredOnApproval is True on the accessReviewScheduleDefinition.</span></span>  |

## <a name="response"></a><span data-ttu-id="fc686-141">响应</span><span class="sxs-lookup"><span data-stu-id="fc686-141">Response</span></span>
<span data-ttu-id="fc686-142">如果成功，此方法返回 响应 `204, NoContent` 代码，无响应正文。</span><span class="sxs-lookup"><span data-stu-id="fc686-142">If successful, this method returns a `204, NoContent` response code and no response body.</span></span>

### <a name="request"></a><span data-ttu-id="fc686-143">请求</span><span class="sxs-lookup"><span data-stu-id="fc686-143">Request</span></span>
## <a name="examples"></a><span data-ttu-id="fc686-144">示例</span><span class="sxs-lookup"><span data-stu-id="fc686-144">Examples</span></span>

<span data-ttu-id="fc686-145">这是一个批准由 表示的用户的访问的示例 `accessReviewInstanceDecisionItem` 。</span><span class="sxs-lookup"><span data-stu-id="fc686-145">This is an example of approving access for a user represented by an `accessReviewInstanceDecisionItem`.</span></span>



# <a name="http"></a>[<span data-ttu-id="fc686-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc686-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
``` http
PATCH https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/12348410-67f3-4d4c-b946-6989e050be19
Content-Type: application/json
Content-length: 730

{
  "decision": "Approve",
  "justification": "This person is still on my team",
}
```
# <a name="c"></a>[<span data-ttu-id="fc686-147">C#</span><span class="sxs-lookup"><span data-stu-id="fc686-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc686-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc686-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc686-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc686-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc686-150">Java</span><span class="sxs-lookup"><span data-stu-id="fc686-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="fc686-151">响应</span><span class="sxs-lookup"><span data-stu-id="fc686-151">Response</span></span>
><span data-ttu-id="fc686-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fc686-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem"
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
