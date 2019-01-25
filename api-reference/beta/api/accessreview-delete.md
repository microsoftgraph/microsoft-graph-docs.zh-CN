---
title: 删除 accessReview
description: 在 Azure AD 中访问审阅功能，删除 accessReview 对象。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 28848cc047306259248d0ba4663ab3eb3e964224
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527771"
---
# <a name="delete-accessreview"></a><span data-ttu-id="36e05-103">删除 accessReview</span><span class="sxs-lookup"><span data-stu-id="36e05-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36e05-104">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，删除[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="36e05-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="36e05-105">权限</span><span class="sxs-lookup"><span data-stu-id="36e05-105">Permissions</span></span>
<span data-ttu-id="36e05-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36e05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36e05-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="36e05-108">Permission type</span></span>                        | <span data-ttu-id="36e05-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36e05-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="36e05-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36e05-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="36e05-111">AccessReview.ReadWrite.All，也应具有完成呼叫中以删除 programControl 方案的 ProgramControl.ReadWrite.All 和</span><span class="sxs-lookup"><span data-stu-id="36e05-111">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with a call to delete a programControl</span></span> |
|<span data-ttu-id="36e05-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36e05-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36e05-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="36e05-113">Not supported.</span></span> |
|<span data-ttu-id="36e05-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="36e05-114">Application</span></span>                            | <span data-ttu-id="36e05-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="36e05-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36e05-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36e05-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="36e05-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="36e05-117">Request headers</span></span>
| <span data-ttu-id="36e05-118">名称</span><span class="sxs-lookup"><span data-stu-id="36e05-118">Name</span></span>         | <span data-ttu-id="36e05-119">类型</span><span class="sxs-lookup"><span data-stu-id="36e05-119">Type</span></span>        | <span data-ttu-id="36e05-120">说明</span><span class="sxs-lookup"><span data-stu-id="36e05-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="36e05-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="36e05-121">Authorization</span></span> | <span data-ttu-id="36e05-122">string</span><span class="sxs-lookup"><span data-stu-id="36e05-122">string</span></span> | <span data-ttu-id="36e05-123">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="36e05-123">Bearer \{token\}.</span></span> <span data-ttu-id="36e05-124">必需。</span><span class="sxs-lookup"><span data-stu-id="36e05-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36e05-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="36e05-125">Request body</span></span>
<span data-ttu-id="36e05-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36e05-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="36e05-127">响应</span><span class="sxs-lookup"><span data-stu-id="36e05-127">Response</span></span>
<span data-ttu-id="36e05-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="36e05-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36e05-130">示例</span><span class="sxs-lookup"><span data-stu-id="36e05-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36e05-131">请求</span><span class="sxs-lookup"><span data-stu-id="36e05-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')
```
##### <a name="response"></a><span data-ttu-id="36e05-132">响应</span><span class="sxs-lookup"><span data-stu-id="36e05-132">Response</span></span>
><span data-ttu-id="36e05-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="36e05-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
