---
title: 删除 accessReview 审阅者
description: '在 Azure AD 访问评论功能中，更新要删除的用户审阅者作为现有 accessReview 对象。  此操作仅允许尚未完成，访问审阅和仅访问审阅显式指定审阅者的位置。 此操作不允许用户在其中查看他们自己的访问，访问审阅，不应在其中为审阅者分配组的所有者访问审阅。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 84bf3d973820067e0d4561e9647f688c025d957f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956687"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="ffe6f-105">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="ffe6f-105">Remove accessReview reviewer</span></span>

> <span data-ttu-id="ffe6f-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ffe6f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffe6f-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ffe6f-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ffe6f-108">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，更新要删除的用户审阅者作为现有[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ffe6f-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="ffe6f-109">此操作仅允许尚未完成，访问审阅和仅访问审阅显式指定审阅者的位置。</span><span class="sxs-lookup"><span data-stu-id="ffe6f-109">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="ffe6f-110">此操作不允许用户在其中查看他们自己的访问，访问审阅，不应在其中为审阅者分配组的所有者访问审阅。</span><span class="sxs-lookup"><span data-stu-id="ffe6f-110">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="ffe6f-111">权限</span><span class="sxs-lookup"><span data-stu-id="ffe6f-111">Permissions</span></span>
<span data-ttu-id="ffe6f-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ffe6f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffe6f-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="ffe6f-114">Permission type</span></span>                        | <span data-ttu-id="ffe6f-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ffe6f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffe6f-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ffe6f-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="ffe6f-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffe6f-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="ffe6f-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ffe6f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffe6f-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffe6f-119">Not supported.</span></span> |
|<span data-ttu-id="ffe6f-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="ffe6f-120">Application</span></span>                            | <span data-ttu-id="ffe6f-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="ffe6f-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffe6f-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ffe6f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="ffe6f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ffe6f-123">Request headers</span></span>
| <span data-ttu-id="ffe6f-124">名称</span><span class="sxs-lookup"><span data-stu-id="ffe6f-124">Name</span></span>         | <span data-ttu-id="ffe6f-125">类型</span><span class="sxs-lookup"><span data-stu-id="ffe6f-125">Type</span></span>        | <span data-ttu-id="ffe6f-126">说明</span><span class="sxs-lookup"><span data-stu-id="ffe6f-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ffe6f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffe6f-127">Authorization</span></span> | <span data-ttu-id="ffe6f-128">string</span><span class="sxs-lookup"><span data-stu-id="ffe6f-128">string</span></span> | <span data-ttu-id="ffe6f-129">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="ffe6f-129">Bearer \{token\}.</span></span> <span data-ttu-id="ffe6f-130">必需。</span><span class="sxs-lookup"><span data-stu-id="ffe6f-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffe6f-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="ffe6f-131">Request body</span></span>
<span data-ttu-id="ffe6f-132">应提供没有请求正文。</span><span class="sxs-lookup"><span data-stu-id="ffe6f-132">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="ffe6f-133">响应</span><span class="sxs-lookup"><span data-stu-id="ffe6f-133">Response</span></span>
<span data-ttu-id="ffe6f-134">如果成功，则此方法将返回 200 系列响应代码。</span><span class="sxs-lookup"><span data-stu-id="ffe6f-134">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="ffe6f-135">示例</span><span class="sxs-lookup"><span data-stu-id="ffe6f-135">Example</span></span>

<span data-ttu-id="ffe6f-136">这是更新一次性 （不) 访问回顾删除不必要的审阅者的示例。</span><span class="sxs-lookup"><span data-stu-id="ffe6f-136">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="ffe6f-137">请求</span><span class="sxs-lookup"><span data-stu-id="ffe6f-137">Request</span></span>
<span data-ttu-id="ffe6f-138">在请求 URL 中，提供 accessReview 对象的 id，然后用户对象的 id。</span><span class="sxs-lookup"><span data-stu-id="ffe6f-138">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers('006111db-0810-4494-a6df-904d368bd81b')

```

##### <a name="response"></a><span data-ttu-id="ffe6f-139">响应</span><span class="sxs-lookup"><span data-stu-id="ffe6f-139">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!-- {
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
