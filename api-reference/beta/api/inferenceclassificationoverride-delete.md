---
title: 删除 inferenceClassificationOverride
description: 删除由其 ID 指定的重点收件箱覆盖。
localization_priority: Normal
ms.openlocfilehash: b1b7eac0e4f3b8a94526306f8918f8d88a117a7d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441819"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="d6025-103">删除 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="d6025-103">Delete inferenceClassificationOverride</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6025-104">删除由其 ID 指定的[重点收件箱](../resources/manage-focused-inbox.md)覆盖。</span><span class="sxs-lookup"><span data-stu-id="d6025-104">Delete a [Focused Inbox](../resources/manage-focused-inbox.md) override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="d6025-105">权限</span><span class="sxs-lookup"><span data-stu-id="d6025-105">Permissions</span></span>
<span data-ttu-id="d6025-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6025-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6025-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6025-108">Permission type</span></span>      | <span data-ttu-id="d6025-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6025-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6025-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6025-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d6025-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6025-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d6025-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6025-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6025-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6025-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d6025-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6025-114">Application</span></span> | <span data-ttu-id="d6025-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6025-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6025-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6025-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d6025-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6025-117">Request headers</span></span>
| <span data-ttu-id="d6025-118">名称</span><span class="sxs-lookup"><span data-stu-id="d6025-118">Name</span></span>       | <span data-ttu-id="d6025-119">类型</span><span class="sxs-lookup"><span data-stu-id="d6025-119">Type</span></span> | <span data-ttu-id="d6025-120">说明</span><span class="sxs-lookup"><span data-stu-id="d6025-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d6025-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6025-121">Authorization</span></span>  | <span data-ttu-id="d6025-122">string</span><span class="sxs-lookup"><span data-stu-id="d6025-122">string</span></span>  | <span data-ttu-id="d6025-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6025-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6025-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6025-125">Request body</span></span>
<span data-ttu-id="d6025-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d6025-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6025-127">响应</span><span class="sxs-lookup"><span data-stu-id="d6025-127">Response</span></span>

<span data-ttu-id="d6025-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d6025-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6025-130">示例</span><span class="sxs-lookup"><span data-stu-id="d6025-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6025-131">请求</span><span class="sxs-lookup"><span data-stu-id="d6025-131">Request</span></span>
<span data-ttu-id="d6025-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6025-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d6025-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d6025-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d6025-134">C#</span><span class="sxs-lookup"><span data-stu-id="d6025-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6025-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="d6025-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d6025-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="d6025-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d6025-137">响应</span><span class="sxs-lookup"><span data-stu-id="d6025-137">Response</span></span>
<span data-ttu-id="d6025-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d6025-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
