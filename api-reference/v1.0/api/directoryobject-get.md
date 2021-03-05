---
title: 获取 directoryObject
description: 检索 directoryObject 对象的属性和关系。
author: keylimesoda
localization_priority: Priority
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: bf1e017e6fd69168b41e83b8adc19f9bd4d5f216
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434424"
---
# <a name="get-directoryobject"></a><span data-ttu-id="5310c-103">获取 directoryObject</span><span class="sxs-lookup"><span data-stu-id="5310c-103">Get directoryObject</span></span>

<span data-ttu-id="5310c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5310c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5310c-105">检索 directoryObject 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5310c-105">Retrieve the properties and relationships of directoryObject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5310c-106">权限</span><span class="sxs-lookup"><span data-stu-id="5310c-106">Permissions</span></span>
<span data-ttu-id="5310c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5310c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5310c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5310c-109">Permission type</span></span>      | <span data-ttu-id="5310c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5310c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5310c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5310c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5310c-112">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5310c-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5310c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5310c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5310c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5310c-114">Not supported.</span></span>    |
|<span data-ttu-id="5310c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5310c-115">Application</span></span> | <span data-ttu-id="5310c-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5310c-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5310c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5310c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5310c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5310c-118">Optional query parameters</span></span>
<span data-ttu-id="5310c-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5310c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5310c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5310c-120">Request headers</span></span>
| <span data-ttu-id="5310c-121">名称</span><span class="sxs-lookup"><span data-stu-id="5310c-121">Name</span></span>       | <span data-ttu-id="5310c-122">类型</span><span class="sxs-lookup"><span data-stu-id="5310c-122">Type</span></span> | <span data-ttu-id="5310c-123">说明</span><span class="sxs-lookup"><span data-stu-id="5310c-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5310c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5310c-124">Authorization</span></span>  | <span data-ttu-id="5310c-125">string</span><span class="sxs-lookup"><span data-stu-id="5310c-125">string</span></span>  | <span data-ttu-id="5310c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5310c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5310c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5310c-128">Request body</span></span>
<span data-ttu-id="5310c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5310c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5310c-130">响应</span><span class="sxs-lookup"><span data-stu-id="5310c-130">Response</span></span>

<span data-ttu-id="5310c-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5310c-131">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5310c-132">示例</span><span class="sxs-lookup"><span data-stu-id="5310c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5310c-133">请求</span><span class="sxs-lookup"><span data-stu-id="5310c-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5310c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5310c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
# <a name="c"></a>[<span data-ttu-id="5310c-135">C#</span><span class="sxs-lookup"><span data-stu-id="5310c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5310c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5310c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5310c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5310c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5310c-138">Java</span><span class="sxs-lookup"><span data-stu-id="5310c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5310c-139">响应</span><span class="sxs-lookup"><span data-stu-id="5310c-139">Response</span></span>
<span data-ttu-id="5310c-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5310c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
