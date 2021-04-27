---
title: 创建 memberOf
description: 使用此 API 创建新的 memberOf。
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b8919fb0a9513d2278d07a73cf1dc95327fdc983
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055510"
---
# <a name="create-memberof"></a><span data-ttu-id="4ecba-103">创建 memberOf</span><span class="sxs-lookup"><span data-stu-id="4ecba-103">Create memberOf</span></span>

<span data-ttu-id="4ecba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ecba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ecba-105">使用此 API 创建新的 memberOf。</span><span class="sxs-lookup"><span data-stu-id="4ecba-105">Use this API to create a new memberOf.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ecba-106">权限</span><span class="sxs-lookup"><span data-stu-id="4ecba-106">Permissions</span></span>
<span data-ttu-id="4ecba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ecba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ecba-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ecba-109">Permission type</span></span>      | <span data-ttu-id="4ecba-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ecba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ecba-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ecba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4ecba-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ecba-112">Not supported.</span></span>    |
|<span data-ttu-id="4ecba-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ecba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ecba-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ecba-114">Not supported.</span></span>    |
|<span data-ttu-id="4ecba-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ecba-115">Application</span></span> | <span data-ttu-id="4ecba-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ecba-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ecba-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ecba-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="4ecba-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ecba-118">Request headers</span></span>
| <span data-ttu-id="4ecba-119">名称</span><span class="sxs-lookup"><span data-stu-id="4ecba-119">Name</span></span>       | <span data-ttu-id="4ecba-120">类型</span><span class="sxs-lookup"><span data-stu-id="4ecba-120">Type</span></span> | <span data-ttu-id="4ecba-121">说明</span><span class="sxs-lookup"><span data-stu-id="4ecba-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4ecba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ecba-122">Authorization</span></span>  | <span data-ttu-id="4ecba-123">string</span><span class="sxs-lookup"><span data-stu-id="4ecba-123">string</span></span>  | <span data-ttu-id="4ecba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ecba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ecba-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ecba-126">Request body</span></span>
<span data-ttu-id="4ecba-127">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ecba-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4ecba-128">响应</span><span class="sxs-lookup"><span data-stu-id="4ecba-128">Response</span></span>

<span data-ttu-id="4ecba-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ecba-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ecba-130">示例</span><span class="sxs-lookup"><span data-stu-id="4ecba-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ecba-131">请求</span><span class="sxs-lookup"><span data-stu-id="4ecba-131">Request</span></span>
<span data-ttu-id="4ecba-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ecba-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ecba-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ecba-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact_2"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/memberOf
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="4ecba-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ecba-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-orgcontact-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="4ecba-135">C#</span><span class="sxs-lookup"><span data-stu-id="4ecba-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-orgcontact-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4ecba-136">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ecba-136">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4ecba-137">响应</span><span class="sxs-lookup"><span data-stu-id="4ecba-137">Response</span></span>
<span data-ttu-id="4ecba-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4ecba-138">Here is an example of the response.</span></span> <span data-ttu-id="4ecba-139">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4ecba-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


