---
title: 列出所有者
description: 检索应用程序的所有者列表（directoryObject 对象）。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: af5ed0ea7360c5e40f6a472992af4ea08eecc6e4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518901"
---
# <a name="list-owners"></a><span data-ttu-id="3c386-103">列出所有者</span><span class="sxs-lookup"><span data-stu-id="3c386-103">List owners</span></span>

<span data-ttu-id="3c386-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c386-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3c386-105">检索[directoryObject](../resources/directoryobject.md)对象的应用程序的所有者列表。</span><span class="sxs-lookup"><span data-stu-id="3c386-105">Retrieve a list of owners for an application that are [directoryObject](../resources/directoryobject.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c386-106">权限</span><span class="sxs-lookup"><span data-stu-id="3c386-106">Permissions</span></span>
<span data-ttu-id="3c386-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c386-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c386-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c386-109">Permission type</span></span>      | <span data-ttu-id="3c386-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c386-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c386-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c386-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3c386-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3c386-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3c386-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c386-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c386-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c386-114">Not supported.</span></span>    |
|<span data-ttu-id="3c386-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c386-115">Application</span></span> | <span data-ttu-id="3c386-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c386-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c386-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c386-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3c386-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3c386-118">Optional query parameters</span></span>
<span data-ttu-id="3c386-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3c386-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c386-120">请求头</span><span class="sxs-lookup"><span data-stu-id="3c386-120">Request headers</span></span>
| <span data-ttu-id="3c386-121">名称</span><span class="sxs-lookup"><span data-stu-id="3c386-121">Name</span></span>       | <span data-ttu-id="3c386-122">类型</span><span class="sxs-lookup"><span data-stu-id="3c386-122">Type</span></span> | <span data-ttu-id="3c386-123">说明</span><span class="sxs-lookup"><span data-stu-id="3c386-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3c386-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c386-124">Authorization</span></span>  | <span data-ttu-id="3c386-125">string</span><span class="sxs-lookup"><span data-stu-id="3c386-125">string</span></span>  | <span data-ttu-id="3c386-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c386-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c386-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c386-128">Request body</span></span>
<span data-ttu-id="3c386-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c386-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c386-130">响应</span><span class="sxs-lookup"><span data-stu-id="3c386-130">Response</span></span>

<span data-ttu-id="3c386-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3c386-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c386-132">示例</span><span class="sxs-lookup"><span data-stu-id="3c386-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c386-133">请求</span><span class="sxs-lookup"><span data-stu-id="3c386-133">Request</span></span>
<span data-ttu-id="3c386-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c386-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3c386-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c386-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="3c386-136">C#</span><span class="sxs-lookup"><span data-stu-id="3c386-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c386-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c386-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c386-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c386-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c386-139">Java</span><span class="sxs-lookup"><span data-stu-id="3c386-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3c386-140">响应</span><span class="sxs-lookup"><span data-stu-id="3c386-140">Response</span></span>
<span data-ttu-id="3c386-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3c386-141">Here is an example of the response.</span></span> 

><span data-ttu-id="3c386-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3c386-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
