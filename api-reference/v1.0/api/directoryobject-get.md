---
title: 获取 directoryObject
description: 检索 directoryObject 对象的属性和关系。
author: keylimesoda
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8d42b3ffcce2d8397cd28d66920271c9d0e6ed28
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406086"
---
# <a name="get-directoryobject"></a><span data-ttu-id="d0a9b-103">获取 directoryObject</span><span class="sxs-lookup"><span data-stu-id="d0a9b-103">Get directoryObject</span></span>

<span data-ttu-id="d0a9b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0a9b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d0a9b-105">检索 directoryObject 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d0a9b-105">Retrieve the properties and relationships of directoryObject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d0a9b-106">权限</span><span class="sxs-lookup"><span data-stu-id="d0a9b-106">Permissions</span></span>
<span data-ttu-id="d0a9b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0a9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0a9b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0a9b-109">Permission type</span></span>      | <span data-ttu-id="d0a9b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0a9b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0a9b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0a9b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d0a9b-112">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0a9b-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d0a9b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0a9b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0a9b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0a9b-114">Not supported.</span></span>    |
|<span data-ttu-id="d0a9b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0a9b-115">Application</span></span> | <span data-ttu-id="d0a9b-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0a9b-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0a9b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0a9b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d0a9b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d0a9b-118">Optional query parameters</span></span>
<span data-ttu-id="d0a9b-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d0a9b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d0a9b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0a9b-120">Request headers</span></span>
| <span data-ttu-id="d0a9b-121">名称</span><span class="sxs-lookup"><span data-stu-id="d0a9b-121">Name</span></span>       | <span data-ttu-id="d0a9b-122">类型</span><span class="sxs-lookup"><span data-stu-id="d0a9b-122">Type</span></span> | <span data-ttu-id="d0a9b-123">说明</span><span class="sxs-lookup"><span data-stu-id="d0a9b-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d0a9b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0a9b-124">Authorization</span></span>  | <span data-ttu-id="d0a9b-125">string</span><span class="sxs-lookup"><span data-stu-id="d0a9b-125">string</span></span>  | <span data-ttu-id="d0a9b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d0a9b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0a9b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0a9b-128">Request body</span></span>
<span data-ttu-id="d0a9b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d0a9b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0a9b-130">响应</span><span class="sxs-lookup"><span data-stu-id="d0a9b-130">Response</span></span>

<span data-ttu-id="d0a9b-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0a9b-131">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d0a9b-132">示例</span><span class="sxs-lookup"><span data-stu-id="d0a9b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0a9b-133">请求</span><span class="sxs-lookup"><span data-stu-id="d0a9b-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d0a9b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0a9b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
# <a name="c"></a>[<span data-ttu-id="d0a9b-135">C#</span><span class="sxs-lookup"><span data-stu-id="d0a9b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0a9b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0a9b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0a9b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0a9b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0a9b-138">Java</span><span class="sxs-lookup"><span data-stu-id="d0a9b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d0a9b-139">响应</span><span class="sxs-lookup"><span data-stu-id="d0a9b-139">Response</span></span>
<span data-ttu-id="d0a9b-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0a9b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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