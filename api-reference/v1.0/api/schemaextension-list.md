---
title: 列出 schemaExtension
description: '获取您在当前租户中拥有的任何应用程序创建的 schemaExtension 对象的列表 (可 '
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 0c798a052974189a2dfb5373ad12c9810c4f11db
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975702"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="fa100-103">列出 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="fa100-103">List schemaExtensions</span></span>

<span data-ttu-id="fa100-104">获取您在当前租户中拥有的任何应用 (可以是**InDevelopment**、**可用**或弃用) 创建的[schemaExtension](../resources/schemaextension.md)对象的列表\*\*\*\*, 以及被标记为**的其他应用程序所拥有的其他所有架构扩展。可用**。</span><span class="sxs-lookup"><span data-stu-id="fa100-104">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fa100-105">权限</span><span class="sxs-lookup"><span data-stu-id="fa100-105">Permissions</span></span>
<span data-ttu-id="fa100-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fa100-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa100-108">Permission type</span></span>      | <span data-ttu-id="fa100-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa100-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa100-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa100-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fa100-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa100-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fa100-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa100-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa100-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa100-113">Not supported.</span></span>    |
|<span data-ttu-id="fa100-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa100-114">Application</span></span> | <span data-ttu-id="fa100-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa100-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa100-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa100-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fa100-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fa100-117">Optional query parameters</span></span>
<span data-ttu-id="fa100-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fa100-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa100-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa100-119">Request headers</span></span>
| <span data-ttu-id="fa100-120">名称</span><span class="sxs-lookup"><span data-stu-id="fa100-120">Name</span></span>      |<span data-ttu-id="fa100-121">说明</span><span class="sxs-lookup"><span data-stu-id="fa100-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fa100-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa100-122">Authorization</span></span>  | <span data-ttu-id="fa100-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa100-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa100-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa100-125">Content-Type</span></span>   | <span data-ttu-id="fa100-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa100-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa100-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa100-127">Request body</span></span>
<span data-ttu-id="fa100-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fa100-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa100-129">响应</span><span class="sxs-lookup"><span data-stu-id="fa100-129">Response</span></span>

<span data-ttu-id="fa100-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[schemaExtension](../resources/schemaextension.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="fa100-130">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fa100-131">示例</span><span class="sxs-lookup"><span data-stu-id="fa100-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa100-132">请求</span><span class="sxs-lookup"><span data-stu-id="fa100-132">Request</span></span>
<span data-ttu-id="fa100-133">下面的示例演示如何通过筛选其唯一**id**来查看特定项的所有可访问扩展。</span><span class="sxs-lookup"><span data-stu-id="fa100-133">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="fa100-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fa100-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa100-135">C#</span><span class="sxs-lookup"><span data-stu-id="fa100-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextensions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa100-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="fa100-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextensions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa100-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="fa100-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextensions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fa100-138">Java</span><span class="sxs-lookup"><span data-stu-id="fa100-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schemaextensions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fa100-139">响应</span><span class="sxs-lookup"><span data-stu-id="fa100-139">Response</span></span>
<span data-ttu-id="fa100-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa100-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="fa100-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fa100-143">See also</span></span>

- [<span data-ttu-id="fa100-144">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="fa100-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fa100-145">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="fa100-145">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
