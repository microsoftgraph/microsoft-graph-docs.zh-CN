---
title: orgContact： getMemberGroups
description: 返回组织联系人所属的所有组。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 431f5e01f9e74f5c9c8d5adf9b9cc2ffa8473b04
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897181"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="e60dd-103">orgContact： getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="e60dd-103">orgContact: getMemberGroups</span></span>

<span data-ttu-id="e60dd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e60dd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e60dd-105">返回[组织联系人](../resources/orgcontact.md)所属的所有组。</span><span class="sxs-lookup"><span data-stu-id="e60dd-105">Return all the groups that the [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="e60dd-106">检查是可传递的，这和读取 **memberOf** 导航属性不同，后者仅返回用户是其直接成员的组。</span><span class="sxs-lookup"><span data-stu-id="e60dd-106">The check is transitive, unlike reading the **memberOf** navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="e60dd-107">此函数支持在 Azure Active Directory （Azure AD）中预配的 Microsoft 365 和其他类型的组。</span><span class="sxs-lookup"><span data-stu-id="e60dd-107">This function supports Microsoft 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="e60dd-108">每个请求可以返回的最大组数为 2046 组。</span><span class="sxs-lookup"><span data-stu-id="e60dd-108">The maximum number of groups each request can return is 2046.</span></span> 

>[!NOTE]
><span data-ttu-id="e60dd-109">Microsoft 365 组不能包含组。</span><span class="sxs-lookup"><span data-stu-id="e60dd-109">Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="e60dd-110">Microsoft 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="e60dd-110">Membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="e60dd-111">权限</span><span class="sxs-lookup"><span data-stu-id="e60dd-111">Permissions</span></span>
<span data-ttu-id="e60dd-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e60dd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e60dd-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="e60dd-114">Permission type</span></span>      | <span data-ttu-id="e60dd-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e60dd-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e60dd-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e60dd-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e60dd-117">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="e60dd-117">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="e60dd-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e60dd-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e60dd-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e60dd-119">Not supported.</span></span>    |
|<span data-ttu-id="e60dd-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="e60dd-120">Application</span></span> | <span data-ttu-id="e60dd-121">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="e60dd-121">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e60dd-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e60dd-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="e60dd-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e60dd-123">Request headers</span></span>
| <span data-ttu-id="e60dd-124">标头</span><span class="sxs-lookup"><span data-stu-id="e60dd-124">Header</span></span>       | <span data-ttu-id="e60dd-125">值</span><span class="sxs-lookup"><span data-stu-id="e60dd-125">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e60dd-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e60dd-126">Authorization</span></span>  |  <span data-ttu-id="e60dd-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e60dd-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e60dd-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="e60dd-129">Content-type</span></span>   | <span data-ttu-id="e60dd-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e60dd-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e60dd-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="e60dd-132">Request body</span></span>
<span data-ttu-id="e60dd-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e60dd-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e60dd-134">参数</span><span class="sxs-lookup"><span data-stu-id="e60dd-134">Parameter</span></span>    | <span data-ttu-id="e60dd-135">类型</span><span class="sxs-lookup"><span data-stu-id="e60dd-135">Type</span></span>   |<span data-ttu-id="e60dd-136">说明</span><span class="sxs-lookup"><span data-stu-id="e60dd-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e60dd-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="e60dd-137">securityEnabledOnly</span></span>|<span data-ttu-id="e60dd-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="e60dd-138">Boolean</span></span>|<span data-ttu-id="e60dd-139">设置为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="e60dd-139">Set to `false`.</span></span> <span data-ttu-id="e60dd-140">只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="e60dd-140">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="e60dd-141">响应</span><span class="sxs-lookup"><span data-stu-id="e60dd-141">Response</span></span>

<span data-ttu-id="e60dd-142">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="e60dd-142">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e60dd-143">示例</span><span class="sxs-lookup"><span data-stu-id="e60dd-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e60dd-144">请求</span><span class="sxs-lookup"><span data-stu-id="e60dd-144">Request</span></span>
<span data-ttu-id="e60dd-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e60dd-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e60dd-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="e60dd-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="c"></a>[<span data-ttu-id="e60dd-147">C#</span><span class="sxs-lookup"><span data-stu-id="e60dd-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e60dd-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e60dd-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e60dd-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e60dd-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e60dd-150">Java</span><span class="sxs-lookup"><span data-stu-id="e60dd-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e60dd-151">响应</span><span class="sxs-lookup"><span data-stu-id="e60dd-151">Response</span></span>
<span data-ttu-id="e60dd-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e60dd-152">The following is an example of the response.</span></span>
><span data-ttu-id="e60dd-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e60dd-153">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
    "groupId-value1",
    "groupId-value2"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
