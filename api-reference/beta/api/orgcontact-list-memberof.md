---
title: orgContact：列表 memberOf
description: 检索联系人所属的组和管理单位的列表。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0cae37a8e8de2de5c87eaa9638b5c8e0757e2b68
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979789"
---
# <a name="orgcontact-list-memberof"></a><span data-ttu-id="940be-103">orgContact：列表 memberOf</span><span class="sxs-lookup"><span data-stu-id="940be-103">orgContact: List memberOf</span></span>

<span data-ttu-id="940be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="940be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="940be-105">检索联系人所属的组和管理单位的列表。</span><span class="sxs-lookup"><span data-stu-id="940be-105">Retrieve the list of groups and adminstrative units the contact is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="940be-106">权限</span><span class="sxs-lookup"><span data-stu-id="940be-106">Permissions</span></span>
<span data-ttu-id="940be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="940be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="940be-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="940be-109">Permission type</span></span>      | <span data-ttu-id="940be-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="940be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="940be-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="940be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="940be-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="940be-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="940be-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="940be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="940be-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="940be-114">Not supported.</span></span>    |
|<span data-ttu-id="940be-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="940be-115">Application</span></span> | <span data-ttu-id="940be-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="940be-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="940be-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="940be-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="940be-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="940be-118">Optional query parameters</span></span>
<span data-ttu-id="940be-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="940be-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="940be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="940be-120">Request headers</span></span>
| <span data-ttu-id="940be-121">名称</span><span class="sxs-lookup"><span data-stu-id="940be-121">Name</span></span>       | <span data-ttu-id="940be-122">类型</span><span class="sxs-lookup"><span data-stu-id="940be-122">Type</span></span> | <span data-ttu-id="940be-123">说明</span><span class="sxs-lookup"><span data-stu-id="940be-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="940be-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="940be-124">Authorization</span></span>  | <span data-ttu-id="940be-125">string</span><span class="sxs-lookup"><span data-stu-id="940be-125">string</span></span>  | <span data-ttu-id="940be-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="940be-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="940be-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="940be-128">Request body</span></span>
<span data-ttu-id="940be-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="940be-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="940be-130">响应</span><span class="sxs-lookup"><span data-stu-id="940be-130">Response</span></span>

<span data-ttu-id="940be-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="940be-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="940be-132">示例</span><span class="sxs-lookup"><span data-stu-id="940be-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="940be-133">请求</span><span class="sxs-lookup"><span data-stu-id="940be-133">Request</span></span>
<span data-ttu-id="940be-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="940be-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="940be-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="940be-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contact_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="940be-136">C#</span><span class="sxs-lookup"><span data-stu-id="940be-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contact-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="940be-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="940be-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contact-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="940be-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="940be-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contact-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="940be-139">响应</span><span class="sxs-lookup"><span data-stu-id="940be-139">Response</span></span>
<span data-ttu-id="940be-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="940be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
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


