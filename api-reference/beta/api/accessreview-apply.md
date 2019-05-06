---
title: 应用 accessReview
description: '在 "Azure AD 访问评论" 功能中, 应用已完成 accessReview 的决策。  目标对象可以是一次性访问评审, 也可以是定期访问评审的实例。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0e160f5247a2725cb8b675b90a36fff2d6759a60
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586252"
---
# <a name="apply-accessreview"></a><span data-ttu-id="13117-104">应用 accessReview</span><span class="sxs-lookup"><span data-stu-id="13117-104">Apply accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13117-105">在 "Azure AD[访问评论](../resources/accessreviews-root.md)" 功能中, 应用已完成[accessReview](../resources/accessreview.md)的决策。</span><span class="sxs-lookup"><span data-stu-id="13117-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="13117-106">目标对象可以是一次性访问评审, 也可以是定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="13117-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="13117-107">在访问审核完成后, 因为它已达到结束日期或管理员手动停止, 且未为审阅配置自动应用, 所以您可以调用 Apply 以应用所做的更改。</span><span class="sxs-lookup"><span data-stu-id="13117-107">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="13117-108">在应用之前, 不会在源资源上显示有关删除访问权限的决策, 因此实例的用户将保留其组成员身份。</span><span class="sxs-lookup"><span data-stu-id="13117-108">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="13117-109">通过调用 apply, 评审的结果通过更新组或应用程序来实现。</span><span class="sxs-lookup"><span data-stu-id="13117-109">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="13117-110">如果在审阅中拒绝了用户的访问权限, 则当管理员调用此 API 时, Azure AD 将删除其成员身份或应用程序分配。</span><span class="sxs-lookup"><span data-stu-id="13117-110">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="13117-111">在访问评审完成且配置了自动应用后, 评审的状态将从 "已完成" 更改为 "中间状态", 最后将更改为 "已应用的状态"。</span><span class="sxs-lookup"><span data-stu-id="13117-111">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="13117-112">您应该会看到已拒绝的用户 (如果有) 在几分钟内从资源组成员身份或应用分配中删除。</span><span class="sxs-lookup"><span data-stu-id="13117-112">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="13117-113">已配置的自动应用审阅, 或选择 "应用" 不会对源于内部部署目录或动态组的组产生影响。</span><span class="sxs-lookup"><span data-stu-id="13117-113">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="13117-114">如果要更改源于内部部署的组, 请下载结果并将这些更改应用于该目录中的组的表示形式。</span><span class="sxs-lookup"><span data-stu-id="13117-114">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="13117-115">权限</span><span class="sxs-lookup"><span data-stu-id="13117-115">Permissions</span></span>
<span data-ttu-id="13117-p106">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13117-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13117-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="13117-118">Permission type</span></span>                        | <span data-ttu-id="13117-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13117-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="13117-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13117-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="13117-121">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13117-121">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="13117-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13117-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13117-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="13117-123">Not supported.</span></span> |
|<span data-ttu-id="13117-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="13117-124">Application</span></span>                            | <span data-ttu-id="13117-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="13117-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="13117-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13117-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="13117-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="13117-127">Request headers</span></span>
| <span data-ttu-id="13117-128">名称</span><span class="sxs-lookup"><span data-stu-id="13117-128">Name</span></span>         | <span data-ttu-id="13117-129">类型</span><span class="sxs-lookup"><span data-stu-id="13117-129">Type</span></span>        | <span data-ttu-id="13117-130">说明</span><span class="sxs-lookup"><span data-stu-id="13117-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="13117-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="13117-131">Authorization</span></span> | <span data-ttu-id="13117-132">string</span><span class="sxs-lookup"><span data-stu-id="13117-132">string</span></span> | <span data-ttu-id="13117-p107">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="13117-p107">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13117-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="13117-135">Request body</span></span>
<span data-ttu-id="13117-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="13117-136">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="13117-137">响应</span><span class="sxs-lookup"><span data-stu-id="13117-137">Response</span></span>
<span data-ttu-id="13117-p108">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="13117-p108">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="see-also"></a><span data-ttu-id="13117-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="13117-140">See also</span></span>

- [<span data-ttu-id="13117-141">如何完成访问评审</span><span class="sxs-lookup"><span data-stu-id="13117-141">How to complete an access review</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a><span data-ttu-id="13117-142">示例</span><span class="sxs-lookup"><span data-stu-id="13117-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13117-143">请求</span><span class="sxs-lookup"><span data-stu-id="13117-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/applyDecisions
```
##### <a name="response"></a><span data-ttu-id="13117-144">响应</span><span class="sxs-lookup"><span data-stu-id="13117-144">Response</span></span>
><span data-ttu-id="13117-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="13117-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="13117-147">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="13117-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="13117-148">语言</span><span class="sxs-lookup"><span data-stu-id="13117-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/apply_accessReview-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="13117-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="13117-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/apply_accessReview-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/accessreview-apply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-apply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
