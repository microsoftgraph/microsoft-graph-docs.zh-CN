---
title: 获取 schemaExtension
description: 获取指定 schemaExtension 定义的属性。
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: cd8252475954df778156ecdfd780179a04444192
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038969"
---
# <a name="get-schemaextension"></a><span data-ttu-id="436a6-103">获取 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="436a6-103">Get schemaExtension</span></span>

<span data-ttu-id="436a6-104">命名空间：microsoft.graph 获取指定 [schemaExtension 定义](../resources/schemaextension.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="436a6-104">Namespace: microsoft.graph Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="436a6-105">权限</span><span class="sxs-lookup"><span data-stu-id="436a6-105">Permissions</span></span>
<span data-ttu-id="436a6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="436a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="436a6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="436a6-108">Permission type</span></span>      | <span data-ttu-id="436a6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="436a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="436a6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="436a6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="436a6-111">User.Read、Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="436a6-111">User.Read, Application.Read.All</span></span>    |
|<span data-ttu-id="436a6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="436a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="436a6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="436a6-113">Not supported.</span></span>    |
|<span data-ttu-id="436a6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="436a6-114">Application</span></span> | <span data-ttu-id="436a6-115">Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="436a6-115">Application.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="436a6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="436a6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="436a6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="436a6-117">Optional query parameters</span></span>
<span data-ttu-id="436a6-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="436a6-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="436a6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="436a6-119">Request headers</span></span>
| <span data-ttu-id="436a6-120">名称</span><span class="sxs-lookup"><span data-stu-id="436a6-120">Name</span></span>      |<span data-ttu-id="436a6-121">说明</span><span class="sxs-lookup"><span data-stu-id="436a6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="436a6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="436a6-122">Authorization</span></span>  | <span data-ttu-id="436a6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="436a6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="436a6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="436a6-125">Content-Type</span></span>   | <span data-ttu-id="436a6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="436a6-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="436a6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="436a6-127">Request body</span></span>
<span data-ttu-id="436a6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="436a6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="436a6-129">响应</span><span class="sxs-lookup"><span data-stu-id="436a6-129">Response</span></span>

<span data-ttu-id="436a6-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [schemaExtension](../resources/schemaextension.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="436a6-130">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="436a6-131">示例</span><span class="sxs-lookup"><span data-stu-id="436a6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="436a6-132">请求</span><span class="sxs-lookup"><span data-stu-id="436a6-132">Request</span></span>
<span data-ttu-id="436a6-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="436a6-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="436a6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="436a6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/schemaExtensions/graphlearn_test
```
# <a name="c"></a>[<span data-ttu-id="436a6-135">C#</span><span class="sxs-lookup"><span data-stu-id="436a6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="436a6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="436a6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="436a6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="436a6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="436a6-138">Java</span><span class="sxs-lookup"><span data-stu-id="436a6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="436a6-139">响应</span><span class="sxs-lookup"><span data-stu-id="436a6-139">Response</span></span>
<span data-ttu-id="436a6-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="436a6-140">Here is an example of the response.</span></span> <span data-ttu-id="436a6-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="436a6-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "id":"graphlearn_test",
    "description": "Yet another test schema",
    "targetTypes": [
        "User", "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "testName",
            "type": "String"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="436a6-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="436a6-142">See also</span></span>

- [<span data-ttu-id="436a6-143">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="436a6-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="436a6-144">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="436a6-144">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
