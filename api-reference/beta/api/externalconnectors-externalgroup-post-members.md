---
title: 创建 externalGroupMember
description: 创建新的 externalGroupMember 对象。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 3120c6aa7744aeedebf8fa6b4eb1a696b21e6e37
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467576"
---
# <a name="create-externalgroupmember"></a><span data-ttu-id="4f2fc-103">创建 externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="4f2fc-103">Create externalGroupMember</span></span>

<span data-ttu-id="4f2fc-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="4f2fc-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f2fc-105">创建新的 [externalGroupMember](../resources/externalconnectors-externalgroupmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f2fc-105">Create a new [externalGroupMember](../resources/externalconnectors-externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f2fc-106">权限</span><span class="sxs-lookup"><span data-stu-id="4f2fc-106">Permissions</span></span>

<span data-ttu-id="4f2fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f2fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f2fc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f2fc-109">Permission type</span></span>                        | <span data-ttu-id="4f2fc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f2fc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4f2fc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f2fc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f2fc-112">不支持</span><span class="sxs-lookup"><span data-stu-id="4f2fc-112">Not supported</span></span>                               |
| <span data-ttu-id="4f2fc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f2fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f2fc-114">不支持</span><span class="sxs-lookup"><span data-stu-id="4f2fc-114">Not supported</span></span>                               |
| <span data-ttu-id="4f2fc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f2fc-115">Application</span></span>                            | <span data-ttu-id="4f2fc-116">ExternalItem.ReadWrite.OwnedBy、ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f2fc-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="4f2fc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f2fc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionsId}/groups/{externalGroupId}/members
```

## <a name="request-headers"></a><span data-ttu-id="4f2fc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f2fc-118">Request headers</span></span>

| <span data-ttu-id="4f2fc-119">名称</span><span class="sxs-lookup"><span data-stu-id="4f2fc-119">Name</span></span>          | <span data-ttu-id="4f2fc-120">说明</span><span class="sxs-lookup"><span data-stu-id="4f2fc-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="4f2fc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f2fc-121">Authorization</span></span> | <span data-ttu-id="4f2fc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f2fc-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="4f2fc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4f2fc-124">Content-Type</span></span>  | <span data-ttu-id="4f2fc-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4f2fc-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f2fc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f2fc-127">Request body</span></span>

<span data-ttu-id="4f2fc-128">在请求正文中，提供 [externalGroupMember](../resources/externalconnectors-externalgroupmember.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f2fc-128">In the request body, supply a JSON representation of the [externalGroupMember](../resources/externalconnectors-externalgroupmember.md) object.</span></span>

<span data-ttu-id="4f2fc-129">下表显示创建 [externalGroupMember 时所需的属性](../resources/externalconnectors-externalgroupmember.md)。</span><span class="sxs-lookup"><span data-stu-id="4f2fc-129">The following table shows the properties that are required when you create the [externalGroupMember](../resources/externalconnectors-externalgroupmember.md).</span></span>

| <span data-ttu-id="4f2fc-130">属性</span><span class="sxs-lookup"><span data-stu-id="4f2fc-130">Property</span></span>       | <span data-ttu-id="4f2fc-131">类型</span><span class="sxs-lookup"><span data-stu-id="4f2fc-131">Type</span></span>                    | <span data-ttu-id="4f2fc-132">说明</span><span class="sxs-lookup"><span data-stu-id="4f2fc-132">Description</span></span>                                              |
|:---------------|:------------------------|:---------------------------------------------------------|
| <span data-ttu-id="4f2fc-133">id</span><span class="sxs-lookup"><span data-stu-id="4f2fc-133">id</span></span>             | <span data-ttu-id="4f2fc-134">String</span><span class="sxs-lookup"><span data-stu-id="4f2fc-134">String</span></span>                  | <span data-ttu-id="4f2fc-135">成员 `id` 的唯一性。</span><span class="sxs-lookup"><span data-stu-id="4f2fc-135">The unique `id` of the member.</span></span> <span data-ttu-id="4f2fc-136">对于用户或组，它Azure Active Directory objectId，对于外部组，为 externalGroupId。</span><span class="sxs-lookup"><span data-stu-id="4f2fc-136">It would be the objectId in case of Azure Active Directory users or groups and the externalGroupId in case of external groups.</span></span>                                    |
| <span data-ttu-id="4f2fc-137">type</span><span class="sxs-lookup"><span data-stu-id="4f2fc-137">type</span></span>           | <span data-ttu-id="4f2fc-138">microsoft.graph.externalConnectors.externalGroupMemberType</span><span class="sxs-lookup"><span data-stu-id="4f2fc-138">microsoft.graph.externalConnectors.externalGroupMemberType</span></span> | <span data-ttu-id="4f2fc-139">添加到外部组的成员的类型。</span><span class="sxs-lookup"><span data-stu-id="4f2fc-139">The type of member added to the external group.</span></span> <span data-ttu-id="4f2fc-140">可能的值是： `user` 或当 identitySource 为 时，或者 `group` 当 `azureActiveDirectory` `group` identitySource 为 `external` 时。</span><span class="sxs-lookup"><span data-stu-id="4f2fc-140">Possible values are: `user` or `group` when the identitySource is `azureActiveDirectory` and just `group` when the identitySource is `external`.</span></span> |
| <span data-ttu-id="4f2fc-141">identitySource</span><span class="sxs-lookup"><span data-stu-id="4f2fc-141">identitySource</span></span> | <span data-ttu-id="4f2fc-142">microsoft.graph.externalConnectors.identitySourceType</span><span class="sxs-lookup"><span data-stu-id="4f2fc-142">microsoft.graph.externalConnectors.identitySourceType</span></span>      | <span data-ttu-id="4f2fc-143">成员所属的标识源。</span><span class="sxs-lookup"><span data-stu-id="4f2fc-143">The identity source that the member belongs to.</span></span> <span data-ttu-id="4f2fc-144">可取值为：`azureActiveDirectory`、`external`。</span><span class="sxs-lookup"><span data-stu-id="4f2fc-144">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="response"></a><span data-ttu-id="4f2fc-145">响应</span><span class="sxs-lookup"><span data-stu-id="4f2fc-145">Response</span></span>

<span data-ttu-id="4f2fc-146">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [externalGroupMember](../resources/externalconnectors-externalgroupmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f2fc-146">If successful, this method returns a `201 Created` response code and an [externalGroupMember](../resources/externalconnectors-externalgroupmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f2fc-147">示例</span><span class="sxs-lookup"><span data-stu-id="4f2fc-147">Examples</span></span>

### <a name="example-1-add-an-azure-active-directory-user-as-a-member"></a><span data-ttu-id="4f2fc-148">示例 1：将Azure Active Directory用户添加为成员</span><span class="sxs-lookup"><span data-stu-id="4f2fc-148">Example 1: Add an Azure Active Directory user as a member</span></span>

### <a name="request"></a><span data-ttu-id="4f2fc-149">请求</span><span class="sxs-lookup"><span data-stu-id="4f2fc-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4f2fc-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f2fc-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from__1"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```
# <a name="c"></a>[<span data-ttu-id="4f2fc-151">C#</span><span class="sxs-lookup"><span data-stu-id="4f2fc-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroupmember-from--1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f2fc-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f2fc-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroupmember-from--1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f2fc-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f2fc-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroupmember-from--1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f2fc-154">Java</span><span class="sxs-lookup"><span data-stu-id="4f2fc-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroupmember-from--1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="4f2fc-155">响应</span><span class="sxs-lookup"><span data-stu-id="4f2fc-155">Response</span></span>

<span data-ttu-id="4f2fc-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4f2fc-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-2-add-an-azure-active-directory-group-as-a-member"></a><span data-ttu-id="4f2fc-157">示例 2：将Azure Active Directory组添加为成员</span><span class="sxs-lookup"><span data-stu-id="4f2fc-157">Example 2: Add an Azure Active Directory group as a member</span></span>

### <a name="request"></a><span data-ttu-id="4f2fc-158">请求</span><span class="sxs-lookup"><span data-stu-id="4f2fc-158">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4f2fc-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f2fc-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from__2"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```
# <a name="c"></a>[<span data-ttu-id="4f2fc-160">C#</span><span class="sxs-lookup"><span data-stu-id="4f2fc-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroupmember-from--2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f2fc-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f2fc-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroupmember-from--2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f2fc-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f2fc-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroupmember-from--2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f2fc-163">Java</span><span class="sxs-lookup"><span data-stu-id="4f2fc-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroupmember-from--2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f2fc-164">响应</span><span class="sxs-lookup"><span data-stu-id="4f2fc-164">Response</span></span>

<span data-ttu-id="4f2fc-165">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4f2fc-165">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-3-add-another-external-group-as-a-member"></a><span data-ttu-id="4f2fc-166">示例 3：将另一个外部组添加为成员</span><span class="sxs-lookup"><span data-stu-id="4f2fc-166">Example 3: Add another external group as a member</span></span>

### <a name="request"></a><span data-ttu-id="4f2fc-167">请求</span><span class="sxs-lookup"><span data-stu-id="4f2fc-167">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4f2fc-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f2fc-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from__3"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "id": "1431b9c38ee647f6a",
  "type": "group",
  "identitySource": "external"
}
```
# <a name="c"></a>[<span data-ttu-id="4f2fc-169">C#</span><span class="sxs-lookup"><span data-stu-id="4f2fc-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroupmember-from--3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f2fc-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f2fc-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroupmember-from--3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f2fc-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f2fc-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroupmember-from--3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f2fc-172">Java</span><span class="sxs-lookup"><span data-stu-id="4f2fc-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroupmember-from--3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f2fc-173">响应</span><span class="sxs-lookup"><span data-stu-id="4f2fc-173">Response</span></span>

<span data-ttu-id="4f2fc-174">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4f2fc-174">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "14m1b9c38qe647f6a",
  "type": "group",
  "identitySource": "external"
}
```
