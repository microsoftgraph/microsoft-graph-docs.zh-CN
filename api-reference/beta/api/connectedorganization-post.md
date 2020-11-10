---
title: 创建 connectedOrganization
description: 创建新的 connectedOrganization。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c1866f57e1f8296c7035faae40372017c1af1c9e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957589"
---
# <a name="create-connectedorganization"></a><span data-ttu-id="709e5-103">创建 connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="709e5-103">Create connectedOrganization</span></span>

<span data-ttu-id="709e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="709e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="709e5-105">创建新的 [connectedOrganization](../resources/connectedorganization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="709e5-105">Create a new [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="709e5-106">权限</span><span class="sxs-lookup"><span data-stu-id="709e5-106">Permissions</span></span>

<span data-ttu-id="709e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="709e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="709e5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="709e5-109">Permission type</span></span>|<span data-ttu-id="709e5-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="709e5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="709e5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="709e5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="709e5-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="709e5-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="709e5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="709e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="709e5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="709e5-114">Not supported.</span></span> |
| <span data-ttu-id="709e5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="709e5-115">Application</span></span>                            | <span data-ttu-id="709e5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="709e5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="709e5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="709e5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="request-headers"></a><span data-ttu-id="709e5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="709e5-118">Request headers</span></span>

|<span data-ttu-id="709e5-119">名称</span><span class="sxs-lookup"><span data-stu-id="709e5-119">Name</span></span>|<span data-ttu-id="709e5-120">说明</span><span class="sxs-lookup"><span data-stu-id="709e5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="709e5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="709e5-121">Authorization</span></span>|<span data-ttu-id="709e5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="709e5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="709e5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="709e5-124">Content-Type</span></span>|<span data-ttu-id="709e5-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="709e5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="709e5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="709e5-127">Request body</span></span>
<span data-ttu-id="709e5-128">在请求正文中，提供 [connectedOrganization](../resources/connectedorganization.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="709e5-128">In the request body, supply a JSON representation of the [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

<span data-ttu-id="709e5-129">下表显示创建 [connectedOrganization](../resources/connectedorganization.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="709e5-129">The following table shows the properties that are required when you create the [connectedOrganization](../resources/connectedorganization.md).</span></span>

|<span data-ttu-id="709e5-130">属性</span><span class="sxs-lookup"><span data-stu-id="709e5-130">Property</span></span>|<span data-ttu-id="709e5-131">类型</span><span class="sxs-lookup"><span data-stu-id="709e5-131">Type</span></span>|<span data-ttu-id="709e5-132">说明</span><span class="sxs-lookup"><span data-stu-id="709e5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="709e5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="709e5-133">displayName</span></span>|<span data-ttu-id="709e5-134">String</span><span class="sxs-lookup"><span data-stu-id="709e5-134">String</span></span>|<span data-ttu-id="709e5-135">连接的组织名称。</span><span class="sxs-lookup"><span data-stu-id="709e5-135">The connected organization name.</span></span> |
|<span data-ttu-id="709e5-136">说明</span><span class="sxs-lookup"><span data-stu-id="709e5-136">description</span></span>|<span data-ttu-id="709e5-137">String</span><span class="sxs-lookup"><span data-stu-id="709e5-137">String</span></span>|<span data-ttu-id="709e5-138">连接的组织说明。</span><span class="sxs-lookup"><span data-stu-id="709e5-138">The connected organization description.</span></span>|
|<span data-ttu-id="709e5-139">identitySources</span><span class="sxs-lookup"><span data-stu-id="709e5-139">identitySources</span></span>|<span data-ttu-id="709e5-140">[identitySource](../resources/identitysource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="709e5-140">[identitySource](../resources/identitysource.md) collection</span></span>|<span data-ttu-id="709e5-141">包含一个元素（此连接组织中的初始标识源）的集合。</span><span class="sxs-lookup"><span data-stu-id="709e5-141">A collection with one element, the initial identity source in this connected organization.</span></span>|
|<span data-ttu-id="709e5-142">state</span><span class="sxs-lookup"><span data-stu-id="709e5-142">state</span></span>|<span data-ttu-id="709e5-143">connectedOrganizationState</span><span class="sxs-lookup"><span data-stu-id="709e5-143">connectedOrganizationState</span></span>|<span data-ttu-id="709e5-144">已连接组织的状态定义了请求者范围类型的工作分配策略是否 `AllConfiguredConnectedOrganizationSubjects` 适用。</span><span class="sxs-lookup"><span data-stu-id="709e5-144">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="709e5-145">可取值为：`configured`、`proposed`。</span><span class="sxs-lookup"><span data-stu-id="709e5-145">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="response"></a><span data-ttu-id="709e5-146">响应</span><span class="sxs-lookup"><span data-stu-id="709e5-146">Response</span></span>

<span data-ttu-id="709e5-147">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的 [connectedOrganization](../resources/connectedorganization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="709e5-147">If successful, this method returns a `201 Created` response code and a new [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="709e5-148">示例</span><span class="sxs-lookup"><span data-stu-id="709e5-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="709e5-149">请求</span><span class="sxs-lookup"><span data-stu-id="709e5-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="709e5-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="709e5-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connectedorganization_from_connectedorganizations"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/
Content-Type: application/json
Content-length: 100

{
  "displayName":"Connected organization name",
  "description":"Connected organization description",
  "identitySources": [
    {
      "@odata.type": "#microsoft.graph.domainIdentitySource",
      "domainName": "example.com",
      "displayName": "example.com"
      }
  ],
  "state":"proposed"
}
```
# <a name="c"></a>[<span data-ttu-id="709e5-151">C#</span><span class="sxs-lookup"><span data-stu-id="709e5-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connectedorganization-from-connectedorganizations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="709e5-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="709e5-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectedorganization-from-connectedorganizations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="709e5-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="709e5-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connectedorganization-from-connectedorganizations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="709e5-154">Java</span><span class="sxs-lookup"><span data-stu-id="709e5-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connectedorganization-from-connectedorganizations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="709e5-155">响应</span><span class="sxs-lookup"><span data-stu-id="709e5-155">Response</span></span>
<span data-ttu-id="709e5-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="709e5-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectedOrganization"
}
-->
``` http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "006111db-0810-4494-a6df-904d368bd81b",
  "displayName":"Connected organization name",
  "description":"Connected organization description",
  "createdBy": "admin@contoso.com",
  "createdDateTime": "2020-06-08T20:13:53.7099947Z",
  "modifiedBy": "admin@contoso.com",
  "modifiedDateTime": "2020-06-08T20:13:53.7099947Z",
  "state":"proposed"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


