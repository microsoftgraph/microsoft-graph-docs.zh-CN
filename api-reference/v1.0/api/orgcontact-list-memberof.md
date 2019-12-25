---
title: 列出 memberOf
description: 列出此 organizaitonal 联系人所属的组。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8a9727f19f8c108203f4341fb864d4776cf24101
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865543"
---
# <a name="list-memberof"></a><span data-ttu-id="26d78-103">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="26d78-103">List memberOf</span></span>

<span data-ttu-id="26d78-104">列出此[组织联系人](../resources/orgcontact.md)所属的组。</span><span class="sxs-lookup"><span data-stu-id="26d78-104">List the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="26d78-105">权限</span><span class="sxs-lookup"><span data-stu-id="26d78-105">Permissions</span></span>
<span data-ttu-id="26d78-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="26d78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26d78-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="26d78-108">Permission type</span></span>      | <span data-ttu-id="26d78-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="26d78-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26d78-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="26d78-110">Delegated (work or school account)</span></span> | <span data-ttu-id="26d78-111">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="26d78-111">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="26d78-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="26d78-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26d78-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="26d78-113">Not supported.</span></span>    |
|<span data-ttu-id="26d78-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="26d78-114">Application</span></span> | <span data-ttu-id="26d78-115">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="26d78-115">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="26d78-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="26d78-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="26d78-117">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="26d78-117">Optional query parameters</span></span>
<span data-ttu-id="26d78-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `$select` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="26d78-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `$select` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26d78-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="26d78-119">Request headers</span></span>
| <span data-ttu-id="26d78-120">标头</span><span class="sxs-lookup"><span data-stu-id="26d78-120">Header</span></span>       | <span data-ttu-id="26d78-121">值</span><span class="sxs-lookup"><span data-stu-id="26d78-121">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="26d78-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="26d78-122">Authorization</span></span>  | <span data-ttu-id="26d78-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="26d78-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26d78-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="26d78-125">Request body</span></span>
<span data-ttu-id="26d78-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="26d78-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26d78-127">响应</span><span class="sxs-lookup"><span data-stu-id="26d78-127">Response</span></span>

<span data-ttu-id="26d78-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="26d78-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="26d78-129">示例</span><span class="sxs-lookup"><span data-stu-id="26d78-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26d78-130">请求</span><span class="sxs-lookup"><span data-stu-id="26d78-130">Request</span></span>
<span data-ttu-id="26d78-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="26d78-131">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="26d78-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="26d78-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contact_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="26d78-133">C#</span><span class="sxs-lookup"><span data-stu-id="26d78-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contact-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26d78-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26d78-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contact-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="26d78-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="26d78-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contact-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="26d78-136">Java</span><span class="sxs-lookup"><span data-stu-id="26d78-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contact-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="26d78-137">响应</span><span class="sxs-lookup"><span data-stu-id="26d78-137">Response</span></span>
<span data-ttu-id="26d78-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="26d78-138">The following is an example of the response.</span></span>
><span data-ttu-id="26d78-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="26d78-139">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="26d78-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="26d78-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 155

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "024bbfa0-fe5a-4fce-9227-bd6ccf1324bb",
      "createdDateTime": "2018-01-18T18:54:43Z",
      "description": "Best group ever created",
      "displayName": "Best Group",
      "groupTypes": [],
      "isAssignableToRole": null,
      "onPremisesProvisioningErrors": []
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
