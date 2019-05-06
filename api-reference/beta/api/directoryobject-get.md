---
title: 获取 directoryObject
description: 检索 directoryobject 对象的属性和关系。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 075ab1ddd6a588993e94337a48a619a3ad6cda69
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590630"
---
# <a name="get-directoryobject"></a><span data-ttu-id="3ca1c-103">获取 directoryObject</span><span class="sxs-lookup"><span data-stu-id="3ca1c-103">Get directoryObject</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ca1c-104">检索 directoryobject 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3ca1c-104">Retrieve the properties and relationships of directoryobject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3ca1c-105">权限</span><span class="sxs-lookup"><span data-stu-id="3ca1c-105">Permissions</span></span>
<span data-ttu-id="3ca1c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ca1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ca1c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ca1c-108">Permission type</span></span>      | <span data-ttu-id="3ca1c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ca1c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ca1c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ca1c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3ca1c-111">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ca1c-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3ca1c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ca1c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ca1c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ca1c-113">Not supported.</span></span>    |
|<span data-ttu-id="3ca1c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ca1c-114">Application</span></span> | <span data-ttu-id="3ca1c-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ca1c-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ca1c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ca1c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3ca1c-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3ca1c-117">Optional query parameters</span></span>
<span data-ttu-id="3ca1c-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3ca1c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3ca1c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ca1c-119">Request headers</span></span>
| <span data-ttu-id="3ca1c-120">名称</span><span class="sxs-lookup"><span data-stu-id="3ca1c-120">Name</span></span>       | <span data-ttu-id="3ca1c-121">类型</span><span class="sxs-lookup"><span data-stu-id="3ca1c-121">Type</span></span> | <span data-ttu-id="3ca1c-122">说明</span><span class="sxs-lookup"><span data-stu-id="3ca1c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3ca1c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ca1c-123">Authorization</span></span>  | <span data-ttu-id="3ca1c-124">string</span><span class="sxs-lookup"><span data-stu-id="3ca1c-124">string</span></span>  | <span data-ttu-id="3ca1c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ca1c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ca1c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ca1c-127">Request body</span></span>
<span data-ttu-id="3ca1c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3ca1c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ca1c-129">响应</span><span class="sxs-lookup"><span data-stu-id="3ca1c-129">Response</span></span>

<span data-ttu-id="3ca1c-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3ca1c-130">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3ca1c-131">示例</span><span class="sxs-lookup"><span data-stu-id="3ca1c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ca1c-132">请求</span><span class="sxs-lookup"><span data-stu-id="3ca1c-132">Request</span></span>
<span data-ttu-id="3ca1c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ca1c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```http
GET https://graph.microsoft.com/beta/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="3ca1c-134">响应</span><span class="sxs-lookup"><span data-stu-id="3ca1c-134">Response</span></span>
<span data-ttu-id="3ca1c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3ca1c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 22

{
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3ca1c-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3ca1c-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3ca1c-139">语言</span><span class="sxs-lookup"><span data-stu-id="3ca1c-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directoryobject-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3ca1c-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="3ca1c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directoryobject-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryobject-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
