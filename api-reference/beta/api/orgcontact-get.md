---
title: 获取 orgContact
description: 检索 orgcontact 对象的属性和关系。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e7fac076640aeb4e09a94377b2ae600fe5f30949
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596858"
---
# <a name="get-orgcontact"></a><span data-ttu-id="0ca3c-103">获取 orgContact</span><span class="sxs-lookup"><span data-stu-id="0ca3c-103">Get orgContact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ca3c-104">检索 orgcontact 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0ca3c-104">Retrieve the properties and relationships of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ca3c-105">权限</span><span class="sxs-lookup"><span data-stu-id="0ca3c-105">Permissions</span></span>
<span data-ttu-id="0ca3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ca3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ca3c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ca3c-108">Permission type</span></span>      | <span data-ttu-id="0ca3c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ca3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ca3c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ca3c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ca3c-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0ca3c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0ca3c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ca3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ca3c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ca3c-113">Not supported.</span></span>    |
|<span data-ttu-id="0ca3c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ca3c-114">Application</span></span> | <span data-ttu-id="0ca3c-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ca3c-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ca3c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ca3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0ca3c-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0ca3c-117">Optional query parameters</span></span>
<span data-ttu-id="0ca3c-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0ca3c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ca3c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ca3c-119">Request headers</span></span>
| <span data-ttu-id="0ca3c-120">名称</span><span class="sxs-lookup"><span data-stu-id="0ca3c-120">Name</span></span>       | <span data-ttu-id="0ca3c-121">类型</span><span class="sxs-lookup"><span data-stu-id="0ca3c-121">Type</span></span> | <span data-ttu-id="0ca3c-122">说明</span><span class="sxs-lookup"><span data-stu-id="0ca3c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0ca3c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ca3c-123">Authorization</span></span>  | <span data-ttu-id="0ca3c-124">string</span><span class="sxs-lookup"><span data-stu-id="0ca3c-124">string</span></span>  | <span data-ttu-id="0ca3c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ca3c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ca3c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ca3c-127">Request body</span></span>
<span data-ttu-id="0ca3c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ca3c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ca3c-129">响应</span><span class="sxs-lookup"><span data-stu-id="0ca3c-129">Response</span></span>

<span data-ttu-id="0ca3c-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[orgContact](../resources/orgcontact.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0ca3c-130">If successful, this method returns a `200 OK` response code and [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ca3c-131">示例</span><span class="sxs-lookup"><span data-stu-id="0ca3c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ca3c-132">请求</span><span class="sxs-lookup"><span data-stu-id="0ca3c-132">Request</span></span>
<span data-ttu-id="0ca3c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ca3c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="0ca3c-134">响应</span><span class="sxs-lookup"><span data-stu-id="0ca3c-134">Response</span></span>
<span data-ttu-id="0ca3c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ca3c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "addresses":[
      {
        "city": "string",
        "countryOrRegion": "string",
        "officeLocation": "string",
        "postalCode": "string",
        "state": "string",
        "street": "string"
      }
  ],
  "companyName": "companyName-value",
  "department": "department-value",
  "displayName": "displayName-value",
  "phones":[
      {
        "type": "string",
        "number": "string"
      }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0ca3c-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="0ca3c-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0ca3c-139">语言</span><span class="sxs-lookup"><span data-stu-id="0ca3c-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_orgcontact-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ca3c-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="0ca3c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_orgcontact-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
