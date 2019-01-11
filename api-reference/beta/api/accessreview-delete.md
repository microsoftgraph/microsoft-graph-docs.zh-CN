---
title: 删除 accessReview
description: 在 Azure AD 中访问审阅功能，删除 accessReview 对象。
localization_priority: Normal
ms.openlocfilehash: b062931e58834e1b6a62c83791ec663865fb5c9c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829454"
---
# <a name="delete-accessreview"></a><span data-ttu-id="4b2af-103">删除 accessReview</span><span class="sxs-lookup"><span data-stu-id="4b2af-103">Delete accessReview</span></span>

> <span data-ttu-id="4b2af-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4b2af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b2af-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4b2af-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b2af-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，删除[accessReview](../resources/accessreview.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4b2af-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4b2af-107">权限</span><span class="sxs-lookup"><span data-stu-id="4b2af-107">Permissions</span></span>
<span data-ttu-id="4b2af-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b2af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b2af-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b2af-110">Permission type</span></span>                        | <span data-ttu-id="4b2af-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b2af-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b2af-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b2af-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b2af-113">AccessReview.ReadWrite.All，也应具有完成呼叫中以删除 programControl 方案的 ProgramControl.ReadWrite.All 和</span><span class="sxs-lookup"><span data-stu-id="4b2af-113">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with a call to delete a programControl</span></span> |
|<span data-ttu-id="4b2af-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b2af-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b2af-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b2af-115">Not supported.</span></span> |
|<span data-ttu-id="4b2af-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b2af-116">Application</span></span>                            | <span data-ttu-id="4b2af-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b2af-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b2af-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b2af-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="4b2af-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b2af-119">Request headers</span></span>
| <span data-ttu-id="4b2af-120">名称</span><span class="sxs-lookup"><span data-stu-id="4b2af-120">Name</span></span>         | <span data-ttu-id="4b2af-121">类型</span><span class="sxs-lookup"><span data-stu-id="4b2af-121">Type</span></span>        | <span data-ttu-id="4b2af-122">说明</span><span class="sxs-lookup"><span data-stu-id="4b2af-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4b2af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b2af-123">Authorization</span></span> | <span data-ttu-id="4b2af-124">string</span><span class="sxs-lookup"><span data-stu-id="4b2af-124">string</span></span> | <span data-ttu-id="4b2af-125">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="4b2af-125">Bearer \{token\}.</span></span> <span data-ttu-id="4b2af-126">必填。</span><span class="sxs-lookup"><span data-stu-id="4b2af-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b2af-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b2af-127">Request body</span></span>
<span data-ttu-id="4b2af-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b2af-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4b2af-129">响应</span><span class="sxs-lookup"><span data-stu-id="4b2af-129">Response</span></span>
<span data-ttu-id="4b2af-p104">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4b2af-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b2af-132">示例</span><span class="sxs-lookup"><span data-stu-id="4b2af-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b2af-133">请求</span><span class="sxs-lookup"><span data-stu-id="4b2af-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')
```
##### <a name="response"></a><span data-ttu-id="4b2af-134">响应</span><span class="sxs-lookup"><span data-stu-id="4b2af-134">Response</span></span>
><span data-ttu-id="4b2af-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4b2af-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
