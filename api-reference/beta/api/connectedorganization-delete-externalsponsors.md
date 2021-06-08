---
title: 删除连接的组织外部发起人
description: 从已连接的组织的外部发起人中删除用户或组。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 936c91f5ebd3bff0af8ec25a4ce542707e04227d
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786508"
---
# <a name="remove-connected-organization-external-sponsor"></a><span data-ttu-id="9dd70-103">删除连接的组织外部发起人</span><span class="sxs-lookup"><span data-stu-id="9dd70-103">Remove connected organization external sponsor</span></span>

<span data-ttu-id="9dd70-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9dd70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dd70-105">从已连接的组织的外部发起人中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="9dd70-105">Remove a user or a group from the connected organization's external sponsors.</span></span> <span data-ttu-id="9dd70-106">外部发起人是一组用户，可以代表该连接的组织的其他用户批准请求。</span><span class="sxs-lookup"><span data-stu-id="9dd70-106">The external sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="9dd70-107">权限</span><span class="sxs-lookup"><span data-stu-id="9dd70-107">Permissions</span></span>
<span data-ttu-id="9dd70-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9dd70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dd70-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9dd70-110">Permission type</span></span>      | <span data-ttu-id="9dd70-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9dd70-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9dd70-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9dd70-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9dd70-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dd70-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="9dd70-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9dd70-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dd70-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9dd70-115">Not supported.</span></span>    |
|<span data-ttu-id="9dd70-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9dd70-116">Application</span></span> | <span data-ttu-id="9dd70-117">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dd70-117">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9dd70-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9dd70-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9dd70-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9dd70-119">Request headers</span></span>
| <span data-ttu-id="9dd70-120">名称</span><span class="sxs-lookup"><span data-stu-id="9dd70-120">Name</span></span>       | <span data-ttu-id="9dd70-121">说明</span><span class="sxs-lookup"><span data-stu-id="9dd70-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9dd70-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9dd70-122">Authorization</span></span>  | <span data-ttu-id="9dd70-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9dd70-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9dd70-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9dd70-125">Request body</span></span>
<span data-ttu-id="9dd70-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9dd70-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9dd70-127">响应</span><span class="sxs-lookup"><span data-stu-id="9dd70-127">Response</span></span>
<span data-ttu-id="9dd70-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9dd70-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dd70-130">示例</span><span class="sxs-lookup"><span data-stu-id="9dd70-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9dd70-131">请求</span><span class="sxs-lookup"><span data-stu-id="9dd70-131">Request</span></span>

<span data-ttu-id="9dd70-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9dd70-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9dd70-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9dd70-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalsponsor_from_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="9dd70-134">C#</span><span class="sxs-lookup"><span data-stu-id="9dd70-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalsponsor-from-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9dd70-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9dd70-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalsponsor-from-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9dd70-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9dd70-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalsponsor-from-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9dd70-137">Java</span><span class="sxs-lookup"><span data-stu-id="9dd70-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalsponsor-from-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9dd70-138">响应</span><span class="sxs-lookup"><span data-stu-id="9dd70-138">Response</span></span>

<span data-ttu-id="9dd70-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9dd70-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
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


