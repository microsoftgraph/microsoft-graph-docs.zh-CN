---
title: 列出 schemaExtension
description: '获取在当前租户中拥有的任何应用创建的 schemaExtension 对象 (可以是 '
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 32ce5aea57fe4becee644d500cba043460ab825d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038955"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="b94b9-103">列出 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="b94b9-103">List schemaExtensions</span></span>

<span data-ttu-id="b94b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b94b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b94b9-105">获取由当前租户 (中拥有的任何应用创建的 [schemaExtension](../resources/schemaextension.md)对象的列表，这些应用可以是 **InDevelopment、Available** 或 **Deprecated**) ，以及标记为 Available 的其他应用所拥有的所有其他架构 **扩展。** </span><span class="sxs-lookup"><span data-stu-id="b94b9-105">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

> <span data-ttu-id="b94b9-106">**注意：** 该列表还将包含架构扩展定义 (标记为) `Available` 租户中其他开发人员创建的列表。</span><span class="sxs-lookup"><span data-stu-id="b94b9-106">**Note:** The list will also contain schema extension definitions (marked as `Available`) created by other developers from other tenants.</span></span> <span data-ttu-id="b94b9-107">这不同于仅返回租户特定数据的其他 API。</span><span class="sxs-lookup"><span data-stu-id="b94b9-107">This is different from other APIs that only return tenant-specific data.</span></span> <span data-ttu-id="b94b9-108">基于架构扩展定义创建的扩展数据特定于租户，并且只有显式授予权限的应用才能访问这些数据。</span><span class="sxs-lookup"><span data-stu-id="b94b9-108">Extension data created based on schema extension definitions is tenant-specific and can only be accessed by apps explicitly granted permission.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b94b9-109">权限</span><span class="sxs-lookup"><span data-stu-id="b94b9-109">Permissions</span></span>
<span data-ttu-id="b94b9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b94b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b94b9-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="b94b9-112">Permission type</span></span>      | <span data-ttu-id="b94b9-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b94b9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b94b9-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b94b9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b94b9-115">User.Read、Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="b94b9-115">User.Read, Application.Read.All</span></span>  |
|<span data-ttu-id="b94b9-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b94b9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b94b9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b94b9-117">Not supported.</span></span>    |
|<span data-ttu-id="b94b9-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b94b9-118">Application</span></span> | <span data-ttu-id="b94b9-119">Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="b94b9-119">Application.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b94b9-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b94b9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b94b9-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b94b9-121">Optional query parameters</span></span>
<span data-ttu-id="b94b9-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b94b9-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b94b9-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b94b9-123">Request headers</span></span>
| <span data-ttu-id="b94b9-124">名称</span><span class="sxs-lookup"><span data-stu-id="b94b9-124">Name</span></span>      |<span data-ttu-id="b94b9-125">说明</span><span class="sxs-lookup"><span data-stu-id="b94b9-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b94b9-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b94b9-126">Authorization</span></span>  | <span data-ttu-id="b94b9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b94b9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b94b9-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b94b9-129">Content-Type</span></span>   | <span data-ttu-id="b94b9-130">application/json</span><span class="sxs-lookup"><span data-stu-id="b94b9-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b94b9-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="b94b9-131">Request body</span></span>
<span data-ttu-id="b94b9-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b94b9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b94b9-133">响应</span><span class="sxs-lookup"><span data-stu-id="b94b9-133">Response</span></span>

<span data-ttu-id="b94b9-134">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [schemaExtension](../resources/schemaextension.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b94b9-134">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b94b9-135">示例</span><span class="sxs-lookup"><span data-stu-id="b94b9-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b94b9-136">请求</span><span class="sxs-lookup"><span data-stu-id="b94b9-136">Request</span></span>
<span data-ttu-id="b94b9-137">下面的示例演示如何通过筛选特定扩展的唯一 id 来查找其所有可访问 **的扩展**。</span><span class="sxs-lookup"><span data-stu-id="b94b9-137">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 

# <a name="http"></a>[<span data-ttu-id="b94b9-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b94b9-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
# <a name="c"></a>[<span data-ttu-id="b94b9-139">C#</span><span class="sxs-lookup"><span data-stu-id="b94b9-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextensions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b94b9-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b94b9-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextensions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b94b9-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b94b9-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextensions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b94b9-142">Java</span><span class="sxs-lookup"><span data-stu-id="b94b9-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schemaextensions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b94b9-143">响应</span><span class="sxs-lookup"><span data-stu-id="b94b9-143">Response</span></span>
<span data-ttu-id="b94b9-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b94b9-144">Here is an example of the response.</span></span> <span data-ttu-id="b94b9-145">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b94b9-145">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 274

{
  "value": [
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
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="b94b9-146">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b94b9-146">See also</span></span>

- [<span data-ttu-id="b94b9-147">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b94b9-147">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b94b9-148">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b94b9-148">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
