---
title: orgContact： getMemberObjects
description: 返回此组织联系人所属的所有组。 检查是可传递的。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bbc577fe998d64a182051815124d364e9d3a7872
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37633927"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="556ca-104">orgContact： getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="556ca-104">orgContact: getMemberObjects</span></span>

<span data-ttu-id="556ca-105">返回此[组织联系人](../resources/orgcontact.md)所属的所有组。</span><span class="sxs-lookup"><span data-stu-id="556ca-105">Return all the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="556ca-106">检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="556ca-106">The check is transitive.</span></span> <span data-ttu-id="556ca-107">组织联系人不能是目录角色的成员。</span><span class="sxs-lookup"><span data-stu-id="556ca-107">Organizational contacts cannot be members of directory roles.</span></span> <span data-ttu-id="556ca-108">将不会返回任何目录角色。</span><span class="sxs-lookup"><span data-stu-id="556ca-108">No directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="556ca-109">权限</span><span class="sxs-lookup"><span data-stu-id="556ca-109">Permissions</span></span>
<span data-ttu-id="556ca-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="556ca-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="556ca-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="556ca-112">Permission type</span></span>      | <span data-ttu-id="556ca-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="556ca-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="556ca-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="556ca-114">Delegated (work or school account)</span></span> | <span data-ttu-id="556ca-115">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="556ca-115">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="556ca-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="556ca-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="556ca-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="556ca-117">Not supported.</span></span>    |
|<span data-ttu-id="556ca-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="556ca-118">Application</span></span> | <span data-ttu-id="556ca-119">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="556ca-119">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="556ca-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="556ca-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="556ca-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="556ca-121">Request headers</span></span>
| <span data-ttu-id="556ca-122">标头</span><span class="sxs-lookup"><span data-stu-id="556ca-122">Header</span></span>       | <span data-ttu-id="556ca-123">值</span><span class="sxs-lookup"><span data-stu-id="556ca-123">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="556ca-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="556ca-124">Authorization</span></span>  | <span data-ttu-id="556ca-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="556ca-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="556ca-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="556ca-127">Content-type</span></span>   | <span data-ttu-id="556ca-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="556ca-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="556ca-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="556ca-130">Request body</span></span>
<span data-ttu-id="556ca-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="556ca-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="556ca-132">参数</span><span class="sxs-lookup"><span data-stu-id="556ca-132">Parameter</span></span>    | <span data-ttu-id="556ca-133">类型</span><span class="sxs-lookup"><span data-stu-id="556ca-133">Type</span></span>   |<span data-ttu-id="556ca-134">说明</span><span class="sxs-lookup"><span data-stu-id="556ca-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="556ca-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="556ca-135">securityEnabledOnly</span></span>|<span data-ttu-id="556ca-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="556ca-136">Boolean</span></span>|<span data-ttu-id="556ca-137">设置为`false`。</span><span class="sxs-lookup"><span data-stu-id="556ca-137">Set to `false`.</span></span> <span data-ttu-id="556ca-138">只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="556ca-138">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="556ca-139">响应</span><span class="sxs-lookup"><span data-stu-id="556ca-139">Response</span></span>

<span data-ttu-id="556ca-140">如果成功，此方法在响应`200 OK`正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="556ca-140">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="556ca-141">示例</span><span class="sxs-lookup"><span data-stu-id="556ca-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="556ca-142">请求</span><span class="sxs-lookup"><span data-stu-id="556ca-142">Request</span></span>
<span data-ttu-id="556ca-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="556ca-143">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="556ca-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="556ca-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="556ca-145">C#</span><span class="sxs-lookup"><span data-stu-id="556ca-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="556ca-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="556ca-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="556ca-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="556ca-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="556ca-148">Java</span><span class="sxs-lookup"><span data-stu-id="556ca-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="556ca-149">响应</span><span class="sxs-lookup"><span data-stu-id="556ca-149">Response</span></span>
<span data-ttu-id="556ca-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="556ca-150">The following is an example of the response.</span></span>
><span data-ttu-id="556ca-151">**注意**：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="556ca-151">**Note**: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "groupID-value1"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
