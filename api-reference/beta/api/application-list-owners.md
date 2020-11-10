---
title: 列出所有者
description: 检索应用程序) 的所有者 (directoryObject 对象的列表。
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dc5554c4ed94b47a0961bcb715d3d02546a4b18c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962113"
---
# <a name="list-owners"></a><span data-ttu-id="80ced-103">列出所有者</span><span class="sxs-lookup"><span data-stu-id="80ced-103">List owners</span></span>

<span data-ttu-id="80ced-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80ced-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80ced-105">检索 [directoryObject](../resources/directoryobject.md) 对象的应用程序的所有者列表。</span><span class="sxs-lookup"><span data-stu-id="80ced-105">Retrieve a list of owners for an application that are [directoryObject](../resources/directoryobject.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="80ced-106">权限</span><span class="sxs-lookup"><span data-stu-id="80ced-106">Permissions</span></span>
<span data-ttu-id="80ced-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80ced-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80ced-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="80ced-109">Permission type</span></span>      | <span data-ttu-id="80ced-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80ced-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80ced-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80ced-111">Delegated (work or school account)</span></span> | <span data-ttu-id="80ced-112">Application.Read.All、Directory.Read.All、Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="80ced-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="80ced-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80ced-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80ced-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="80ced-114">Not supported.</span></span>    |
|<span data-ttu-id="80ced-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="80ced-115">Application</span></span> | <span data-ttu-id="80ced-116">Application.Read.All、Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80ced-116">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="80ced-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80ced-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="80ced-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="80ced-118">Optional query parameters</span></span>
<span data-ttu-id="80ced-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="80ced-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80ced-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="80ced-120">Request headers</span></span>
| <span data-ttu-id="80ced-121">名称</span><span class="sxs-lookup"><span data-stu-id="80ced-121">Name</span></span>           | <span data-ttu-id="80ced-122">说明</span><span class="sxs-lookup"><span data-stu-id="80ced-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="80ced-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80ced-123">Authorization</span></span>  | <span data-ttu-id="80ced-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80ced-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="80ced-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="80ced-126">Request body</span></span>
<span data-ttu-id="80ced-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="80ced-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80ced-128">响应</span><span class="sxs-lookup"><span data-stu-id="80ced-128">Response</span></span>

<span data-ttu-id="80ced-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="80ced-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="80ced-130">示例</span><span class="sxs-lookup"><span data-stu-id="80ced-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80ced-131">请求</span><span class="sxs-lookup"><span data-stu-id="80ced-131">Request</span></span>
<span data-ttu-id="80ced-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80ced-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="80ced-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="80ced-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="80ced-134">C#</span><span class="sxs-lookup"><span data-stu-id="80ced-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80ced-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80ced-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80ced-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80ced-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80ced-137">Java</span><span class="sxs-lookup"><span data-stu-id="80ced-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="80ced-138">响应</span><span class="sxs-lookup"><span data-stu-id="80ced-138">Response</span></span>
<span data-ttu-id="80ced-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80ced-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
