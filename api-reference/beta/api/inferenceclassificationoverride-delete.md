---
title: 删除 inferenceClassificationOverride
description: 删除由其 ID 指定的重点收件箱覆盖。
localization_priority: Normal
doc_type: apiPageType
author: svpsiva
ms.prod: ''
ms.openlocfilehash: 117a5ce205f7c615300cbe42f1607af03c9ce2af
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953031"
---
# <a name="delete-inferenceclassificationoverride"></a><span data-ttu-id="f0b5e-103">删除 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="f0b5e-103">Delete inferenceClassificationOverride</span></span>

<span data-ttu-id="f0b5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0b5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0b5e-105">删除由其 ID 指定的 [重点收件箱](../resources/manage-focused-inbox.md) 覆盖。</span><span class="sxs-lookup"><span data-stu-id="f0b5e-105">Delete a [Focused Inbox](../resources/manage-focused-inbox.md) override specified by its ID.</span></span>
## <a name="permissions"></a><span data-ttu-id="f0b5e-106">权限</span><span class="sxs-lookup"><span data-stu-id="f0b5e-106">Permissions</span></span>
<span data-ttu-id="f0b5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0b5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0b5e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0b5e-109">Permission type</span></span>      | <span data-ttu-id="f0b5e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0b5e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0b5e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0b5e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f0b5e-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0b5e-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f0b5e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0b5e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0b5e-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0b5e-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f0b5e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0b5e-115">Application</span></span> | <span data-ttu-id="f0b5e-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0b5e-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0b5e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0b5e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/inferenceClassification/overrides/{id}
DELETE /users/{id}/inferenceClassification/overrides/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f0b5e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0b5e-118">Request headers</span></span>
| <span data-ttu-id="f0b5e-119">名称</span><span class="sxs-lookup"><span data-stu-id="f0b5e-119">Name</span></span>       | <span data-ttu-id="f0b5e-120">类型</span><span class="sxs-lookup"><span data-stu-id="f0b5e-120">Type</span></span> | <span data-ttu-id="f0b5e-121">说明</span><span class="sxs-lookup"><span data-stu-id="f0b5e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f0b5e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0b5e-122">Authorization</span></span>  | <span data-ttu-id="f0b5e-123">string</span><span class="sxs-lookup"><span data-stu-id="f0b5e-123">string</span></span>  | <span data-ttu-id="f0b5e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f0b5e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0b5e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0b5e-126">Request body</span></span>
<span data-ttu-id="f0b5e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f0b5e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0b5e-128">响应</span><span class="sxs-lookup"><span data-stu-id="f0b5e-128">Response</span></span>

<span data-ttu-id="f0b5e-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f0b5e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0b5e-131">示例</span><span class="sxs-lookup"><span data-stu-id="f0b5e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0b5e-132">请求</span><span class="sxs-lookup"><span data-stu-id="f0b5e-132">Request</span></span>
<span data-ttu-id="f0b5e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0b5e-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0b5e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0b5e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_inferenceclassificationoverride"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r
```
# <a name="c"></a>[<span data-ttu-id="f0b5e-135">C#</span><span class="sxs-lookup"><span data-stu-id="f0b5e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-inferenceclassificationoverride-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0b5e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0b5e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-inferenceclassificationoverride-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0b5e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0b5e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-inferenceclassificationoverride-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0b5e-138">Java</span><span class="sxs-lookup"><span data-stu-id="f0b5e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-inferenceclassificationoverride-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f0b5e-139">响应</span><span class="sxs-lookup"><span data-stu-id="f0b5e-139">Response</span></span>
<span data-ttu-id="f0b5e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0b5e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


