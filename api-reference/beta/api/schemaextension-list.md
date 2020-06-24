---
title: 列出 schemaExtension
description: '获取您在当前租户中拥有的任何应用程序创建的 schemaExtension 对象的列表（可 '
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 1c43bd8227b80661c7194e8269dfce3ee76d0f96
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863479"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="5f062-103">列出 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="5f062-103">List schemaExtensions</span></span>

<span data-ttu-id="5f062-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f062-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f062-105">获取您在当前租户中拥有的任何应用程序（可以是**InDevelopment**、**可用**或**弃用**）创建的[schemaExtension](../resources/schemaextension.md)对象的列表，以及标记为**可用**的其他应用程序所拥有的其他所有架构扩展。</span><span class="sxs-lookup"><span data-stu-id="5f062-105">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

> <span data-ttu-id="5f062-106">**注意：** 此列表还将包含 `Available` 其他租户从其他租户创建的架构扩展定义（标记为）。</span><span class="sxs-lookup"><span data-stu-id="5f062-106">**Note:** The list will also contain schema extension definitions (marked as `Available`) created by other developers from other tenants.</span></span> <span data-ttu-id="5f062-107">这不同于仅返回租户特定数据的其他 Api。</span><span class="sxs-lookup"><span data-stu-id="5f062-107">This is different from other APIs that only return tenant-specific data.</span></span> <span data-ttu-id="5f062-108">基于架构扩展定义创建的扩展数据是租户特定的，并且只能由明确授予权限的应用程序访问。</span><span class="sxs-lookup"><span data-stu-id="5f062-108">Extension data created based on schema extension definitions is tenant-specific and can only be accessed by apps explicitly granted permission.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5f062-109">权限</span><span class="sxs-lookup"><span data-stu-id="5f062-109">Permissions</span></span>
<span data-ttu-id="5f062-110">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5f062-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5f062-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f062-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5f062-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f062-112">Permission type</span></span>      | <span data-ttu-id="5f062-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f062-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f062-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f062-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5f062-115">Read、Application. All</span><span class="sxs-lookup"><span data-stu-id="5f062-115">User.Read, Application.Read.All</span></span>   |
|<span data-ttu-id="5f062-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f062-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f062-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f062-117">Not supported.</span></span>    |
|<span data-ttu-id="5f062-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f062-118">Application</span></span> | <span data-ttu-id="5f062-119">Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f062-119">Application.Read.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5f062-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f062-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5f062-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5f062-121">Optional query parameters</span></span>
<span data-ttu-id="5f062-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5f062-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f062-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f062-123">Request headers</span></span>
| <span data-ttu-id="5f062-124">名称</span><span class="sxs-lookup"><span data-stu-id="5f062-124">Name</span></span>      |<span data-ttu-id="5f062-125">说明</span><span class="sxs-lookup"><span data-stu-id="5f062-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5f062-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f062-126">Authorization</span></span>  | <span data-ttu-id="5f062-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="5f062-127">Bearer {token}.</span></span> <span data-ttu-id="5f062-128">Required.</span><span class="sxs-lookup"><span data-stu-id="5f062-128">Required.</span></span> |
| <span data-ttu-id="5f062-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f062-129">Content-Type</span></span>   | <span data-ttu-id="5f062-130">application/json</span><span class="sxs-lookup"><span data-stu-id="5f062-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f062-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f062-131">Request body</span></span>
<span data-ttu-id="5f062-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5f062-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f062-133">响应</span><span class="sxs-lookup"><span data-stu-id="5f062-133">Response</span></span>

<span data-ttu-id="5f062-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[schemaExtension](../resources/schemaextension.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="5f062-134">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5f062-135">示例</span><span class="sxs-lookup"><span data-stu-id="5f062-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f062-136">请求</span><span class="sxs-lookup"><span data-stu-id="5f062-136">Request</span></span>
<span data-ttu-id="5f062-137">下面的示例演示如何通过筛选其唯一**id**来查看特定项的所有可访问扩展。</span><span class="sxs-lookup"><span data-stu-id="5f062-137">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 

# <a name="http"></a>[<span data-ttu-id="5f062-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f062-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
# <a name="c"></a>[<span data-ttu-id="5f062-139">C#</span><span class="sxs-lookup"><span data-stu-id="5f062-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextensions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f062-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f062-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextensions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f062-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f062-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextensions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5f062-142">响应</span><span class="sxs-lookup"><span data-stu-id="5f062-142">Response</span></span>
<span data-ttu-id="5f062-143">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="5f062-143">Here is an example of the response.</span></span> <span data-ttu-id="5f062-144">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="5f062-144">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5f062-145">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5f062-145">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="5f062-146">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5f062-146">See also</span></span>

- [<span data-ttu-id="5f062-147">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="5f062-147">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5f062-148">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="5f062-148">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
