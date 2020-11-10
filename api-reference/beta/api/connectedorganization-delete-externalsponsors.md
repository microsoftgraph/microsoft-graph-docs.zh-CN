---
title: 删除已连接的组织外部发起人
description: 从连接的组织的外部发起人中删除用户或组。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a5290bcd6cbb5d6ebfab002d977e96890ed9ff73
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957805"
---
# <a name="remove-connected-organization-external-sponsor"></a><span data-ttu-id="96262-103">删除已连接的组织外部发起人</span><span class="sxs-lookup"><span data-stu-id="96262-103">Remove connected organization external sponsor</span></span>

<span data-ttu-id="96262-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96262-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96262-105">从连接的组织的外部发起人中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="96262-105">Remove a user or a group from the connected organization's external sponsors.</span></span> <span data-ttu-id="96262-106">外部发起人是一组用户，他们可以代表连接的组织中的其他用户批准请求。</span><span class="sxs-lookup"><span data-stu-id="96262-106">The external sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="96262-107">权限</span><span class="sxs-lookup"><span data-stu-id="96262-107">Permissions</span></span>
<span data-ttu-id="96262-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96262-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96262-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="96262-110">Permission type</span></span>      | <span data-ttu-id="96262-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96262-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96262-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96262-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="96262-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96262-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="96262-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96262-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96262-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="96262-115">Not supported.</span></span>    |
|<span data-ttu-id="96262-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="96262-116">Application</span></span> | <span data-ttu-id="96262-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="96262-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96262-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96262-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="96262-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="96262-119">Request headers</span></span>
| <span data-ttu-id="96262-120">名称</span><span class="sxs-lookup"><span data-stu-id="96262-120">Name</span></span>       | <span data-ttu-id="96262-121">说明</span><span class="sxs-lookup"><span data-stu-id="96262-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="96262-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="96262-122">Authorization</span></span>  | <span data-ttu-id="96262-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96262-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96262-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="96262-125">Request body</span></span>
<span data-ttu-id="96262-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96262-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96262-127">响应</span><span class="sxs-lookup"><span data-stu-id="96262-127">Response</span></span>
<span data-ttu-id="96262-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="96262-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96262-130">示例</span><span class="sxs-lookup"><span data-stu-id="96262-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="96262-131">请求</span><span class="sxs-lookup"><span data-stu-id="96262-131">Request</span></span>

<span data-ttu-id="96262-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="96262-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="96262-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="96262-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalsponsor_from_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="96262-134">C#</span><span class="sxs-lookup"><span data-stu-id="96262-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalsponsor-from-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96262-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96262-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalsponsor-from-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96262-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96262-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalsponsor-from-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96262-137">Java</span><span class="sxs-lookup"><span data-stu-id="96262-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalsponsor-from-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="96262-138">响应</span><span class="sxs-lookup"><span data-stu-id="96262-138">Response</span></span>

<span data-ttu-id="96262-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="96262-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete connected organization external sponsor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


