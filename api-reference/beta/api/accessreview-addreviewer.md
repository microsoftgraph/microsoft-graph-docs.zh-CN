---
title: 添加 accessReview 审阅者
description: '在 Azure AD 访问评论功能中，更新要作为审阅者添加另一个用户现有 accessReview 对象。  此操作仅允许尚未完成，访问审阅和仅访问审阅显式指定审阅者的位置。 此操作不允许用户在其中查看他们自己的访问，访问审阅，不应在其中为审阅者分配组的所有者访问审阅。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1a526451330321c7fbbfd1d5287dd5ad892eee84
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516362"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="3a37f-105">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="3a37f-105">Add accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a37f-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，更新要作为审阅者添加另一个用户现有[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3a37f-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="3a37f-107">此操作仅允许尚未完成，访问审阅和仅访问审阅显式指定审阅者的位置。</span><span class="sxs-lookup"><span data-stu-id="3a37f-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="3a37f-108">此操作不允许用户在其中查看他们自己的访问，访问审阅，不应在其中为审阅者分配组的所有者访问审阅。</span><span class="sxs-lookup"><span data-stu-id="3a37f-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="3a37f-109">权限</span><span class="sxs-lookup"><span data-stu-id="3a37f-109">Permissions</span></span>
<span data-ttu-id="3a37f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3a37f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a37f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a37f-112">Permission type</span></span>                        | <span data-ttu-id="3a37f-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3a37f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a37f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a37f-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a37f-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a37f-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="3a37f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a37f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a37f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a37f-117">Not supported.</span></span> |
|<span data-ttu-id="3a37f-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a37f-118">Application</span></span>                            | <span data-ttu-id="3a37f-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a37f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a37f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a37f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="3a37f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a37f-121">Request headers</span></span>
| <span data-ttu-id="3a37f-122">名称</span><span class="sxs-lookup"><span data-stu-id="3a37f-122">Name</span></span>         | <span data-ttu-id="3a37f-123">类型</span><span class="sxs-lookup"><span data-stu-id="3a37f-123">Type</span></span>        | <span data-ttu-id="3a37f-124">说明</span><span class="sxs-lookup"><span data-stu-id="3a37f-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3a37f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a37f-125">Authorization</span></span> | <span data-ttu-id="3a37f-126">string</span><span class="sxs-lookup"><span data-stu-id="3a37f-126">string</span></span> | <span data-ttu-id="3a37f-127">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="3a37f-127">Bearer \{token\}.</span></span> <span data-ttu-id="3a37f-128">必需。</span><span class="sxs-lookup"><span data-stu-id="3a37f-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a37f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a37f-129">Request body</span></span>
<span data-ttu-id="3a37f-130">在请求正文中，提供用户将成为审阅者的 ID 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a37f-130">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="3a37f-131">下表显示可更新 accessReview 时提供的属性。</span><span class="sxs-lookup"><span data-stu-id="3a37f-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="3a37f-132">属性</span><span class="sxs-lookup"><span data-stu-id="3a37f-132">Property</span></span>     | <span data-ttu-id="3a37f-133">类型</span><span class="sxs-lookup"><span data-stu-id="3a37f-133">Type</span></span>        | <span data-ttu-id="3a37f-134">说明</span><span class="sxs-lookup"><span data-stu-id="3a37f-134">Description</span></span> |
|:-------------|:------------|:------------|
| `id`             |`String`                                                        | <span data-ttu-id="3a37f-135">用户 id。</span><span class="sxs-lookup"><span data-stu-id="3a37f-135">The user ID.</span></span>  |


## <a name="response"></a><span data-ttu-id="3a37f-136">响应</span><span class="sxs-lookup"><span data-stu-id="3a37f-136">Response</span></span>
<span data-ttu-id="3a37f-137">如果成功，此方法返回`201, Created`响应代码。</span><span class="sxs-lookup"><span data-stu-id="3a37f-137">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="3a37f-138">示例</span><span class="sxs-lookup"><span data-stu-id="3a37f-138">Example</span></span>

<span data-ttu-id="3a37f-139">这是一次性的 （不) 访问审阅更新与其他审阅者的示例。</span><span class="sxs-lookup"><span data-stu-id="3a37f-139">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="3a37f-140">请求</span><span class="sxs-lookup"><span data-stu-id="3a37f-140">Request</span></span>
<span data-ttu-id="3a37f-141">在请求正文中，提供的用户对象的 id 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a37f-141">In the request body, supply a JSON representation of the id of the user object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="3a37f-142">响应</span><span class="sxs-lookup"><span data-stu-id="3a37f-142">Response</span></span>
><span data-ttu-id="3a37f-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3a37f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created

```

<!--
{
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-addreviewer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
