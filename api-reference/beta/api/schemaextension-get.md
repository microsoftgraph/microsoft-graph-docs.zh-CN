---
title: 获取 schemaExtension
description: 获取指定的 schemaExtension 定义的属性。
ms.openlocfilehash: 32376d6afd0d6171362db1978b708610d9f4d056
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047275"
---
# <a name="get-schemaextension"></a><span data-ttu-id="d775c-103">获取 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="d775c-103">Get schemaExtension</span></span>

> <span data-ttu-id="d775c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d775c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d775c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d775c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d775c-106">获取指定的 [schemaExtension](../resources/schemaextension.md) 定义的属性。</span><span class="sxs-lookup"><span data-stu-id="d775c-106">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="d775c-107">权限</span><span class="sxs-lookup"><span data-stu-id="d775c-107">Permissions</span></span>
<span data-ttu-id="d775c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d775c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d775c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d775c-110">Permission type</span></span>      | <span data-ttu-id="d775c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d775c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d775c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d775c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d775c-113">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d775c-113">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d775c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d775c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d775c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d775c-115">Not supported.</span></span>    |
|<span data-ttu-id="d775c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d775c-116">Application</span></span> | <span data-ttu-id="d775c-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d775c-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d775c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d775c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d775c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d775c-119">Optional query parameters</span></span>
<span data-ttu-id="d775c-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d775c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d775c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d775c-121">Request headers</span></span>
| <span data-ttu-id="d775c-122">名称</span><span class="sxs-lookup"><span data-stu-id="d775c-122">Name</span></span>      |<span data-ttu-id="d775c-123">说明</span><span class="sxs-lookup"><span data-stu-id="d775c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d775c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d775c-124">Authorization</span></span>  | <span data-ttu-id="d775c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d775c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d775c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d775c-127">Content-Type</span></span>   | <span data-ttu-id="d775c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d775c-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d775c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d775c-129">Request body</span></span>
<span data-ttu-id="d775c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d775c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d775c-131">响应</span><span class="sxs-lookup"><span data-stu-id="d775c-131">Response</span></span>

<span data-ttu-id="d775c-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [schemaExtension](../resources/schemaextension.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d775c-132">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d775c-133">示例</span><span class="sxs-lookup"><span data-stu-id="d775c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d775c-134">请求</span><span class="sxs-lookup"><span data-stu-id="d775c-134">Request</span></span>
<span data-ttu-id="d775c-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d775c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/beta/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="d775c-136">响应</span><span class="sxs-lookup"><span data-stu-id="d775c-136">Response</span></span>
<span data-ttu-id="d775c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d775c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d775c-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d775c-140">See also</span></span>

- [<span data-ttu-id="d775c-141">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="d775c-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d775c-142">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="d775c-142">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->