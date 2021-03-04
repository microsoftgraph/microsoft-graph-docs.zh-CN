---
title: 获取 orgContact
description: 检索 orgcontact 对象的属性和关系。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3a4e960ba30d666df5bec9c85135c874ca6394d8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447785"
---
# <a name="get-orgcontact"></a><span data-ttu-id="64a97-103">获取 orgContact</span><span class="sxs-lookup"><span data-stu-id="64a97-103">Get orgContact</span></span>

<span data-ttu-id="64a97-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64a97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64a97-105">获取组织联系人对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="64a97-105">Get the properties and relationships of an organizational contact object.</span></span>

## <a name="permissions"></a><span data-ttu-id="64a97-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="64a97-106">Permissions</span></span>
<span data-ttu-id="64a97-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64a97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64a97-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="64a97-109">Permission type</span></span>      | <span data-ttu-id="64a97-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64a97-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64a97-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64a97-111">Delegated (work or school account)</span></span> | <span data-ttu-id="64a97-112">OrgContact.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64a97-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="64a97-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64a97-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64a97-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="64a97-114">Not supported.</span></span>    |
|<span data-ttu-id="64a97-115">Application</span><span class="sxs-lookup"><span data-stu-id="64a97-115">Application</span></span> | <span data-ttu-id="64a97-116">OrgContact.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64a97-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64a97-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64a97-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="64a97-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="64a97-118">Optional query parameters</span></span>
<span data-ttu-id="64a97-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="64a97-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64a97-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="64a97-120">Request headers</span></span>
| <span data-ttu-id="64a97-121">名称</span><span class="sxs-lookup"><span data-stu-id="64a97-121">Name</span></span>       | <span data-ttu-id="64a97-122">类型</span><span class="sxs-lookup"><span data-stu-id="64a97-122">Type</span></span> | <span data-ttu-id="64a97-123">说明</span><span class="sxs-lookup"><span data-stu-id="64a97-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="64a97-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="64a97-124">Authorization</span></span>  | <span data-ttu-id="64a97-125">string</span><span class="sxs-lookup"><span data-stu-id="64a97-125">string</span></span>  | <span data-ttu-id="64a97-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="64a97-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64a97-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="64a97-128">Request body</span></span>
<span data-ttu-id="64a97-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="64a97-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64a97-130">响应</span><span class="sxs-lookup"><span data-stu-id="64a97-130">Response</span></span>

<span data-ttu-id="64a97-131">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [orgContact](../resources/orgcontact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64a97-131">If successful, this method returns a `200 OK` response code and [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="64a97-132">示例</span><span class="sxs-lookup"><span data-stu-id="64a97-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64a97-133">请求</span><span class="sxs-lookup"><span data-stu-id="64a97-133">Request</span></span>
<span data-ttu-id="64a97-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64a97-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64a97-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="64a97-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="64a97-136">C#</span><span class="sxs-lookup"><span data-stu-id="64a97-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64a97-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64a97-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64a97-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64a97-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64a97-139">Java</span><span class="sxs-lookup"><span data-stu-id="64a97-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="64a97-140">响应</span><span class="sxs-lookup"><span data-stu-id="64a97-140">Response</span></span>
<span data-ttu-id="64a97-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="64a97-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact"
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
  ]
}
-->
