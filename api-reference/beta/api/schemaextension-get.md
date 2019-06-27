---
title: 获取 schemaExtension
description: 获取指定的 schemaExtension 定义的属性。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: c93e8e588c6e49e034bae7cd7ae67b94d258c38f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263978"
---
# <a name="get-schemaextension"></a><span data-ttu-id="54407-103">获取 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="54407-103">Get schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54407-104">获取指定的[schemaExtension](../resources/schemaextension.md)定义的属性。</span><span class="sxs-lookup"><span data-stu-id="54407-104">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="54407-105">权限</span><span class="sxs-lookup"><span data-stu-id="54407-105">Permissions</span></span>
<span data-ttu-id="54407-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="54407-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="54407-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="54407-108">Permission type</span></span>      | <span data-ttu-id="54407-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="54407-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54407-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="54407-110">Delegated (work or school account)</span></span> | <span data-ttu-id="54407-111">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="54407-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="54407-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="54407-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54407-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="54407-113">Not supported.</span></span>    |
|<span data-ttu-id="54407-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="54407-114">Application</span></span> | <span data-ttu-id="54407-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="54407-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54407-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="54407-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="54407-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="54407-117">Optional query parameters</span></span>
<span data-ttu-id="54407-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="54407-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54407-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="54407-119">Request headers</span></span>
| <span data-ttu-id="54407-120">名称</span><span class="sxs-lookup"><span data-stu-id="54407-120">Name</span></span>      |<span data-ttu-id="54407-121">说明</span><span class="sxs-lookup"><span data-stu-id="54407-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="54407-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="54407-122">Authorization</span></span>  | <span data-ttu-id="54407-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="54407-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54407-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54407-125">Content-Type</span></span>   | <span data-ttu-id="54407-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54407-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="54407-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="54407-127">Request body</span></span>
<span data-ttu-id="54407-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="54407-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54407-129">响应</span><span class="sxs-lookup"><span data-stu-id="54407-129">Response</span></span>

<span data-ttu-id="54407-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[schemaExtension](../resources/schemaextension.md)对象。</span><span class="sxs-lookup"><span data-stu-id="54407-130">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="54407-131">示例</span><span class="sxs-lookup"><span data-stu-id="54407-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54407-132">请求</span><span class="sxs-lookup"><span data-stu-id="54407-132">Request</span></span>
<span data-ttu-id="54407-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="54407-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/beta/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="54407-134">响应</span><span class="sxs-lookup"><span data-stu-id="54407-134">Response</span></span>
<span data-ttu-id="54407-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="54407-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="54407-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="54407-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="54407-139">C#</span><span class="sxs-lookup"><span data-stu-id="54407-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_schemaextension-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="54407-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="54407-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_schemaextension-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="54407-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="54407-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_schemaextension-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="54407-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="54407-142">See also</span></span>

- [<span data-ttu-id="54407-143">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="54407-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="54407-144">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="54407-144">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/schemaextension-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/schemaextension-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schemaextension-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
