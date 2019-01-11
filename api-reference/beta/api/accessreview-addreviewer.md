---
title: 添加 accessReview 审阅者
description: '在 Azure AD 访问评论功能中，更新要作为审阅者添加另一个用户现有 accessReview 对象。  此操作仅允许尚未完成，访问审阅和仅访问审阅显式指定审阅者的位置。 此操作不允许用户在其中查看他们自己的访问，访问审阅，不应在其中为审阅者分配组的所有者访问审阅。 '
localization_priority: Normal
ms.openlocfilehash: ab339a6538fc41d7e538c51251302c5e589367f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838764"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="a023d-105">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="a023d-105">Add accessReview reviewer</span></span>

> <span data-ttu-id="a023d-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a023d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a023d-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a023d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a023d-108">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，更新要作为审阅者添加另一个用户现有[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a023d-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="a023d-109">此操作仅允许尚未完成，访问审阅和仅访问审阅显式指定审阅者的位置。</span><span class="sxs-lookup"><span data-stu-id="a023d-109">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="a023d-110">此操作不允许用户在其中查看他们自己的访问，访问审阅，不应在其中为审阅者分配组的所有者访问审阅。</span><span class="sxs-lookup"><span data-stu-id="a023d-110">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="a023d-111">权限</span><span class="sxs-lookup"><span data-stu-id="a023d-111">Permissions</span></span>
<span data-ttu-id="a023d-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a023d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a023d-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="a023d-114">Permission type</span></span>                        | <span data-ttu-id="a023d-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a023d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a023d-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a023d-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="a023d-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a023d-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="a023d-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a023d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a023d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a023d-119">Not supported.</span></span> |
|<span data-ttu-id="a023d-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="a023d-120">Application</span></span>                            | <span data-ttu-id="a023d-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="a023d-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a023d-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a023d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="a023d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="a023d-123">Request headers</span></span>
| <span data-ttu-id="a023d-124">名称</span><span class="sxs-lookup"><span data-stu-id="a023d-124">Name</span></span>         | <span data-ttu-id="a023d-125">类型</span><span class="sxs-lookup"><span data-stu-id="a023d-125">Type</span></span>        | <span data-ttu-id="a023d-126">说明</span><span class="sxs-lookup"><span data-stu-id="a023d-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a023d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a023d-127">Authorization</span></span> | <span data-ttu-id="a023d-128">string</span><span class="sxs-lookup"><span data-stu-id="a023d-128">string</span></span> | <span data-ttu-id="a023d-129">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="a023d-129">Bearer \{token\}.</span></span> <span data-ttu-id="a023d-130">必填。</span><span class="sxs-lookup"><span data-stu-id="a023d-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a023d-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="a023d-131">Request body</span></span>
<span data-ttu-id="a023d-132">在请求正文中，提供用户将成为审阅者的 ID 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a023d-132">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="a023d-133">下表显示可更新 accessReview 时提供的属性。</span><span class="sxs-lookup"><span data-stu-id="a023d-133">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="a023d-134">属性</span><span class="sxs-lookup"><span data-stu-id="a023d-134">Property</span></span>     | <span data-ttu-id="a023d-135">类型</span><span class="sxs-lookup"><span data-stu-id="a023d-135">Type</span></span>        | <span data-ttu-id="a023d-136">Description</span><span class="sxs-lookup"><span data-stu-id="a023d-136">Description</span></span> |
|:-------------|:------------|:------------|
| `id`             |`String`                                                        | <span data-ttu-id="a023d-137">用户 id。</span><span class="sxs-lookup"><span data-stu-id="a023d-137">The user ID.</span></span>  |


## <a name="response"></a><span data-ttu-id="a023d-138">响应</span><span class="sxs-lookup"><span data-stu-id="a023d-138">Response</span></span>
<span data-ttu-id="a023d-139">如果成功，此方法返回`201, Created`响应代码。</span><span class="sxs-lookup"><span data-stu-id="a023d-139">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="a023d-140">示例</span><span class="sxs-lookup"><span data-stu-id="a023d-140">Example</span></span>

<span data-ttu-id="a023d-141">这是一次性的 （不) 访问审阅更新与其他审阅者的示例。</span><span class="sxs-lookup"><span data-stu-id="a023d-141">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="a023d-142">请求</span><span class="sxs-lookup"><span data-stu-id="a023d-142">Request</span></span>
<span data-ttu-id="a023d-143">在请求正文中，提供的用户对象的 id 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a023d-143">In the request body, supply a JSON representation of the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
Content-type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```

##### <a name="response"></a><span data-ttu-id="a023d-144">响应</span><span class="sxs-lookup"><span data-stu-id="a023d-144">Response</span></span>
><span data-ttu-id="a023d-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a023d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created

```

<!-- {
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
