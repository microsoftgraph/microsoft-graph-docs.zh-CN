---
title: 删除已连接的组织内部赞助商
description: 从连接的组织的内部发起人中删除用户或组。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0085f4641ab03b0b4f93e13e116ff34be514397f
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757423"
---
# <a name="remove-connected-organization-internal-sponsor"></a><span data-ttu-id="1986d-103">删除已连接的组织内部赞助商</span><span class="sxs-lookup"><span data-stu-id="1986d-103">Remove connected organization internal sponsor</span></span>

<span data-ttu-id="1986d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1986d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1986d-105">从连接的组织的内部发起人中删除用户或组。</span><span class="sxs-lookup"><span data-stu-id="1986d-105">Remove a user or a group from the connected organization's internal sponsors.</span></span> <span data-ttu-id="1986d-106">内部赞助商是一组用户，可以代表来自该连接组织的其他用户批准请求。</span><span class="sxs-lookup"><span data-stu-id="1986d-106">The internal sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="1986d-107">权限</span><span class="sxs-lookup"><span data-stu-id="1986d-107">Permissions</span></span>
<span data-ttu-id="1986d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1986d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1986d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1986d-110">Permission type</span></span>      | <span data-ttu-id="1986d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1986d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1986d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1986d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1986d-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1986d-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="1986d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1986d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1986d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1986d-115">Not supported.</span></span>    |
|<span data-ttu-id="1986d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1986d-116">Application</span></span> | <span data-ttu-id="1986d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1986d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1986d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1986d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/internalSponsors/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="1986d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1986d-119">Request headers</span></span>
| <span data-ttu-id="1986d-120">名称</span><span class="sxs-lookup"><span data-stu-id="1986d-120">Name</span></span>       | <span data-ttu-id="1986d-121">说明</span><span class="sxs-lookup"><span data-stu-id="1986d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1986d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1986d-122">Authorization</span></span>  | <span data-ttu-id="1986d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1986d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1986d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1986d-125">Request body</span></span>
<span data-ttu-id="1986d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1986d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1986d-127">响应</span><span class="sxs-lookup"><span data-stu-id="1986d-127">Response</span></span>
<span data-ttu-id="1986d-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1986d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1986d-130">示例</span><span class="sxs-lookup"><span data-stu-id="1986d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1986d-131">请求</span><span class="sxs-lookup"><span data-stu-id="1986d-131">Request</span></span>

<span data-ttu-id="1986d-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1986d-132">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "delete_internalsponsor_from_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/internalSponsors/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="1986d-133">响应</span><span class="sxs-lookup"><span data-stu-id="1986d-133">Response</span></span>

<span data-ttu-id="1986d-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1986d-134">The following is an example of the response.</span></span>

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
  "description": "Delete connected organization internal sponsor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
