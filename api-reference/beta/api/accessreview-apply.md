---
title: 应用 accessReview
description: '在 Azure AD 中访问评论功能、 apply 完成 accessReview 的决策。  目标对象可以是一次性访问回顾或定期访问评审的实例。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9612f3bcb8a032ee32cd7b058d3f21950c9b120f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512211"
---
# <a name="apply-accessreview"></a><span data-ttu-id="eaee1-104">应用 accessReview</span><span class="sxs-lookup"><span data-stu-id="eaee1-104">Apply accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaee1-105">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能应用完成[accessReview](../resources/accessreview.md)的决策。</span><span class="sxs-lookup"><span data-stu-id="eaee1-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="eaee1-106">目标对象可以是一次性访问回顾或定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="eaee1-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="eaee1-107">访问审阅完毕后，或者因为它到达的结束日期或管理员手动停止，将自动应用未配置供审阅，您可以调用应用，以应用所做的更改。</span><span class="sxs-lookup"><span data-stu-id="eaee1-107">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="eaee1-108">应用，发生此事件，直到要删除的访问权限的决定不显示对源资源，用户例如保留其组成员身份。</span><span class="sxs-lookup"><span data-stu-id="eaee1-108">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="eaee1-109">通过调用应用，由更新的组或应用程序实现的审阅结果。</span><span class="sxs-lookup"><span data-stu-id="eaee1-109">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="eaee1-110">如果用户的访问被拒绝在审阅中，当管理员调用此 API，Azure AD 中删除其成员身份或应用程序的工作分配。</span><span class="sxs-lookup"><span data-stu-id="eaee1-110">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="eaee1-111">访问查看已完成，并自动应用之后进行配置，然后查看的状态将从已完成通过中间状态更改和最后将更改为状态应用。</span><span class="sxs-lookup"><span data-stu-id="eaee1-111">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="eaee1-112">您应该会看到拒绝的用户，如果要删除资源中的任何组成员身份或应用程序的工作分配，请过几分钟。</span><span class="sxs-lookup"><span data-stu-id="eaee1-112">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="eaee1-113">配置的自动应用审阅，或选择应用不会影响的本地目录中的组或动态组。</span><span class="sxs-lookup"><span data-stu-id="eaee1-113">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="eaee1-114">如果您想要更改组的内部部署，下载结果并将这些更改应用于该目录中的组的表示形式。</span><span class="sxs-lookup"><span data-stu-id="eaee1-114">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="eaee1-115">权限</span><span class="sxs-lookup"><span data-stu-id="eaee1-115">Permissions</span></span>
<span data-ttu-id="eaee1-p106">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eaee1-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaee1-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="eaee1-118">Permission type</span></span>                        | <span data-ttu-id="eaee1-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eaee1-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eaee1-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eaee1-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="eaee1-121">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaee1-121">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="eaee1-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eaee1-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaee1-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="eaee1-123">Not supported.</span></span> |
|<span data-ttu-id="eaee1-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="eaee1-124">Application</span></span>                            | <span data-ttu-id="eaee1-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="eaee1-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eaee1-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eaee1-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="eaee1-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="eaee1-127">Request headers</span></span>
| <span data-ttu-id="eaee1-128">名称</span><span class="sxs-lookup"><span data-stu-id="eaee1-128">Name</span></span>         | <span data-ttu-id="eaee1-129">类型</span><span class="sxs-lookup"><span data-stu-id="eaee1-129">Type</span></span>        | <span data-ttu-id="eaee1-130">说明</span><span class="sxs-lookup"><span data-stu-id="eaee1-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="eaee1-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaee1-131">Authorization</span></span> | <span data-ttu-id="eaee1-132">string</span><span class="sxs-lookup"><span data-stu-id="eaee1-132">string</span></span> | <span data-ttu-id="eaee1-133">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="eaee1-133">Bearer \{token\}.</span></span> <span data-ttu-id="eaee1-134">必需。</span><span class="sxs-lookup"><span data-stu-id="eaee1-134">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eaee1-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="eaee1-135">Request body</span></span>
<span data-ttu-id="eaee1-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eaee1-136">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="eaee1-137">响应</span><span class="sxs-lookup"><span data-stu-id="eaee1-137">Response</span></span>
<span data-ttu-id="eaee1-p108">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="eaee1-p108">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="see-also"></a><span data-ttu-id="eaee1-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="eaee1-140">See also</span></span>

- [<span data-ttu-id="eaee1-141">如何完成访问审阅</span><span class="sxs-lookup"><span data-stu-id="eaee1-141">How to complete an access review</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a><span data-ttu-id="eaee1-142">示例</span><span class="sxs-lookup"><span data-stu-id="eaee1-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eaee1-143">请求</span><span class="sxs-lookup"><span data-stu-id="eaee1-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/applyDecisions()
```
##### <a name="response"></a><span data-ttu-id="eaee1-144">响应</span><span class="sxs-lookup"><span data-stu-id="eaee1-144">Response</span></span>
><span data-ttu-id="eaee1-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="eaee1-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/accessreview-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
