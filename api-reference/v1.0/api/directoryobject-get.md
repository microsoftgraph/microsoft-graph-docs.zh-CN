---
title: 获取 directoryObject
description: 检索 directoryObject 对象的属性和关系。
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f70e9fac71b9ddaf74ec1f9d0556abb5328b4451
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455950"
---
# <a name="get-directoryobject"></a><span data-ttu-id="7333f-103">获取 directoryObject</span><span class="sxs-lookup"><span data-stu-id="7333f-103">Get directoryObject</span></span>

<span data-ttu-id="7333f-104">检索 directoryObject 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7333f-104">Retrieve the properties and relationships of directoryObject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7333f-105">权限</span><span class="sxs-lookup"><span data-stu-id="7333f-105">Permissions</span></span>
<span data-ttu-id="7333f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7333f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7333f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7333f-108">Permission type</span></span>      | <span data-ttu-id="7333f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7333f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7333f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7333f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7333f-111">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7333f-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7333f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7333f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7333f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7333f-113">Not supported.</span></span>    |
|<span data-ttu-id="7333f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7333f-114">Application</span></span> | <span data-ttu-id="7333f-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7333f-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7333f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7333f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7333f-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7333f-117">Optional query parameters</span></span>
<span data-ttu-id="7333f-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7333f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7333f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7333f-119">Request headers</span></span>
| <span data-ttu-id="7333f-120">名称</span><span class="sxs-lookup"><span data-stu-id="7333f-120">Name</span></span>       | <span data-ttu-id="7333f-121">类型</span><span class="sxs-lookup"><span data-stu-id="7333f-121">Type</span></span> | <span data-ttu-id="7333f-122">说明</span><span class="sxs-lookup"><span data-stu-id="7333f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7333f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7333f-123">Authorization</span></span>  | <span data-ttu-id="7333f-124">string</span><span class="sxs-lookup"><span data-stu-id="7333f-124">string</span></span>  | <span data-ttu-id="7333f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7333f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7333f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7333f-127">Request body</span></span>
<span data-ttu-id="7333f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7333f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7333f-129">响应</span><span class="sxs-lookup"><span data-stu-id="7333f-129">Response</span></span>

<span data-ttu-id="7333f-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7333f-130">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7333f-131">示例</span><span class="sxs-lookup"><span data-stu-id="7333f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7333f-132">请求</span><span class="sxs-lookup"><span data-stu-id="7333f-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7333f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7333f-133">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7333f-134">C#</span><span class="sxs-lookup"><span data-stu-id="7333f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7333f-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="7333f-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7333f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7333f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7333f-137">响应</span><span class="sxs-lookup"><span data-stu-id="7333f-137">Response</span></span>
<span data-ttu-id="7333f-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7333f-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
