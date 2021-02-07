---
title: 列出所有者
description: 检索应用程序 (directoryObject 对象) 列表。
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: d9f942bb007ce3a3ade3632ddcbe9f2e79e9e9cb
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134034"
---
# <a name="list-owners"></a><span data-ttu-id="d733d-103">列出所有者</span><span class="sxs-lookup"><span data-stu-id="d733d-103">List owners</span></span>

<span data-ttu-id="d733d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d733d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d733d-105">检索作为 [directoryObject](../resources/directoryobject.md) 对象的应用程序的所有者列表。</span><span class="sxs-lookup"><span data-stu-id="d733d-105">Retrieve a list of owners for an application that are [directoryObject](../resources/directoryobject.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d733d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d733d-106">Permissions</span></span>
<span data-ttu-id="d733d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d733d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d733d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d733d-109">Permission type</span></span>      | <span data-ttu-id="d733d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d733d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d733d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d733d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d733d-112">Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d733d-112">Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d733d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d733d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d733d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d733d-114">Not supported.</span></span>    |
|<span data-ttu-id="d733d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d733d-115">Application</span></span> | <span data-ttu-id="d733d-116">Application.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d733d-116">Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d733d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d733d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d733d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d733d-118">Optional query parameters</span></span>
<span data-ttu-id="d733d-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d733d-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d733d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d733d-120">Request headers</span></span>
| <span data-ttu-id="d733d-121">名称</span><span class="sxs-lookup"><span data-stu-id="d733d-121">Name</span></span>           | <span data-ttu-id="d733d-122">说明</span><span class="sxs-lookup"><span data-stu-id="d733d-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="d733d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d733d-123">Authorization</span></span>  | <span data-ttu-id="d733d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d733d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d733d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d733d-126">Request body</span></span>
<span data-ttu-id="d733d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d733d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d733d-128">响应</span><span class="sxs-lookup"><span data-stu-id="d733d-128">Response</span></span>

<span data-ttu-id="d733d-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d733d-129">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d733d-130">示例</span><span class="sxs-lookup"><span data-stu-id="d733d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d733d-131">请求</span><span class="sxs-lookup"><span data-stu-id="d733d-131">Request</span></span>
<span data-ttu-id="d733d-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d733d-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d733d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d733d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="d733d-134">C#</span><span class="sxs-lookup"><span data-stu-id="d733d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d733d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d733d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d733d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d733d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d733d-137">Java</span><span class="sxs-lookup"><span data-stu-id="d733d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d733d-138">响应</span><span class="sxs-lookup"><span data-stu-id="d733d-138">Response</span></span>
<span data-ttu-id="d733d-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d733d-139">Here is an example of the response.</span></span> 

><span data-ttu-id="d733d-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d733d-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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

