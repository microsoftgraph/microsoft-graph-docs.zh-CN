---
title: 获取 orgContact
description: 检索 orgContact 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3f3ed6d94a51809b9c3838b5e9cb6972f824db5a
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37633977"
---
# <a name="get-orgcontact"></a><span data-ttu-id="efd3c-103">获取 orgContact</span><span class="sxs-lookup"><span data-stu-id="efd3c-103">Get orgContact</span></span>

<span data-ttu-id="efd3c-104">获取[组织联系人](../resources/orgcontact.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="efd3c-104">Get the properties and relationships of an [organizational contact](../resources/orgcontact.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="efd3c-105">权限</span><span class="sxs-lookup"><span data-stu-id="efd3c-105">Permissions</span></span>
<span data-ttu-id="efd3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efd3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efd3c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="efd3c-108">Permission type</span></span>      | <span data-ttu-id="efd3c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="efd3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efd3c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efd3c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="efd3c-111">OrgContact、Directory.accessasuser.all、所有的目录、所有、和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="efd3c-111">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="efd3c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efd3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efd3c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="efd3c-113">Not supported.</span></span>    |
|<span data-ttu-id="efd3c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="efd3c-114">Application</span></span> | <span data-ttu-id="efd3c-115">OrgContact、所有目录、全部读取、所有读写。</span><span class="sxs-lookup"><span data-stu-id="efd3c-115">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="efd3c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efd3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="efd3c-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="efd3c-117">Optional query parameters</span></span>
<span data-ttu-id="efd3c-118">此方法支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="efd3c-118">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="efd3c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="efd3c-119">Request headers</span></span>
| <span data-ttu-id="efd3c-120">标头</span><span class="sxs-lookup"><span data-stu-id="efd3c-120">Header</span></span>       | <span data-ttu-id="efd3c-121">值</span><span class="sxs-lookup"><span data-stu-id="efd3c-121">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="efd3c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="efd3c-122">Authorization</span></span>  | <span data-ttu-id="efd3c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="efd3c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="efd3c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="efd3c-125">Request body</span></span>
<span data-ttu-id="efd3c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="efd3c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efd3c-127">响应</span><span class="sxs-lookup"><span data-stu-id="efd3c-127">Response</span></span>

<span data-ttu-id="efd3c-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[orgContact](../resources/orgcontact.md)对象。</span><span class="sxs-lookup"><span data-stu-id="efd3c-128">If successful, this method returns a `200 OK` response code and an [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="efd3c-129">示例</span><span class="sxs-lookup"><span data-stu-id="efd3c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="efd3c-130">请求</span><span class="sxs-lookup"><span data-stu-id="efd3c-130">Request</span></span>
<span data-ttu-id="efd3c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="efd3c-131">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="efd3c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="efd3c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="efd3c-133">C#</span><span class="sxs-lookup"><span data-stu-id="efd3c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="efd3c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="efd3c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="efd3c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="efd3c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="efd3c-136">Java</span><span class="sxs-lookup"><span data-stu-id="efd3c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="efd3c-137">响应</span><span class="sxs-lookup"><span data-stu-id="efd3c-137">Response</span></span>
<span data-ttu-id="efd3c-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="efd3c-138">The following is an example of the response.</span></span>
><span data-ttu-id="efd3c-139">**注意**：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="efd3c-139">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
