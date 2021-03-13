---
title: 获取 orgContact
description: 检索 orgContact 对象的属性。
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: f3702f51779bfb42d794aa011bc671b5b7dd99d3
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761649"
---
# <a name="get-orgcontact"></a><span data-ttu-id="bb2b8-103">获取 orgContact</span><span class="sxs-lookup"><span data-stu-id="bb2b8-103">Get orgContact</span></span>

<span data-ttu-id="bb2b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb2b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bb2b8-105">获取组织联系人的属性 [和关系](../resources/orgcontact.md)。</span><span class="sxs-lookup"><span data-stu-id="bb2b8-105">Get the properties and relationships of an [organizational contact](../resources/orgcontact.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bb2b8-106">权限</span><span class="sxs-lookup"><span data-stu-id="bb2b8-106">Permissions</span></span>
<span data-ttu-id="bb2b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb2b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb2b8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb2b8-109">Permission type</span></span>      | <span data-ttu-id="bb2b8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb2b8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb2b8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb2b8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bb2b8-112">OrgContact.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bb2b8-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bb2b8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb2b8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb2b8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb2b8-114">Not supported.</span></span>    |
|<span data-ttu-id="bb2b8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb2b8-115">Application</span></span> | <span data-ttu-id="bb2b8-116">OrgContact.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb2b8-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb2b8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb2b8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bb2b8-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bb2b8-118">Optional query parameters</span></span>
<span data-ttu-id="bb2b8-119">此方法支持`$select` 和 `$expand` [OData 查询参数](/graph/query-parameters)，以帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bb2b8-119">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb2b8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb2b8-120">Request headers</span></span>
| <span data-ttu-id="bb2b8-121">标头</span><span class="sxs-lookup"><span data-stu-id="bb2b8-121">Header</span></span>       | <span data-ttu-id="bb2b8-122">值</span><span class="sxs-lookup"><span data-stu-id="bb2b8-122">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="bb2b8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb2b8-123">Authorization</span></span>  | <span data-ttu-id="bb2b8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bb2b8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb2b8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb2b8-126">Request body</span></span>
<span data-ttu-id="bb2b8-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb2b8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb2b8-128">响应</span><span class="sxs-lookup"><span data-stu-id="bb2b8-128">Response</span></span>

<span data-ttu-id="bb2b8-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [orgContact](../resources/orgcontact.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb2b8-129">If successful, this method returns a `200 OK` response code and an [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb2b8-130">示例</span><span class="sxs-lookup"><span data-stu-id="bb2b8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb2b8-131">请求</span><span class="sxs-lookup"><span data-stu-id="bb2b8-131">Request</span></span>
<span data-ttu-id="bb2b8-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bb2b8-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bb2b8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb2b8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="bb2b8-134">C#</span><span class="sxs-lookup"><span data-stu-id="bb2b8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb2b8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb2b8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb2b8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb2b8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb2b8-137">Java</span><span class="sxs-lookup"><span data-stu-id="bb2b8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bb2b8-138">响应</span><span class="sxs-lookup"><span data-stu-id="bb2b8-138">Response</span></span>
<span data-ttu-id="bb2b8-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bb2b8-139">The following is an example of the response.</span></span>
><span data-ttu-id="bb2b8-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bb2b8-140">**Note**: The response object shown here might be shortened for readability.</span></span> 
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

