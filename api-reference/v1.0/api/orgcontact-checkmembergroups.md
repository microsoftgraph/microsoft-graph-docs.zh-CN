---
title: orgContact： checkMemberGroups
description: 检查指定组列表中的成员身份。 从列表中返回，其中组织联系人具有直接或可传递成员身份的组 Id。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 40dbe27c9d3bbf90cb4ada184d088159883065be
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37622588"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="e8619-104">orgContact： checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="e8619-104">orgContact: checkMemberGroups</span></span>

<span data-ttu-id="e8619-105">检查指定组列表中的成员身份。</span><span class="sxs-lookup"><span data-stu-id="e8619-105">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="e8619-106">从列表中返回，其中[组织联系人](../resources/orgcontact.md)具有直接或可传递成员身份的组 id。</span><span class="sxs-lookup"><span data-stu-id="e8619-106">Returns from the list those group IDs of which the [organizational contact](../resources/orgcontact.md) has a direct or transitive membership.</span></span>

<span data-ttu-id="e8619-107">每个请求最多可检查 20 个组。</span><span class="sxs-lookup"><span data-stu-id="e8619-107">You can check up to a maximum of 20 groups per request.</span></span> <span data-ttu-id="e8619-108">此函数支持在 Azure Active Directory （Azure AD）中预配的 Office 365 和其他类型的组。</span><span class="sxs-lookup"><span data-stu-id="e8619-108">This function supports Office 365 and other types of groups provisioned in Azure Active Directory (Azure AD).</span></span>

>[!NOTE]
><span data-ttu-id="e8619-109">Office 365 组不能包含组。</span><span class="sxs-lookup"><span data-stu-id="e8619-109">Office 365 groups cannot contain groups.</span></span> <span data-ttu-id="e8619-110">Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="e8619-110">Membership in an Office 365 group is always direct.</span></span>


## <a name="permissions"></a><span data-ttu-id="e8619-111">权限</span><span class="sxs-lookup"><span data-stu-id="e8619-111">Permissions</span></span>
<span data-ttu-id="e8619-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8619-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8619-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8619-114">Permission type</span></span>      | <span data-ttu-id="e8619-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8619-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8619-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8619-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e8619-117">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="e8619-117">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="e8619-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8619-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8619-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8619-119">Not supported.</span></span>    |
|<span data-ttu-id="e8619-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8619-120">Application</span></span> | <span data-ttu-id="e8619-121">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="e8619-121">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8619-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8619-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="e8619-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8619-123">Request headers</span></span>
| <span data-ttu-id="e8619-124">标头</span><span class="sxs-lookup"><span data-stu-id="e8619-124">Header</span></span>       | <span data-ttu-id="e8619-125">值</span><span class="sxs-lookup"><span data-stu-id="e8619-125">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e8619-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8619-126">Authorization</span></span>  | <span data-ttu-id="e8619-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8619-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e8619-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="e8619-129">Content-type</span></span>   | <span data-ttu-id="e8619-p107">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e8619-p107">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8619-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8619-132">Request body</span></span>
<span data-ttu-id="e8619-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e8619-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e8619-134">参数</span><span class="sxs-lookup"><span data-stu-id="e8619-134">Parameter</span></span>    | <span data-ttu-id="e8619-135">类型</span><span class="sxs-lookup"><span data-stu-id="e8619-135">Type</span></span>   |<span data-ttu-id="e8619-136">说明</span><span class="sxs-lookup"><span data-stu-id="e8619-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8619-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="e8619-137">groupIds</span></span>|<span data-ttu-id="e8619-138">String collection</span><span class="sxs-lookup"><span data-stu-id="e8619-138">String collection</span></span> | <span data-ttu-id="e8619-139">要检查的组 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="e8619-139">A list of group IDs to check.</span></span> |

## <a name="response"></a><span data-ttu-id="e8619-140">响应</span><span class="sxs-lookup"><span data-stu-id="e8619-140">Response</span></span>

<span data-ttu-id="e8619-141">如果成功，此方法在响应`200 OK`正文中返回响应代码和字符串集合对象。</span><span class="sxs-lookup"><span data-stu-id="e8619-141">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8619-142">示例</span><span class="sxs-lookup"><span data-stu-id="e8619-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e8619-143">请求</span><span class="sxs-lookup"><span data-stu-id="e8619-143">Request</span></span>
<span data-ttu-id="e8619-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e8619-144">The following is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="e8619-145">响应</span><span class="sxs-lookup"><span data-stu-id="e8619-145">Response</span></span>
<span data-ttu-id="e8619-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e8619-146">The following is an example of the response.</span></span>
><span data-ttu-id="e8619-147">**注意**：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e8619-147">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
