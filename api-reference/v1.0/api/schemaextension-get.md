---
title: 获取 schemaExtension
description: 获取指定的 schemaExtension 定义的属性。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 70a4fdc5e51a5965098a6b0331a31c200b553ec9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521031"
---
# <a name="get-schemaextension"></a><span data-ttu-id="e9387-103">获取 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="e9387-103">Get schemaExtension</span></span>
<span data-ttu-id="e9387-104">获取指定的[schemaExtension](../resources/schemaextension.md)定义的属性。</span><span class="sxs-lookup"><span data-stu-id="e9387-104">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9387-105">权限</span><span class="sxs-lookup"><span data-stu-id="e9387-105">Permissions</span></span>
<span data-ttu-id="e9387-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9387-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e9387-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9387-108">Permission type</span></span>      | <span data-ttu-id="e9387-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e9387-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9387-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9387-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e9387-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e9387-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e9387-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9387-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9387-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9387-113">Not supported.</span></span>    |
|<span data-ttu-id="e9387-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9387-114">Application</span></span> | <span data-ttu-id="e9387-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9387-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9387-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9387-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e9387-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e9387-117">Optional query parameters</span></span>
<span data-ttu-id="e9387-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e9387-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9387-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9387-119">Request headers</span></span>
| <span data-ttu-id="e9387-120">名称</span><span class="sxs-lookup"><span data-stu-id="e9387-120">Name</span></span>      |<span data-ttu-id="e9387-121">说明</span><span class="sxs-lookup"><span data-stu-id="e9387-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e9387-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9387-122">Authorization</span></span>  | <span data-ttu-id="e9387-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e9387-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9387-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9387-125">Content-Type</span></span>   | <span data-ttu-id="e9387-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9387-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9387-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9387-127">Request body</span></span>
<span data-ttu-id="e9387-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e9387-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9387-129">响应</span><span class="sxs-lookup"><span data-stu-id="e9387-129">Response</span></span>

<span data-ttu-id="e9387-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[schemaExtension](../resources/schemaextension.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e9387-130">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e9387-131">示例</span><span class="sxs-lookup"><span data-stu-id="e9387-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9387-132">请求</span><span class="sxs-lookup"><span data-stu-id="e9387-132">Request</span></span>
<span data-ttu-id="e9387-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e9387-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="e9387-134">响应</span><span class="sxs-lookup"><span data-stu-id="e9387-134">Response</span></span>
<span data-ttu-id="e9387-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e9387-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e9387-138">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e9387-138">See also</span></span>

- [<span data-ttu-id="e9387-139">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e9387-139">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e9387-140">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e9387-140">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
