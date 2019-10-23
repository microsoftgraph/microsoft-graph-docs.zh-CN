---
title: orgContact： getMemberGroups
description: 返回组织联系人所属的所有组。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bfff689d075fc874c3ce31b2992cf90286af3049
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37633966"
---
# <a name="orgcontact-getmembergroups"></a><span data-ttu-id="00e72-103">orgContact： getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="00e72-103">orgContact: getMemberGroups</span></span>

<span data-ttu-id="00e72-104">返回[组织联系人](../resources/orgcontact.md)所属的所有组。</span><span class="sxs-lookup"><span data-stu-id="00e72-104">Return all the groups that the [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="00e72-105">检查是可传递的，这和读取 **memberOf** 导航属性不同，后者仅返回用户是其直接成员的组。</span><span class="sxs-lookup"><span data-stu-id="00e72-105">The check is transitive, unlike reading the **memberOf** navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="00e72-106">此函数支持在 Azure Active Directory （Azure AD）中预配的 Office 365 和其他类型的组。</span><span class="sxs-lookup"><span data-stu-id="00e72-106">This function supports Office 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="00e72-107">每个请求可以返回的最大组数为 2046 组。</span><span class="sxs-lookup"><span data-stu-id="00e72-107">The maximum number of groups each request can return is 2046.</span></span> 

>[!NOTE]
><span data-ttu-id="00e72-108">Office 365 组不能包含组。</span><span class="sxs-lookup"><span data-stu-id="00e72-108">Office 365 groups cannot contain groups.</span></span> <span data-ttu-id="00e72-109">Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="00e72-109">Membership in an Office 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="00e72-110">权限</span><span class="sxs-lookup"><span data-stu-id="00e72-110">Permissions</span></span>
<span data-ttu-id="00e72-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00e72-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00e72-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="00e72-113">Permission type</span></span>      | <span data-ttu-id="00e72-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00e72-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00e72-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00e72-115">Delegated (work or school account)</span></span> | <span data-ttu-id="00e72-116">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="00e72-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="00e72-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00e72-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00e72-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="00e72-118">Not supported.</span></span>    |
|<span data-ttu-id="00e72-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="00e72-119">Application</span></span> | <span data-ttu-id="00e72-120">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="00e72-120">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00e72-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00e72-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="00e72-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="00e72-122">Request headers</span></span>
| <span data-ttu-id="00e72-123">标头</span><span class="sxs-lookup"><span data-stu-id="00e72-123">Header</span></span>       | <span data-ttu-id="00e72-124">值</span><span class="sxs-lookup"><span data-stu-id="00e72-124">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="00e72-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="00e72-125">Authorization</span></span>  |  <span data-ttu-id="00e72-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="00e72-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="00e72-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="00e72-128">Content-type</span></span>   | <span data-ttu-id="00e72-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="00e72-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00e72-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="00e72-131">Request body</span></span>
<span data-ttu-id="00e72-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="00e72-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="00e72-133">参数</span><span class="sxs-lookup"><span data-stu-id="00e72-133">Parameter</span></span>    | <span data-ttu-id="00e72-134">类型</span><span class="sxs-lookup"><span data-stu-id="00e72-134">Type</span></span>   |<span data-ttu-id="00e72-135">说明</span><span class="sxs-lookup"><span data-stu-id="00e72-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00e72-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="00e72-136">securityEnabledOnly</span></span>|<span data-ttu-id="00e72-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="00e72-137">Boolean</span></span>|<span data-ttu-id="00e72-138">设置为`false`。</span><span class="sxs-lookup"><span data-stu-id="00e72-138">Set to `false`.</span></span> <span data-ttu-id="00e72-139">只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="00e72-139">Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="00e72-140">响应</span><span class="sxs-lookup"><span data-stu-id="00e72-140">Response</span></span>

<span data-ttu-id="00e72-141">如果成功，此方法在响应`200 OK`正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="00e72-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00e72-142">示例</span><span class="sxs-lookup"><span data-stu-id="00e72-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="00e72-143">请求</span><span class="sxs-lookup"><span data-stu-id="00e72-143">Request</span></span>
<span data-ttu-id="00e72-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="00e72-144">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="00e72-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="00e72-145">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="00e72-146">C#</span><span class="sxs-lookup"><span data-stu-id="00e72-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00e72-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00e72-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="00e72-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00e72-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="00e72-149">Java</span><span class="sxs-lookup"><span data-stu-id="00e72-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="00e72-150">响应</span><span class="sxs-lookup"><span data-stu-id="00e72-150">Response</span></span>
<span data-ttu-id="00e72-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="00e72-151">The following is an example of the response.</span></span>
><span data-ttu-id="00e72-152">**注意**：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="00e72-152">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
