---
title: orgContact： getMemberObjects
description: 返回此组织联系人所属的所有组。 检查是可传递的。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7fd09f86c53252cb0fd7cbcc69b9ac4d3db3d47a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988653"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="4def2-104">orgContact： getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="4def2-104">orgContact: getMemberObjects</span></span>

<span data-ttu-id="4def2-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4def2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4def2-106">返回此 [组织联系人](../resources/orgcontact.md) 所属的所有组。</span><span class="sxs-lookup"><span data-stu-id="4def2-106">Return all the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="4def2-107">检查是可传递的。</span><span class="sxs-lookup"><span data-stu-id="4def2-107">The check is transitive.</span></span> <span data-ttu-id="4def2-108">组织联系人不能是目录角色的成员。</span><span class="sxs-lookup"><span data-stu-id="4def2-108">Organizational contacts cannot be members of directory roles.</span></span> <span data-ttu-id="4def2-109">将不会返回任何目录角色。</span><span class="sxs-lookup"><span data-stu-id="4def2-109">No directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="4def2-110">权限</span><span class="sxs-lookup"><span data-stu-id="4def2-110">Permissions</span></span>
<span data-ttu-id="4def2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4def2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4def2-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="4def2-113">Permission type</span></span>      | <span data-ttu-id="4def2-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4def2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4def2-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4def2-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4def2-116">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="4def2-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="4def2-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4def2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4def2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4def2-118">Not supported.</span></span>    |
|<span data-ttu-id="4def2-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="4def2-119">Application</span></span> | <span data-ttu-id="4def2-120">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="4def2-120">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4def2-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4def2-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="4def2-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="4def2-122">Request headers</span></span>
| <span data-ttu-id="4def2-123">标头</span><span class="sxs-lookup"><span data-stu-id="4def2-123">Header</span></span>       | <span data-ttu-id="4def2-124">值</span><span class="sxs-lookup"><span data-stu-id="4def2-124">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4def2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4def2-125">Authorization</span></span>  | <span data-ttu-id="4def2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4def2-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4def2-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="4def2-128">Content-type</span></span>   | <span data-ttu-id="4def2-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4def2-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4def2-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="4def2-131">Request body</span></span>
<span data-ttu-id="4def2-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4def2-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4def2-133">参数</span><span class="sxs-lookup"><span data-stu-id="4def2-133">Parameter</span></span>    | <span data-ttu-id="4def2-134">类型</span><span class="sxs-lookup"><span data-stu-id="4def2-134">Type</span></span>   |<span data-ttu-id="4def2-135">说明</span><span class="sxs-lookup"><span data-stu-id="4def2-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4def2-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="4def2-136">securityEnabledOnly</span></span>|<span data-ttu-id="4def2-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="4def2-137">Boolean</span></span>|<span data-ttu-id="4def2-138">设置为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="4def2-138">Set to `false`.</span></span> <span data-ttu-id="4def2-139">只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="4def2-139">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="4def2-140">响应</span><span class="sxs-lookup"><span data-stu-id="4def2-140">Response</span></span>

<span data-ttu-id="4def2-141">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="4def2-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4def2-142">示例</span><span class="sxs-lookup"><span data-stu-id="4def2-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4def2-143">请求</span><span class="sxs-lookup"><span data-stu-id="4def2-143">Request</span></span>
<span data-ttu-id="4def2-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4def2-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4def2-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4def2-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4def2-146">C#</span><span class="sxs-lookup"><span data-stu-id="4def2-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4def2-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4def2-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4def2-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4def2-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4def2-149">Java</span><span class="sxs-lookup"><span data-stu-id="4def2-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4def2-150">响应</span><span class="sxs-lookup"><span data-stu-id="4def2-150">Response</span></span>
<span data-ttu-id="4def2-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4def2-151">The following is an example of the response.</span></span>
><span data-ttu-id="4def2-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4def2-152">**Note**: The response object shown here might be shortened for readability.</span></span> 
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

