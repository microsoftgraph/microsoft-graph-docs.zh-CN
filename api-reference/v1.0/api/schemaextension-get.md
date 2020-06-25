---
title: 获取 schemaExtension
description: 获取指定的 schemaExtension 定义的属性。
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: 194b1ecbb31c6674ac8e285792d302fc2ee4ae76
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863142"
---
# <a name="get-schemaextension"></a><span data-ttu-id="a656f-103">获取 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="a656f-103">Get schemaExtension</span></span>

<span data-ttu-id="a656f-104">命名空间： microsoft. graph 获取指定的[schemaExtension](../resources/schemaextension.md)定义的属性。</span><span class="sxs-lookup"><span data-stu-id="a656f-104">Namespace: microsoft.graph Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="a656f-105">权限</span><span class="sxs-lookup"><span data-stu-id="a656f-105">Permissions</span></span>
<span data-ttu-id="a656f-106">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a656f-106">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a656f-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a656f-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a656f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a656f-108">Permission type</span></span>      | <span data-ttu-id="a656f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a656f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a656f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a656f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a656f-111">Read、Application. All</span><span class="sxs-lookup"><span data-stu-id="a656f-111">User.Read, Application.Read.All</span></span>    |
|<span data-ttu-id="a656f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a656f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a656f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a656f-113">Not supported.</span></span>    |
|<span data-ttu-id="a656f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a656f-114">Application</span></span> | <span data-ttu-id="a656f-115">Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="a656f-115">Application.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a656f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a656f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a656f-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a656f-117">Optional query parameters</span></span>
<span data-ttu-id="a656f-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a656f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a656f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a656f-119">Request headers</span></span>
| <span data-ttu-id="a656f-120">名称</span><span class="sxs-lookup"><span data-stu-id="a656f-120">Name</span></span>      |<span data-ttu-id="a656f-121">说明</span><span class="sxs-lookup"><span data-stu-id="a656f-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a656f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a656f-122">Authorization</span></span>  | <span data-ttu-id="a656f-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="a656f-123">Bearer {token}.</span></span> <span data-ttu-id="a656f-124">Required.</span><span class="sxs-lookup"><span data-stu-id="a656f-124">Required.</span></span> |
| <span data-ttu-id="a656f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a656f-125">Content-Type</span></span>   | <span data-ttu-id="a656f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a656f-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a656f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a656f-127">Request body</span></span>
<span data-ttu-id="a656f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a656f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a656f-129">响应</span><span class="sxs-lookup"><span data-stu-id="a656f-129">Response</span></span>

<span data-ttu-id="a656f-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[schemaExtension](../resources/schemaextension.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a656f-130">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a656f-131">示例</span><span class="sxs-lookup"><span data-stu-id="a656f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a656f-132">请求</span><span class="sxs-lookup"><span data-stu-id="a656f-132">Request</span></span>
<span data-ttu-id="a656f-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a656f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="a656f-134">响应</span><span class="sxs-lookup"><span data-stu-id="a656f-134">Response</span></span>
<span data-ttu-id="a656f-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="a656f-135">Here is an example of the response.</span></span> <span data-ttu-id="a656f-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="a656f-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a656f-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a656f-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
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

## <a name="see-also"></a><span data-ttu-id="a656f-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a656f-138">See also</span></span>

- [<span data-ttu-id="a656f-139">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="a656f-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a656f-140">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="a656f-140">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
