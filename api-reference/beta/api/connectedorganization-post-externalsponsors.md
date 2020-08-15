---
title: 添加已连接的组织外部发起人
description: 将用户或组添加到连接的组织的外部发起人。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2a4e21f2f8d3adcbea6b8888e257fe32ac2892fa
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757415"
---
# <a name="add-connected-organization-external-sponsor"></a><span data-ttu-id="b943f-103">添加已连接的组织外部发起人</span><span class="sxs-lookup"><span data-stu-id="b943f-103">Add connected organization external sponsor</span></span>

<span data-ttu-id="b943f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b943f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b943f-105">将用户或组添加到连接的组织的外部发起人。</span><span class="sxs-lookup"><span data-stu-id="b943f-105">Add a user or a group to the connected organization's external sponsors.</span></span> <span data-ttu-id="b943f-106">外部发起人是一组用户，他们可以代表连接的组织中的其他用户批准请求。</span><span class="sxs-lookup"><span data-stu-id="b943f-106">The external sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="b943f-107">权限</span><span class="sxs-lookup"><span data-stu-id="b943f-107">Permissions</span></span>
<span data-ttu-id="b943f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b943f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b943f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b943f-110">Permission type</span></span>      | <span data-ttu-id="b943f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b943f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b943f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b943f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b943f-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b943f-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="b943f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b943f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b943f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b943f-115">Not supported.</span></span>    |
|<span data-ttu-id="b943f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b943f-116">Application</span></span> | <span data-ttu-id="b943f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b943f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b943f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b943f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b943f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b943f-119">Request headers</span></span>
| <span data-ttu-id="b943f-120">名称</span><span class="sxs-lookup"><span data-stu-id="b943f-120">Name</span></span>       | <span data-ttu-id="b943f-121">说明</span><span class="sxs-lookup"><span data-stu-id="b943f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b943f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b943f-122">Authorization</span></span>  | <span data-ttu-id="b943f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b943f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b943f-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="b943f-125">Content-type</span></span> | <span data-ttu-id="b943f-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b943f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b943f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b943f-128">Request body</span></span>
<span data-ttu-id="b943f-129">在请求正文中，提供要添加的 [用户](../resources/user.md) 或 [组](../resources/group.md) 对象的引用的 JSON 表示形式，作为 `@odata.id` 具有用户或组的完整 URI 的属性。</span><span class="sxs-lookup"><span data-stu-id="b943f-129">In the request body, supply a JSON representation of the reference to the [user](../resources/user.md) or [group](../resources/group.md) object to be added, as an `@odata.id` property with the full URI of the user or group.</span></span>

## <a name="response"></a><span data-ttu-id="b943f-130">响应</span><span class="sxs-lookup"><span data-stu-id="b943f-130">Response</span></span>
<span data-ttu-id="b943f-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b943f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b943f-133">示例</span><span class="sxs-lookup"><span data-stu-id="b943f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b943f-134">请求</span><span class="sxs-lookup"><span data-stu-id="b943f-134">Request</span></span>

<span data-ttu-id="b943f-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b943f-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_externalsponsor_from_connectedorganization"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```

### <a name="response"></a><span data-ttu-id="b943f-136">响应</span><span class="sxs-lookup"><span data-stu-id="b943f-136">Response</span></span>

<span data-ttu-id="b943f-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b943f-137">The following is an example of the response.</span></span>

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
  "description": "Create connected organization external sponsor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
