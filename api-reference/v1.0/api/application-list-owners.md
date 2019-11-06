---
title: 列出所有者
description: 检索应用程序的所有者列表（directoryObject 对象）。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f91a7926c5635a1f66622b6f3dd7e375d42c3f7d
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999111"
---
# <a name="list-owners"></a><span data-ttu-id="39950-103">列出所有者</span><span class="sxs-lookup"><span data-stu-id="39950-103">List owners</span></span>

<span data-ttu-id="39950-104">检索[directoryObject](../resources/directoryobject.md)对象的应用程序的所有者列表。</span><span class="sxs-lookup"><span data-stu-id="39950-104">Retrieve a list of owners for an application that are [directoryObject](../resources/directoryobject.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="39950-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="39950-105">Permissions</span></span>
<span data-ttu-id="39950-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39950-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="39950-108">Permission type</span></span>      | <span data-ttu-id="39950-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39950-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39950-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39950-110">Delegated (work or school account)</span></span> | <span data-ttu-id="39950-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="39950-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="39950-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39950-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39950-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="39950-113">Not supported.</span></span>    |
|<span data-ttu-id="39950-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="39950-114">Application</span></span> | <span data-ttu-id="39950-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39950-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39950-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39950-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="39950-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="39950-117">Optional query parameters</span></span>
<span data-ttu-id="39950-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="39950-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39950-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="39950-119">Request headers</span></span>
| <span data-ttu-id="39950-120">名称</span><span class="sxs-lookup"><span data-stu-id="39950-120">Name</span></span>       | <span data-ttu-id="39950-121">类型</span><span class="sxs-lookup"><span data-stu-id="39950-121">Type</span></span> | <span data-ttu-id="39950-122">说明</span><span class="sxs-lookup"><span data-stu-id="39950-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="39950-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="39950-123">Authorization</span></span>  | <span data-ttu-id="39950-124">string</span><span class="sxs-lookup"><span data-stu-id="39950-124">string</span></span>  | <span data-ttu-id="39950-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="39950-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="39950-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="39950-127">Request body</span></span>
<span data-ttu-id="39950-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="39950-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39950-129">响应</span><span class="sxs-lookup"><span data-stu-id="39950-129">Response</span></span>

<span data-ttu-id="39950-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="39950-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="39950-131">示例</span><span class="sxs-lookup"><span data-stu-id="39950-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39950-132">请求</span><span class="sxs-lookup"><span data-stu-id="39950-132">Request</span></span>
<span data-ttu-id="39950-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39950-133">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="39950-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="39950-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/owners
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="39950-135">C#</span><span class="sxs-lookup"><span data-stu-id="39950-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="39950-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39950-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="39950-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39950-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="39950-138">Java</span><span class="sxs-lookup"><span data-stu-id="39950-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="39950-139">响应</span><span class="sxs-lookup"><span data-stu-id="39950-139">Response</span></span>
<span data-ttu-id="39950-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="39950-140">Here is an example of the response.</span></span> 

><span data-ttu-id="39950-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="39950-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
