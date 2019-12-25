---
title: 列出 directReports
description: 获取联系人的直接下属。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2fe1300415a4511258edd530f81705f22f9d2209
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864612"
---
# <a name="list-directreports"></a><span data-ttu-id="65aee-103">列出 directReports</span><span class="sxs-lookup"><span data-stu-id="65aee-103">List directReports</span></span>

<span data-ttu-id="65aee-104">获取此[组织联系人](../resources/orgcontact.md)的直接下属。</span><span class="sxs-lookup"><span data-stu-id="65aee-104">Get the direct reports for this [organizational contact](../resources/orgcontact.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="65aee-105">权限</span><span class="sxs-lookup"><span data-stu-id="65aee-105">Permissions</span></span>
<span data-ttu-id="65aee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65aee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65aee-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="65aee-108">Permission type</span></span>      | <span data-ttu-id="65aee-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65aee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65aee-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65aee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="65aee-111">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="65aee-111">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="65aee-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65aee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65aee-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="65aee-113">Not supported.</span></span>    |
|<span data-ttu-id="65aee-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="65aee-114">Application</span></span> | <span data-ttu-id="65aee-115">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="65aee-115">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="65aee-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65aee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="65aee-117">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="65aee-117">Optional query parameters</span></span>
<span data-ttu-id="65aee-118">此方法支持`$select` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="65aee-118">This method supports the `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65aee-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="65aee-119">Request headers</span></span>
| <span data-ttu-id="65aee-120">标头</span><span class="sxs-lookup"><span data-stu-id="65aee-120">Header</span></span>       | <span data-ttu-id="65aee-121">值</span><span class="sxs-lookup"><span data-stu-id="65aee-121">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="65aee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="65aee-122">Authorization</span></span>  | <span data-ttu-id="65aee-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65aee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65aee-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="65aee-125">Request body</span></span>
<span data-ttu-id="65aee-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="65aee-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65aee-127">响应</span><span class="sxs-lookup"><span data-stu-id="65aee-127">Response</span></span>

<span data-ttu-id="65aee-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="65aee-128">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65aee-129">示例</span><span class="sxs-lookup"><span data-stu-id="65aee-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65aee-130">请求</span><span class="sxs-lookup"><span data-stu-id="65aee-130">Request</span></span>
<span data-ttu-id="65aee-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="65aee-131">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="65aee-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="65aee-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contacts_get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}/directReports
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="65aee-133">C#</span><span class="sxs-lookup"><span data-stu-id="65aee-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contacts-get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65aee-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65aee-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contacts-get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65aee-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65aee-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contacts-get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="65aee-136">Java</span><span class="sxs-lookup"><span data-stu-id="65aee-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contacts-get-directreports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="65aee-137">响应</span><span class="sxs-lookup"><span data-stu-id="65aee-137">Response</span></span>
<span data-ttu-id="65aee-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="65aee-138">The following is an example of the response.</span></span>
><span data-ttu-id="65aee-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="65aee-139">**Note**: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 455

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "24fcbca3-c3e2-48bf-9ffc-c7f81b81483d",
      "businessPhones": [
          "+1 205 555 0108"
      ],
      "displayName": "Diego Siciliani",
      "givenName": "Diego",
      "jobTitle": "CVP Finance",
      "mail": "DiegoS@contoso.com",
      "mobilePhone": null,
      "officeLocation": "14/1108",
      "preferredLanguage": "en-US",
      "surname": "Siciliani",
      "userPrincipalName": "DiegoS@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
