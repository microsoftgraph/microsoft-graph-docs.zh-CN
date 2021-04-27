---
title: 应用 accessReview
description: '在 Azure AD 访问评审功能中，应用已完成的 accessReview 的决策。  目标对象可以是一次性访问评审，也可以作为定期访问评审的实例。  '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b590b741915aaf9ef901ee51e2eb11d43f9b439f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048531"
---
# <a name="apply-accessreview"></a><span data-ttu-id="fe5f7-104">应用 accessReview</span><span class="sxs-lookup"><span data-stu-id="fe5f7-104">Apply accessReview</span></span>

<span data-ttu-id="fe5f7-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe5f7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe5f7-106">在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，应用已完成 [的 accessReview 的决策](../resources/accessreview.md)。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="fe5f7-107">目标对象可以是一次性访问评审，也可以作为定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="fe5f7-108">完成访问评审后，无论是因为到达结束日期，还是管理员手动停止了访问评审，并且未针对该评审配置自动应用，您可以调用 Apply 以应用更改。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-108">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="fe5f7-109">在应用发生之前，删除访问权限的决策不会显示在源资源上，例如，用户保留其组成员身份。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-109">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="fe5f7-110">通过调用 apply，审阅结果通过更新组或应用程序实现。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-110">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="fe5f7-111">如果在审查中拒绝用户访问，当管理员调用此 API 时，Azure AD 将删除其成员身份或应用程序分配。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-111">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="fe5f7-112">完成访问评审并配置自动应用后，检查的状态会从"已完成"更改为"中间"状态，最后将更改为"已应用"状态。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-112">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="fe5f7-113">你应该会看到拒绝的用户（如果有）在几分钟内从资源组成员身份或应用分配中删除。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-113">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="fe5f7-114">配置的自动应用评审或选择应用对源自本地目录或动态组的组没有影响。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-114">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="fe5f7-115">如果要更改源自本地的组，请下载结果，将这些更改应用到该目录中该组的表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-115">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="fe5f7-116">权限</span><span class="sxs-lookup"><span data-stu-id="fe5f7-116">Permissions</span></span>
<span data-ttu-id="fe5f7-p106">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe5f7-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe5f7-119">Permission type</span></span>                        | <span data-ttu-id="fe5f7-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe5f7-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe5f7-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe5f7-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe5f7-122">AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe5f7-122">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="fe5f7-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe5f7-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe5f7-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-124">Not supported.</span></span> |
|<span data-ttu-id="fe5f7-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe5f7-125">Application</span></span>                            | <span data-ttu-id="fe5f7-126">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="fe5f7-126">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe5f7-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe5f7-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/applyDecisions
```
## <a name="request-headers"></a><span data-ttu-id="fe5f7-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe5f7-128">Request headers</span></span>
| <span data-ttu-id="fe5f7-129">名称</span><span class="sxs-lookup"><span data-stu-id="fe5f7-129">Name</span></span>         | <span data-ttu-id="fe5f7-130">类型</span><span class="sxs-lookup"><span data-stu-id="fe5f7-130">Type</span></span>        | <span data-ttu-id="fe5f7-131">说明</span><span class="sxs-lookup"><span data-stu-id="fe5f7-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fe5f7-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe5f7-132">Authorization</span></span> | <span data-ttu-id="fe5f7-133">string</span><span class="sxs-lookup"><span data-stu-id="fe5f7-133">string</span></span> | <span data-ttu-id="fe5f7-p107">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-p107">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe5f7-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe5f7-136">Request body</span></span>
<span data-ttu-id="fe5f7-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-137">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="fe5f7-138">响应</span><span class="sxs-lookup"><span data-stu-id="fe5f7-138">Response</span></span>
<span data-ttu-id="fe5f7-p108">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-p108">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe5f7-141">示例</span><span class="sxs-lookup"><span data-stu-id="fe5f7-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe5f7-142">请求</span><span class="sxs-lookup"><span data-stu-id="fe5f7-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fe5f7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe5f7-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/applyDecisions
```
# <a name="c"></a>[<span data-ttu-id="fe5f7-144">C#</span><span class="sxs-lookup"><span data-stu-id="fe5f7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/apply-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe5f7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe5f7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/apply-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe5f7-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe5f7-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/apply-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe5f7-147">Java</span><span class="sxs-lookup"><span data-stu-id="fe5f7-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/apply-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="fe5f7-148">响应</span><span class="sxs-lookup"><span data-stu-id="fe5f7-148">Response</span></span>
><span data-ttu-id="fe5f7-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fe5f7-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="fe5f7-150">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fe5f7-150">See also</span></span>

- [<span data-ttu-id="fe5f7-151">如何完成访问评审</span><span class="sxs-lookup"><span data-stu-id="fe5f7-151">How to complete an access review</span></span>](/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)
