---
title: orgContact： getMemberObjects
description: 返回此组织联系人所属的所有组。 检查是可传递的。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2d3f283eaaaed217596c8cdaa200b3bc0a1c2f06
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451685"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="90c2b-104">orgContact： getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="90c2b-104">orgContact: getMemberObjects</span></span>

<span data-ttu-id="90c2b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90c2b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90c2b-106">返回此[组织联系人](../resources/orgcontact.md)所属的所有组。</span><span class="sxs-lookup"><span data-stu-id="90c2b-106">Return all the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="90c2b-107">检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="90c2b-107">The check is transitive.</span></span> <span data-ttu-id="90c2b-108">组织联系人不能是目录角色的成员。</span><span class="sxs-lookup"><span data-stu-id="90c2b-108">Organizational contacts cannot be members of directory roles.</span></span> <span data-ttu-id="90c2b-109">将不会返回任何目录角色。</span><span class="sxs-lookup"><span data-stu-id="90c2b-109">No directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="90c2b-110">权限</span><span class="sxs-lookup"><span data-stu-id="90c2b-110">Permissions</span></span>
<span data-ttu-id="90c2b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90c2b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90c2b-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="90c2b-113">Permission type</span></span>      | <span data-ttu-id="90c2b-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90c2b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90c2b-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90c2b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="90c2b-116">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="90c2b-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="90c2b-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90c2b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90c2b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="90c2b-118">Not supported.</span></span>    |
|<span data-ttu-id="90c2b-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="90c2b-119">Application</span></span> | <span data-ttu-id="90c2b-120">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="90c2b-120">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90c2b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90c2b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="90c2b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="90c2b-122">Request headers</span></span>
| <span data-ttu-id="90c2b-123">标头</span><span class="sxs-lookup"><span data-stu-id="90c2b-123">Header</span></span>       | <span data-ttu-id="90c2b-124">值</span><span class="sxs-lookup"><span data-stu-id="90c2b-124">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="90c2b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="90c2b-125">Authorization</span></span>  | <span data-ttu-id="90c2b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90c2b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="90c2b-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="90c2b-128">Content-type</span></span>   | <span data-ttu-id="90c2b-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="90c2b-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90c2b-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="90c2b-131">Request body</span></span>
<span data-ttu-id="90c2b-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="90c2b-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="90c2b-133">参数</span><span class="sxs-lookup"><span data-stu-id="90c2b-133">Parameter</span></span>    | <span data-ttu-id="90c2b-134">类型</span><span class="sxs-lookup"><span data-stu-id="90c2b-134">Type</span></span>   |<span data-ttu-id="90c2b-135">说明</span><span class="sxs-lookup"><span data-stu-id="90c2b-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90c2b-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="90c2b-136">securityEnabledOnly</span></span>|<span data-ttu-id="90c2b-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="90c2b-137">Boolean</span></span>|<span data-ttu-id="90c2b-138">设置为`false`。</span><span class="sxs-lookup"><span data-stu-id="90c2b-138">Set to `false`.</span></span> <span data-ttu-id="90c2b-139">只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="90c2b-139">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="90c2b-140">响应</span><span class="sxs-lookup"><span data-stu-id="90c2b-140">Response</span></span>

<span data-ttu-id="90c2b-141">如果成功，此方法在响应`200 OK`正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="90c2b-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90c2b-142">示例</span><span class="sxs-lookup"><span data-stu-id="90c2b-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="90c2b-143">请求</span><span class="sxs-lookup"><span data-stu-id="90c2b-143">Request</span></span>
<span data-ttu-id="90c2b-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="90c2b-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="90c2b-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="90c2b-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="90c2b-146">C#</span><span class="sxs-lookup"><span data-stu-id="90c2b-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90c2b-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90c2b-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90c2b-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90c2b-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90c2b-149">Java</span><span class="sxs-lookup"><span data-stu-id="90c2b-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="90c2b-150">响应</span><span class="sxs-lookup"><span data-stu-id="90c2b-150">Response</span></span>
<span data-ttu-id="90c2b-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="90c2b-151">The following is an example of the response.</span></span>
><span data-ttu-id="90c2b-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="90c2b-152">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
