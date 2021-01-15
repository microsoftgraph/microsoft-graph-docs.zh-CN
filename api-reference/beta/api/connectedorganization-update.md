---
title: 更新 connectedOrganization 对象
description: 更新 connectedOrganization 对象。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 980fade00646062a6afe740e26cc5a9cdf976512
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872672"
---
# <a name="update-connectedorganization"></a><span data-ttu-id="7a3e3-103">更新 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="7a3e3-103">Update connectedOrganization</span></span>

<span data-ttu-id="7a3e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a3e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a3e3-105">更新 [connectedOrganization](../resources/connectedorganization.md) 对象以更改其一个或多个属性。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-105">Update a [connectedOrganization](../resources/connectedorganization.md) object to change one or more of its properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a3e3-106">权限</span><span class="sxs-lookup"><span data-stu-id="7a3e3-106">Permissions</span></span>
<span data-ttu-id="7a3e3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a3e3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a3e3-109">Permission type</span></span>|<span data-ttu-id="7a3e3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a3e3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a3e3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a3e3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a3e3-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a3e3-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="7a3e3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a3e3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a3e3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-114">Not supported.</span></span> |
|<span data-ttu-id="7a3e3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a3e3-115">Application</span></span>                            | <span data-ttu-id="7a3e3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a3e3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a3e3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7a3e3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a3e3-118">Request headers</span></span>
|<span data-ttu-id="7a3e3-119">名称</span><span class="sxs-lookup"><span data-stu-id="7a3e3-119">Name</span></span>|<span data-ttu-id="7a3e3-120">说明</span><span class="sxs-lookup"><span data-stu-id="7a3e3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7a3e3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a3e3-121">Authorization</span></span>|<span data-ttu-id="7a3e3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7a3e3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a3e3-124">Content-Type</span></span>|<span data-ttu-id="7a3e3-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7a3e3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a3e3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a3e3-127">Request body</span></span>
<span data-ttu-id="7a3e3-128">在请求正文中，提供 [connectedOrganization](../resources/connectedorganization.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="7a3e3-129">下表显示更新 [connectedOrganization](../resources/connectedorganization.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-129">The following table shows the properties that are required when you update the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="7a3e3-130">属性</span><span class="sxs-lookup"><span data-stu-id="7a3e3-130">Property</span></span>|<span data-ttu-id="7a3e3-131">类型</span><span class="sxs-lookup"><span data-stu-id="7a3e3-131">Type</span></span>|<span data-ttu-id="7a3e3-132">说明</span><span class="sxs-lookup"><span data-stu-id="7a3e3-132">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="7a3e3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="7a3e3-133">displayName</span></span>  |<span data-ttu-id="7a3e3-134">String</span><span class="sxs-lookup"><span data-stu-id="7a3e3-134">String</span></span> | <span data-ttu-id="7a3e3-135">连接的组织名称。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-135">The connected organization name.</span></span>  |
| <span data-ttu-id="7a3e3-136">说明</span><span class="sxs-lookup"><span data-stu-id="7a3e3-136">description</span></span>  |<span data-ttu-id="7a3e3-137">String</span><span class="sxs-lookup"><span data-stu-id="7a3e3-137">String</span></span> | <span data-ttu-id="7a3e3-138">连接的组织说明。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-138">The connected organization description.</span></span> |
| <span data-ttu-id="7a3e3-139">state</span><span class="sxs-lookup"><span data-stu-id="7a3e3-139">state</span></span>        |<span data-ttu-id="7a3e3-140">connectedOrganizationState</span><span class="sxs-lookup"><span data-stu-id="7a3e3-140">connectedOrganizationState</span></span>|<span data-ttu-id="7a3e3-141">已连接组织的状态定义具有请求者范围类型的分配策略 `AllConfiguredConnectedOrganizationSubjects` 是否适用。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-141">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="7a3e3-142">可取值为：`configured`、`proposed`。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-142">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="response"></a><span data-ttu-id="7a3e3-143">响应</span><span class="sxs-lookup"><span data-stu-id="7a3e3-143">Response</span></span>

<span data-ttu-id="7a3e3-144">如果成功，此方法在响应 `204 Accepted` 正文中返回响应代码和 [connectedOrganization](../resources/connectedorganization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-144">If successful, this method returns a `204 Accepted` response code and a [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a3e3-145">示例</span><span class="sxs-lookup"><span data-stu-id="7a3e3-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a3e3-146">请求</span><span class="sxs-lookup"><span data-stu-id="7a3e3-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7a3e3-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a3e3-147">HTTP</span></span>](#tab/http)
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
  "description":"Connected organization new description",
  "state":"configured"
}
```
# <a name="c"></a>[<span data-ttu-id="7a3e3-148">C#</span><span class="sxs-lookup"><span data-stu-id="7a3e3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a3e3-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a3e3-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a3e3-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a3e3-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a3e3-151">Java</span><span class="sxs-lookup"><span data-stu-id="7a3e3-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7a3e3-152">响应</span><span class="sxs-lookup"><span data-stu-id="7a3e3-152">Response</span></span>
<span data-ttu-id="7a3e3-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description":"Connected organization new description",
  "state":"configured"
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


