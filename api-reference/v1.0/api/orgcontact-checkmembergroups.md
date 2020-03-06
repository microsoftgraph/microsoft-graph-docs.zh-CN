---
title: orgContact： checkMemberGroups
description: 检查指定组列表中的成员身份。 从列表中返回，其中组织联系人具有直接或可传递成员身份的组 Id。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e9ce7ba67aa979349b5a3aeae287d52bfb55a995
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511213"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="5a38f-104">orgContact： checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="5a38f-104">orgContact: checkMemberGroups</span></span>

<span data-ttu-id="5a38f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a38f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a38f-106">检查指定组列表中的成员身份。</span><span class="sxs-lookup"><span data-stu-id="5a38f-106">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="5a38f-107">从列表中返回，其中[组织联系人](../resources/orgcontact.md)具有直接或可传递成员身份的组 id。</span><span class="sxs-lookup"><span data-stu-id="5a38f-107">Returns from the list those group IDs of which the [organizational contact](../resources/orgcontact.md) has a direct or transitive membership.</span></span>

<span data-ttu-id="5a38f-108">每个请求最多可检查 20 个组。</span><span class="sxs-lookup"><span data-stu-id="5a38f-108">You can check up to a maximum of 20 groups per request.</span></span> <span data-ttu-id="5a38f-109">此函数支持在 Azure Active Directory （Azure AD）中预配的 Office 365 和其他类型的组。</span><span class="sxs-lookup"><span data-stu-id="5a38f-109">This function supports Office 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span>

>[!NOTE]
><span data-ttu-id="5a38f-110">Office 365 组不能包含组。</span><span class="sxs-lookup"><span data-stu-id="5a38f-110">Office 365 groups cannot contain groups.</span></span> <span data-ttu-id="5a38f-111">Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="5a38f-111">Membership in an Office 365 group is always direct.</span></span>


## <a name="permissions"></a><span data-ttu-id="5a38f-112">权限</span><span class="sxs-lookup"><span data-stu-id="5a38f-112">Permissions</span></span>
<span data-ttu-id="5a38f-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a38f-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a38f-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a38f-115">Permission type</span></span>      | <span data-ttu-id="5a38f-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a38f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a38f-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a38f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="5a38f-118">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="5a38f-118">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="5a38f-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a38f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a38f-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a38f-120">Not supported.</span></span>    |
|<span data-ttu-id="5a38f-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a38f-121">Application</span></span> | <span data-ttu-id="5a38f-122">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="5a38f-122">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a38f-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a38f-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="5a38f-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a38f-124">Request headers</span></span>
| <span data-ttu-id="5a38f-125">标头</span><span class="sxs-lookup"><span data-stu-id="5a38f-125">Header</span></span>       | <span data-ttu-id="5a38f-126">值</span><span class="sxs-lookup"><span data-stu-id="5a38f-126">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="5a38f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a38f-127">Authorization</span></span>  | <span data-ttu-id="5a38f-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a38f-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5a38f-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="5a38f-130">Content-type</span></span>   | <span data-ttu-id="5a38f-p107">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5a38f-p107">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a38f-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a38f-133">Request body</span></span>
<span data-ttu-id="5a38f-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5a38f-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5a38f-135">参数</span><span class="sxs-lookup"><span data-stu-id="5a38f-135">Parameter</span></span>    | <span data-ttu-id="5a38f-136">类型</span><span class="sxs-lookup"><span data-stu-id="5a38f-136">Type</span></span>   |<span data-ttu-id="5a38f-137">说明</span><span class="sxs-lookup"><span data-stu-id="5a38f-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a38f-138">groupIds</span><span class="sxs-lookup"><span data-stu-id="5a38f-138">groupIds</span></span>|<span data-ttu-id="5a38f-139">String collection</span><span class="sxs-lookup"><span data-stu-id="5a38f-139">String collection</span></span> | <span data-ttu-id="5a38f-140">要检查的组 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="5a38f-140">A list of group IDs to check.</span></span> |

## <a name="response"></a><span data-ttu-id="5a38f-141">响应</span><span class="sxs-lookup"><span data-stu-id="5a38f-141">Response</span></span>

<span data-ttu-id="5a38f-142">如果成功，此方法在响应`200 OK`正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="5a38f-142">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a38f-143">示例</span><span class="sxs-lookup"><span data-stu-id="5a38f-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5a38f-144">请求</span><span class="sxs-lookup"><span data-stu-id="5a38f-144">Request</span></span>
<span data-ttu-id="5a38f-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5a38f-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5a38f-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a38f-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5a38f-147">C#</span><span class="sxs-lookup"><span data-stu-id="5a38f-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a38f-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a38f-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a38f-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a38f-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a38f-150">Java</span><span class="sxs-lookup"><span data-stu-id="5a38f-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5a38f-151">响应</span><span class="sxs-lookup"><span data-stu-id="5a38f-151">Response</span></span>
<span data-ttu-id="5a38f-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5a38f-152">The following is an example of the response.</span></span>
><span data-ttu-id="5a38f-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5a38f-153">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
