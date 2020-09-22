---
title: 获取 schemaExtension
description: 获取指定的 schemaExtension 定义的属性。
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 8282492d2d5ba8d99a2b7301fa594896025df139
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058735"
---
# <a name="get-schemaextension"></a><span data-ttu-id="c2b62-103">获取 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="c2b62-103">Get schemaExtension</span></span>

<span data-ttu-id="c2b62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2b62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2b62-105">获取指定的 [schemaExtension](../resources/schemaextension.md) 定义的属性。</span><span class="sxs-lookup"><span data-stu-id="c2b62-105">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2b62-106">权限</span><span class="sxs-lookup"><span data-stu-id="c2b62-106">Permissions</span></span>
<span data-ttu-id="c2b62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2b62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c2b62-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2b62-109">Permission type</span></span>      | <span data-ttu-id="c2b62-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2b62-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2b62-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2b62-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c2b62-112">Read、Application. All</span><span class="sxs-lookup"><span data-stu-id="c2b62-112">User.Read, Application.Read.All</span></span>  |
|<span data-ttu-id="c2b62-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2b62-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2b62-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2b62-114">Not supported.</span></span>    |
|<span data-ttu-id="c2b62-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2b62-115">Application</span></span> | <span data-ttu-id="c2b62-116">Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2b62-116">Application.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2b62-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2b62-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c2b62-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c2b62-118">Optional query parameters</span></span>
<span data-ttu-id="c2b62-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c2b62-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2b62-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2b62-120">Request headers</span></span>
| <span data-ttu-id="c2b62-121">名称</span><span class="sxs-lookup"><span data-stu-id="c2b62-121">Name</span></span>      |<span data-ttu-id="c2b62-122">说明</span><span class="sxs-lookup"><span data-stu-id="c2b62-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c2b62-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2b62-123">Authorization</span></span>  | <span data-ttu-id="c2b62-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c2b62-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2b62-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2b62-126">Content-Type</span></span>   | <span data-ttu-id="c2b62-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c2b62-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2b62-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2b62-128">Request body</span></span>
<span data-ttu-id="c2b62-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c2b62-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2b62-130">响应</span><span class="sxs-lookup"><span data-stu-id="c2b62-130">Response</span></span>

<span data-ttu-id="c2b62-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [schemaExtension](../resources/schemaextension.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c2b62-131">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2b62-132">示例</span><span class="sxs-lookup"><span data-stu-id="c2b62-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2b62-133">请求</span><span class="sxs-lookup"><span data-stu-id="c2b62-133">Request</span></span>
<span data-ttu-id="c2b62-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c2b62-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2b62-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2b62-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/schemaExtensions/graphlearn_test
```
# <a name="c"></a>[<span data-ttu-id="c2b62-136">C#</span><span class="sxs-lookup"><span data-stu-id="c2b62-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2b62-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2b62-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2b62-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2b62-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c2b62-139">响应</span><span class="sxs-lookup"><span data-stu-id="c2b62-139">Response</span></span>
<span data-ttu-id="c2b62-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c2b62-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="c2b62-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c2b62-143">See also</span></span>

- [<span data-ttu-id="c2b62-144">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="c2b62-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c2b62-145">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="c2b62-145">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


