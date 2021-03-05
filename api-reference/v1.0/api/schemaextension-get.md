---
title: 获取 schemaExtension
description: 获取指定 schemaExtension 定义的属性。
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 2b08b4600a729af8289c2592a023b95a0e73a182
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474500"
---
# <a name="get-schemaextension"></a><span data-ttu-id="e6215-103">获取 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="e6215-103">Get schemaExtension</span></span>

<span data-ttu-id="e6215-104">命名空间：microsoft.graph 获取指定 [schemaExtension 定义](../resources/schemaextension.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="e6215-104">Namespace: microsoft.graph Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6215-105">权限</span><span class="sxs-lookup"><span data-stu-id="e6215-105">Permissions</span></span>
<span data-ttu-id="e6215-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6215-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e6215-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6215-108">Permission type</span></span>      | <span data-ttu-id="e6215-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6215-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6215-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6215-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e6215-111">User.Read、Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6215-111">User.Read, Application.Read.All</span></span>    |
|<span data-ttu-id="e6215-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6215-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6215-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6215-113">Not supported.</span></span>    |
|<span data-ttu-id="e6215-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6215-114">Application</span></span> | <span data-ttu-id="e6215-115">Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6215-115">Application.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6215-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6215-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e6215-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e6215-117">Optional query parameters</span></span>
<span data-ttu-id="e6215-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e6215-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6215-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6215-119">Request headers</span></span>
| <span data-ttu-id="e6215-120">名称</span><span class="sxs-lookup"><span data-stu-id="e6215-120">Name</span></span>      |<span data-ttu-id="e6215-121">说明</span><span class="sxs-lookup"><span data-stu-id="e6215-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e6215-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6215-122">Authorization</span></span>  | <span data-ttu-id="e6215-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6215-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e6215-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6215-125">Content-Type</span></span>   | <span data-ttu-id="e6215-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6215-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6215-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6215-127">Request body</span></span>
<span data-ttu-id="e6215-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e6215-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6215-129">响应</span><span class="sxs-lookup"><span data-stu-id="e6215-129">Response</span></span>

<span data-ttu-id="e6215-130">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [schemaExtension](../resources/schemaextension.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e6215-130">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e6215-131">示例</span><span class="sxs-lookup"><span data-stu-id="e6215-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6215-132">请求</span><span class="sxs-lookup"><span data-stu-id="e6215-132">Request</span></span>
<span data-ttu-id="e6215-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6215-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e6215-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6215-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/schemaExtensions/graphlearn_test
```
# <a name="c"></a>[<span data-ttu-id="e6215-135">C#</span><span class="sxs-lookup"><span data-stu-id="e6215-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6215-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6215-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6215-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6215-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6215-138">Java</span><span class="sxs-lookup"><span data-stu-id="e6215-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e6215-139">响应</span><span class="sxs-lookup"><span data-stu-id="e6215-139">Response</span></span>
<span data-ttu-id="e6215-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6215-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e6215-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e6215-143">See also</span></span>

- [<span data-ttu-id="e6215-144">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e6215-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e6215-145">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e6215-145">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
