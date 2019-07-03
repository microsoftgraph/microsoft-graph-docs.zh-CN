---
title: 'servicePrincipal: List createdObjects'
description: 检索 directoryobject 对象的列表。
localization_priority: Normal
ms.openlocfilehash: 892f5a182f632c3e289b663f1f288eec4c6c0435
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453731"
---
# <a name="serviceprincipal-list-createdobjects"></a><span data-ttu-id="16730-103">servicePrincipal: List createdObjects</span><span class="sxs-lookup"><span data-stu-id="16730-103">servicePrincipal: List createdObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16730-104">检索 directoryobject 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="16730-104">Retrieve a list of directoryobject objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="16730-105">权限</span><span class="sxs-lookup"><span data-stu-id="16730-105">Permissions</span></span>
<span data-ttu-id="16730-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16730-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16730-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="16730-108">Permission type</span></span>      | <span data-ttu-id="16730-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16730-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16730-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16730-110">Delegated (work or school account)</span></span> | <span data-ttu-id="16730-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="16730-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="16730-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16730-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16730-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="16730-113">Not supported.</span></span>    |
|<span data-ttu-id="16730-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="16730-114">Application</span></span> | <span data-ttu-id="16730-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16730-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16730-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16730-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="16730-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="16730-117">Optional query parameters</span></span>
<span data-ttu-id="16730-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="16730-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16730-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="16730-119">Request headers</span></span>
| <span data-ttu-id="16730-120">名称</span><span class="sxs-lookup"><span data-stu-id="16730-120">Name</span></span>       | <span data-ttu-id="16730-121">类型</span><span class="sxs-lookup"><span data-stu-id="16730-121">Type</span></span> | <span data-ttu-id="16730-122">说明</span><span class="sxs-lookup"><span data-stu-id="16730-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="16730-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16730-123">Authorization</span></span>  | <span data-ttu-id="16730-124">string</span><span class="sxs-lookup"><span data-stu-id="16730-124">string</span></span>  | <span data-ttu-id="16730-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16730-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16730-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="16730-127">Request body</span></span>
<span data-ttu-id="16730-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16730-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16730-129">响应</span><span class="sxs-lookup"><span data-stu-id="16730-129">Response</span></span>

<span data-ttu-id="16730-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="16730-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="16730-131">示例</span><span class="sxs-lookup"><span data-stu-id="16730-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16730-132">请求</span><span class="sxs-lookup"><span data-stu-id="16730-132">Request</span></span>
<span data-ttu-id="16730-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16730-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="16730-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="16730-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/createdObjects
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16730-135">C#</span><span class="sxs-lookup"><span data-stu-id="16730-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16730-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="16730-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16730-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="16730-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16730-138">响应</span><span class="sxs-lookup"><span data-stu-id="16730-138">Response</span></span>
<span data-ttu-id="16730-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16730-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
