---
title: 列出 orgContacts
description: 检索此组织的组织联系人列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 24d0a809bf7cb5c8a32eec0d6cb81f17e7f799a6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511157"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="c311c-103">列出 orgContacts</span><span class="sxs-lookup"><span data-stu-id="c311c-103">List orgContacts</span></span>

<span data-ttu-id="c311c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c311c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c311c-105">获取此组织的[组织联系人](../resources/orgcontact.md)列表。</span><span class="sxs-lookup"><span data-stu-id="c311c-105">Get the list of [organizational contacts](../resources/orgcontact.md) for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="c311c-106">权限</span><span class="sxs-lookup"><span data-stu-id="c311c-106">Permissions</span></span>
<span data-ttu-id="c311c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c311c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c311c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c311c-109">Permission type</span></span>      | <span data-ttu-id="c311c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c311c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c311c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c311c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c311c-112">OrgContact、Directory.accessasuser.all、所有的目录、所有、和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="c311c-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c311c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c311c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c311c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c311c-114">Not supported.</span></span>    |
|<span data-ttu-id="c311c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c311c-115">Application</span></span> | <span data-ttu-id="c311c-116">OrgContact、所有目录、全部读取、所有读写。</span><span class="sxs-lookup"><span data-stu-id="c311c-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c311c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c311c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c311c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c311c-118">Optional query parameters</span></span>
<span data-ttu-id="c311c-119">此方法支持`$expand`、 `$filter`、 `$select`和`$top` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c311c-119">This method supports the `$expand`, `$filter`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c311c-120">请求头</span><span class="sxs-lookup"><span data-stu-id="c311c-120">Request headers</span></span>
| <span data-ttu-id="c311c-121">标头</span><span class="sxs-lookup"><span data-stu-id="c311c-121">Header</span></span>       | <span data-ttu-id="c311c-122">值</span><span class="sxs-lookup"><span data-stu-id="c311c-122">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c311c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c311c-123">Authorization</span></span>  |<span data-ttu-id="c311c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c311c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c311c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c311c-126">Request body</span></span>
<span data-ttu-id="c311c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c311c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c311c-128">响应</span><span class="sxs-lookup"><span data-stu-id="c311c-128">Response</span></span>

<span data-ttu-id="c311c-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[orgContact](../resources/orgcontact.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c311c-129">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c311c-130">示例</span><span class="sxs-lookup"><span data-stu-id="c311c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c311c-131">请求</span><span class="sxs-lookup"><span data-stu-id="c311c-131">Request</span></span>
<span data-ttu-id="c311c-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c311c-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c311c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c311c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts
```
# <a name="c"></a>[<span data-ttu-id="c311c-134">C#</span><span class="sxs-lookup"><span data-stu-id="c311c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c311c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c311c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c311c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c311c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c311c-137">Java</span><span class="sxs-lookup"><span data-stu-id="c311c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c311c-138">响应</span><span class="sxs-lookup"><span data-stu-id="c311c-138">Response</span></span>
<span data-ttu-id="c311c-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c311c-139">The following is an example of the response.</span></span>
><span data-ttu-id="c311c-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c311c-140">**Note**: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
