---
title: 列出 externalSponsors
description: 检索 connectedOrganization 的 externalSponsors 列表。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 82fffe33aced00b142bee52777bf154a38fb52a2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957721"
---
# <a name="list-externalsponsors"></a><span data-ttu-id="64128-103">列出 externalSponsors</span><span class="sxs-lookup"><span data-stu-id="64128-103">List externalSponsors</span></span>

<span data-ttu-id="64128-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64128-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64128-105">检索 [connectedOrganization](../resources/connectedorganization.md)的外部发起人列表。</span><span class="sxs-lookup"><span data-stu-id="64128-105">Retrieve a list of a [connectedOrganization](../resources/connectedorganization.md)'s external sponsors.</span></span>  <span data-ttu-id="64128-106">外部发起人是一组用户，他们可以代表连接的组织中的其他用户批准请求。</span><span class="sxs-lookup"><span data-stu-id="64128-106">The external sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="64128-107">权限</span><span class="sxs-lookup"><span data-stu-id="64128-107">Permissions</span></span>

<span data-ttu-id="64128-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64128-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64128-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="64128-110">Permission type</span></span>|<span data-ttu-id="64128-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="64128-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="64128-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64128-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="64128-113">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="64128-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="64128-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64128-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64128-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="64128-115">Not supported.</span></span> |
| <span data-ttu-id="64128-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="64128-116">Application</span></span>                            | <span data-ttu-id="64128-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="64128-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64128-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64128-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors
```

## <a name="request-headers"></a><span data-ttu-id="64128-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="64128-119">Request headers</span></span>
|<span data-ttu-id="64128-120">名称</span><span class="sxs-lookup"><span data-stu-id="64128-120">Name</span></span>|<span data-ttu-id="64128-121">说明</span><span class="sxs-lookup"><span data-stu-id="64128-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="64128-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="64128-122">Authorization</span></span>|<span data-ttu-id="64128-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="64128-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64128-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="64128-125">Request body</span></span>
<span data-ttu-id="64128-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="64128-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64128-127">响应</span><span class="sxs-lookup"><span data-stu-id="64128-127">Response</span></span>

<span data-ttu-id="64128-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="64128-128">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64128-129">示例</span><span class="sxs-lookup"><span data-stu-id="64128-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64128-130">请求</span><span class="sxs-lookup"><span data-stu-id="64128-130">Request</span></span>

<span data-ttu-id="64128-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="64128-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="64128-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="64128-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connectedorganization_get_externalSponsors"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors
```
# <a name="c"></a>[<span data-ttu-id="64128-133">C#</span><span class="sxs-lookup"><span data-stu-id="64128-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connectedorganization-get-externalsponsors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64128-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64128-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connectedorganization-get-externalsponsors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64128-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64128-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connectedorganization-get-externalsponsors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64128-136">Java</span><span class="sxs-lookup"><span data-stu-id="64128-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/connectedorganization-get-externalsponsors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="64128-137">响应</span><span class="sxs-lookup"><span data-stu-id="64128-137">Response</span></span>

<span data-ttu-id="64128-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="64128-138">The following is an example of the response.</span></span>

<span data-ttu-id="64128-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="64128-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "cd3709c6-be6a-4725-bd07-50f90ccca93f"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List externalSponsors",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


