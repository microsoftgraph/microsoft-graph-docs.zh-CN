---
title: orgContact： checkMemberGroups
description: 检查指定组列表中的成员身份。 从列表中返回组织联系人具有直接或可传递成员身份的组 ID。
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5bdafc5ecaf7e2f95017267bf35ff140994bfb1d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761358"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="5a1cd-104">orgContact： checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="5a1cd-104">orgContact: checkMemberGroups</span></span>

<span data-ttu-id="5a1cd-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a1cd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a1cd-106">检查指定组列表中的成员身份。</span><span class="sxs-lookup"><span data-stu-id="5a1cd-106">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="5a1cd-107">从列表中返回组织联系人具有直接或可传递成员身份的[](../resources/orgcontact.md)组 ID。</span><span class="sxs-lookup"><span data-stu-id="5a1cd-107">Returns from the list those group IDs of which the [organizational contact](../resources/orgcontact.md) has a direct or transitive membership.</span></span>

<span data-ttu-id="5a1cd-108">每个请求最多可检查 20 个组。</span><span class="sxs-lookup"><span data-stu-id="5a1cd-108">You can check up to a maximum of 20 groups per request.</span></span> <span data-ttu-id="5a1cd-109">此函数支持 Microsoft 365 和 Azure AD (Azure Active Directory 中预配) 。</span><span class="sxs-lookup"><span data-stu-id="5a1cd-109">This function supports Microsoft 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span>

>[!NOTE]
><span data-ttu-id="5a1cd-110">Microsoft 365 组不能包含组。</span><span class="sxs-lookup"><span data-stu-id="5a1cd-110">Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="5a1cd-111">Microsoft 365 组的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="5a1cd-111">Membership in a Microsoft 365 group is always direct.</span></span>


## <a name="permissions"></a><span data-ttu-id="5a1cd-112">权限</span><span class="sxs-lookup"><span data-stu-id="5a1cd-112">Permissions</span></span>
<span data-ttu-id="5a1cd-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a1cd-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a1cd-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a1cd-115">Permission type</span></span>      | <span data-ttu-id="5a1cd-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a1cd-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a1cd-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a1cd-117">Delegated (work or school account)</span></span> | <span data-ttu-id="5a1cd-118">OrgContact.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a1cd-118">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="5a1cd-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a1cd-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a1cd-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a1cd-120">Not supported.</span></span>    |
|<span data-ttu-id="5a1cd-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a1cd-121">Application</span></span> | <span data-ttu-id="5a1cd-122">OrgContact.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a1cd-122">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a1cd-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a1cd-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="5a1cd-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a1cd-124">Request headers</span></span>
| <span data-ttu-id="5a1cd-125">标头</span><span class="sxs-lookup"><span data-stu-id="5a1cd-125">Header</span></span>       | <span data-ttu-id="5a1cd-126">值</span><span class="sxs-lookup"><span data-stu-id="5a1cd-126">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="5a1cd-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a1cd-127">Authorization</span></span>  | <span data-ttu-id="5a1cd-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a1cd-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5a1cd-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="5a1cd-130">Content-type</span></span>   | <span data-ttu-id="5a1cd-p107">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5a1cd-p107">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a1cd-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a1cd-133">Request body</span></span>
<span data-ttu-id="5a1cd-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5a1cd-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5a1cd-135">参数</span><span class="sxs-lookup"><span data-stu-id="5a1cd-135">Parameter</span></span>    | <span data-ttu-id="5a1cd-136">类型</span><span class="sxs-lookup"><span data-stu-id="5a1cd-136">Type</span></span>   |<span data-ttu-id="5a1cd-137">说明</span><span class="sxs-lookup"><span data-stu-id="5a1cd-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a1cd-138">groupIds</span><span class="sxs-lookup"><span data-stu-id="5a1cd-138">groupIds</span></span>|<span data-ttu-id="5a1cd-139">String collection</span><span class="sxs-lookup"><span data-stu-id="5a1cd-139">String collection</span></span> | <span data-ttu-id="5a1cd-140">要检查的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="5a1cd-140">A list of group IDs to check.</span></span> |

## <a name="response"></a><span data-ttu-id="5a1cd-141">响应</span><span class="sxs-lookup"><span data-stu-id="5a1cd-141">Response</span></span>

<span data-ttu-id="5a1cd-142">如果成功，该运营商将返回 `200 OK` 响应代码和响应正文中的字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="5a1cd-142">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a1cd-143">示例</span><span class="sxs-lookup"><span data-stu-id="5a1cd-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5a1cd-144">请求</span><span class="sxs-lookup"><span data-stu-id="5a1cd-144">Request</span></span>
<span data-ttu-id="5a1cd-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5a1cd-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5a1cd-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a1cd-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupId-value1", "groupId-value2" 
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="5a1cd-147">C#</span><span class="sxs-lookup"><span data-stu-id="5a1cd-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a1cd-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a1cd-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a1cd-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a1cd-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a1cd-150">Java</span><span class="sxs-lookup"><span data-stu-id="5a1cd-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5a1cd-151">响应</span><span class="sxs-lookup"><span data-stu-id="5a1cd-151">Response</span></span>
<span data-ttu-id="5a1cd-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5a1cd-152">The following is an example of the response.</span></span>
><span data-ttu-id="5a1cd-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5a1cd-153">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
    "groupId-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

