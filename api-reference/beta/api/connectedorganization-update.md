---
title: 更新 connectedOrganization 对象
description: 更新 connectedOrganization 对象。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 804beb5db6fe42d430912fc14377764b9f4d6dcb
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566503"
---
# <a name="update-connectedorganization"></a><span data-ttu-id="475fe-103">更新 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="475fe-103">Update connectedOrganization</span></span>

<span data-ttu-id="475fe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="475fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="475fe-105">更新[connectedOrganization](../resources/connectedorganization.md)对象以更改其一个或多个属性。</span><span class="sxs-lookup"><span data-stu-id="475fe-105">Update a [connectedOrganization](../resources/connectedorganization.md) object to change one or more of its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="475fe-106">权限</span><span class="sxs-lookup"><span data-stu-id="475fe-106">Permissions</span></span>
<span data-ttu-id="475fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="475fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="475fe-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="475fe-109">Permission type</span></span>|<span data-ttu-id="475fe-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="475fe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="475fe-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="475fe-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="475fe-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="475fe-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="475fe-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="475fe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="475fe-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="475fe-114">Not supported.</span></span> |
|<span data-ttu-id="475fe-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="475fe-115">Application</span></span>                            | <span data-ttu-id="475fe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="475fe-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="475fe-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="475fe-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="475fe-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="475fe-118">Request headers</span></span>
|<span data-ttu-id="475fe-119">名称</span><span class="sxs-lookup"><span data-stu-id="475fe-119">Name</span></span>|<span data-ttu-id="475fe-120">说明</span><span class="sxs-lookup"><span data-stu-id="475fe-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="475fe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="475fe-121">Authorization</span></span>|<span data-ttu-id="475fe-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="475fe-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="475fe-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="475fe-124">Content-Type</span></span>|<span data-ttu-id="475fe-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="475fe-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="475fe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="475fe-127">Request body</span></span>
<span data-ttu-id="475fe-128">在请求正文中，提供[connectedOrganization](../resources/connectedorganization.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="475fe-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="475fe-129">下表显示了在更新[connectedOrganization](../resources/connectedorganization.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="475fe-129">The following table shows the properties that are required when you update the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="475fe-130">属性</span><span class="sxs-lookup"><span data-stu-id="475fe-130">Property</span></span>|<span data-ttu-id="475fe-131">类型</span><span class="sxs-lookup"><span data-stu-id="475fe-131">Type</span></span>|<span data-ttu-id="475fe-132">说明</span><span class="sxs-lookup"><span data-stu-id="475fe-132">Description</span></span>|
|:---|:---|:---|
| `displayName`  |`String` | <span data-ttu-id="475fe-133">连接的组织名称。</span><span class="sxs-lookup"><span data-stu-id="475fe-133">The connected organization name.</span></span>  |
| `description`  |`String` | <span data-ttu-id="475fe-134">连接的组织说明。</span><span class="sxs-lookup"><span data-stu-id="475fe-134">The connected organization description.</span></span> |

## <a name="response"></a><span data-ttu-id="475fe-135">响应</span><span class="sxs-lookup"><span data-stu-id="475fe-135">Response</span></span>

<span data-ttu-id="475fe-136">如果成功，此方法 `204 Accepted` 在响应正文中返回响应代码和[connectedOrganization](../resources/connectedorganization.md)对象。</span><span class="sxs-lookup"><span data-stu-id="475fe-136">If successful, this method returns a `204 Accepted` response code and a [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="475fe-137">示例</span><span class="sxs-lookup"><span data-stu-id="475fe-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="475fe-138">请求</span><span class="sxs-lookup"><span data-stu-id="475fe-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="475fe-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="475fe-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connectedorganization"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
Content-Type: application/json
Content-length: 100

{
  "displayName":"Connected organization new name",
  "description":"Connected organization new description"
}
```
# <a name="c"></a>[<span data-ttu-id="475fe-140">C#</span><span class="sxs-lookup"><span data-stu-id="475fe-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="475fe-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="475fe-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="475fe-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="475fe-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="475fe-143">响应</span><span class="sxs-lookup"><span data-stu-id="475fe-143">Response</span></span>
<span data-ttu-id="475fe-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="475fe-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectedOrganization"
}
-->
``` http
HTTP/1.1 204 Accepted
Content-type: application/json

{
  "id": "006111db-0810-4494-a6df-904d368bd81b",
  "displayName":"Connected organization new name",
  "description":"Connected organization new description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
