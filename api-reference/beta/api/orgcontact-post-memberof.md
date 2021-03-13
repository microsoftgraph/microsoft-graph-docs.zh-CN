---
title: 创建 memberOf
description: 使用此 API 创建新的 memberOf。
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e88f669020d1566765f9313182ee21bc33fe1dd9
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759417"
---
# <a name="create-memberof"></a><span data-ttu-id="4007f-103">创建 memberOf</span><span class="sxs-lookup"><span data-stu-id="4007f-103">Create memberOf</span></span>

<span data-ttu-id="4007f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4007f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4007f-105">使用此 API 创建新的 memberOf。</span><span class="sxs-lookup"><span data-stu-id="4007f-105">Use this API to create a new memberOf.</span></span>
## <a name="permissions"></a><span data-ttu-id="4007f-106">权限</span><span class="sxs-lookup"><span data-stu-id="4007f-106">Permissions</span></span>
<span data-ttu-id="4007f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4007f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4007f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4007f-109">Permission type</span></span>      | <span data-ttu-id="4007f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4007f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4007f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4007f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4007f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="4007f-112">Not supported.</span></span>    |
|<span data-ttu-id="4007f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4007f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4007f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4007f-114">Not supported.</span></span>    |
|<span data-ttu-id="4007f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4007f-115">Application</span></span> | <span data-ttu-id="4007f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4007f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4007f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4007f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="4007f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4007f-118">Request headers</span></span>
| <span data-ttu-id="4007f-119">名称</span><span class="sxs-lookup"><span data-stu-id="4007f-119">Name</span></span>       | <span data-ttu-id="4007f-120">类型</span><span class="sxs-lookup"><span data-stu-id="4007f-120">Type</span></span> | <span data-ttu-id="4007f-121">说明</span><span class="sxs-lookup"><span data-stu-id="4007f-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4007f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4007f-122">Authorization</span></span>  | <span data-ttu-id="4007f-123">string</span><span class="sxs-lookup"><span data-stu-id="4007f-123">string</span></span>  | <span data-ttu-id="4007f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4007f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4007f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4007f-126">Request body</span></span>
<span data-ttu-id="4007f-127">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4007f-127">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4007f-128">响应</span><span class="sxs-lookup"><span data-stu-id="4007f-128">Response</span></span>

<span data-ttu-id="4007f-129">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4007f-129">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4007f-130">示例</span><span class="sxs-lookup"><span data-stu-id="4007f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4007f-131">请求</span><span class="sxs-lookup"><span data-stu-id="4007f-131">Request</span></span>
<span data-ttu-id="4007f-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4007f-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4007f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4007f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_orgcontact"
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
# <a name="javascript"></a>[<span data-ttu-id="4007f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4007f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="4007f-135">C#</span><span class="sxs-lookup"><span data-stu-id="4007f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4007f-136">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4007f-136">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4007f-137">响应</span><span class="sxs-lookup"><span data-stu-id="4007f-137">Response</span></span>
<span data-ttu-id="4007f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4007f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


