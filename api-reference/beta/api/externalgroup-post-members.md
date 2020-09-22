---
title: 创建 externalGroupMember
description: 创建新的 externalGroupMember 对象。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c66c21e4b0842df4fb7ececa3378249347f3002d
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193845"
---
# <a name="create-externalgroupmember"></a><span data-ttu-id="ac429-103">创建 externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="ac429-103">Create externalGroupMember</span></span>

<span data-ttu-id="ac429-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac429-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac429-105">创建新的 [externalGroupMember](../resources/externalgroupmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ac429-105">Create a new [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac429-106">权限</span><span class="sxs-lookup"><span data-stu-id="ac429-106">Permissions</span></span>

<span data-ttu-id="ac429-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac429-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac429-109">Permission type</span></span>                        | <span data-ttu-id="ac429-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ac429-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ac429-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac429-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac429-112">不支持</span><span class="sxs-lookup"><span data-stu-id="ac429-112">Not supported</span></span>                               |
| <span data-ttu-id="ac429-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac429-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac429-114">不支持</span><span class="sxs-lookup"><span data-stu-id="ac429-114">Not supported</span></span>                               |
| <span data-ttu-id="ac429-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac429-115">Application</span></span>                            | <span data-ttu-id="ac429-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac429-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="ac429-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac429-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionsId}/groups/{externalGroupId}/members
```

## <a name="request-headers"></a><span data-ttu-id="ac429-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac429-118">Request headers</span></span>

| <span data-ttu-id="ac429-119">名称</span><span class="sxs-lookup"><span data-stu-id="ac429-119">Name</span></span>          | <span data-ttu-id="ac429-120">说明</span><span class="sxs-lookup"><span data-stu-id="ac429-120">Description</span></span>                 |
|:--------------|:----------------------------|
| <span data-ttu-id="ac429-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac429-121">Authorization</span></span> | <span data-ttu-id="ac429-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac429-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ac429-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ac429-124">Content-Type</span></span>  | <span data-ttu-id="ac429-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ac429-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac429-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac429-127">Request body</span></span>

<span data-ttu-id="ac429-128">在请求正文中，提供 [externalGroupMember](../resources/externalgroupmember.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac429-128">In the request body, supply a JSON representation of the [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

<span data-ttu-id="ac429-129">下表显示创建 [externalGroupMember](../resources/externalgroupmember.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ac429-129">The following table shows the properties that are required when you create the [externalGroupMember](../resources/externalgroupmember.md).</span></span>

| <span data-ttu-id="ac429-130">属性</span><span class="sxs-lookup"><span data-stu-id="ac429-130">Property</span></span>       | <span data-ttu-id="ac429-131">类型</span><span class="sxs-lookup"><span data-stu-id="ac429-131">Type</span></span>                    | <span data-ttu-id="ac429-132">说明</span><span class="sxs-lookup"><span data-stu-id="ac429-132">Description</span></span>                                              |
|:---------------|:------------------------|:---------------------------------------------------------|
| <span data-ttu-id="ac429-133">id</span><span class="sxs-lookup"><span data-stu-id="ac429-133">id</span></span>             | <span data-ttu-id="ac429-134">字符串</span><span class="sxs-lookup"><span data-stu-id="ac429-134">String</span></span>                  | <span data-ttu-id="ac429-135">成员的唯一 `id` 。</span><span class="sxs-lookup"><span data-stu-id="ac429-135">The unique `id` of the member.</span></span> <span data-ttu-id="ac429-136">在 Azure Active Directory 用户或组以及外部组的情况下，它将是 externalGroupId 的 objectId。</span><span class="sxs-lookup"><span data-stu-id="ac429-136">It would be the objectId in case of Azure Active Directory users or groups and the externalGroupId in case of external groups.</span></span>                                    |
| <span data-ttu-id="ac429-137">type</span><span class="sxs-lookup"><span data-stu-id="ac429-137">type</span></span>           | <span data-ttu-id="ac429-138">externalGroupMemberType</span><span class="sxs-lookup"><span data-stu-id="ac429-138">externalGroupMemberType</span></span> | <span data-ttu-id="ac429-139">添加到外部组的成员类型。</span><span class="sxs-lookup"><span data-stu-id="ac429-139">The type of member added to the external group.</span></span> <span data-ttu-id="ac429-140">可能的值为： `user` 或者 `group` 当 identitySource 是 `azureActiveDirectory` identitySource 时， `group` `external` 则为。</span><span class="sxs-lookup"><span data-stu-id="ac429-140">Possible values are: `user` or `group` when the identitySource is `azureActiveDirectory` and just `group` when the identitySource is `external`.</span></span> |
| <span data-ttu-id="ac429-141">identitySource</span><span class="sxs-lookup"><span data-stu-id="ac429-141">identitySource</span></span> | <span data-ttu-id="ac429-142">identitySourceType</span><span class="sxs-lookup"><span data-stu-id="ac429-142">identitySourceType</span></span>      | <span data-ttu-id="ac429-143">成员所属的标识源。</span><span class="sxs-lookup"><span data-stu-id="ac429-143">The identity source that the member belongs to.</span></span> <span data-ttu-id="ac429-144">可取值为：`azureActiveDirectory`、`external`。</span><span class="sxs-lookup"><span data-stu-id="ac429-144">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="response"></a><span data-ttu-id="ac429-145">响应</span><span class="sxs-lookup"><span data-stu-id="ac429-145">Response</span></span>

<span data-ttu-id="ac429-146">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [externalGroupMember](../resources/externalgroupmember.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ac429-146">If successful, this method returns a `201 Created` response code and an [externalGroupMember](../resources/externalgroupmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac429-147">示例</span><span class="sxs-lookup"><span data-stu-id="ac429-147">Examples</span></span>

### <a name="example-1-add-an-azure-active-directory-user-as-a-member"></a><span data-ttu-id="ac429-148">示例1：将 Azure Active Directory 用户添加为成员</span><span class="sxs-lookup"><span data-stu-id="ac429-148">Example 1: Add an Azure Active Directory user as a member</span></span>

### <a name="request"></a><span data-ttu-id="ac429-149">请求</span><span class="sxs-lookup"><span data-stu-id="ac429-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="ac429-150">响应</span><span class="sxs-lookup"><span data-stu-id="ac429-150">Response</span></span>

<span data-ttu-id="ac429-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ac429-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-2-add-an-azure-active-directory-group-as-a-member"></a><span data-ttu-id="ac429-152">示例2：将 Azure Active Directory 组添加为成员</span><span class="sxs-lookup"><span data-stu-id="ac429-152">Example 2: Add an Azure Active Directory group as a member</span></span>

### <a name="request"></a><span data-ttu-id="ac429-153">请求</span><span class="sxs-lookup"><span data-stu-id="ac429-153">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="response"></a><span data-ttu-id="ac429-154">响应</span><span class="sxs-lookup"><span data-stu-id="ac429-154">Response</span></span>

<span data-ttu-id="ac429-155">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ac429-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-3-add-another-external-group-as-a-member"></a><span data-ttu-id="ac429-156">示例3：将另一个外部组添加为成员</span><span class="sxs-lookup"><span data-stu-id="ac429-156">Example 3: Add another external group as a member</span></span>

### <a name="request"></a><span data-ttu-id="ac429-157">请求</span><span class="sxs-lookup"><span data-stu-id="ac429-157">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "1431b9c38ee647f6a",
  "type": "group",
  "identitySource": "external"
}
```

### <a name="response"></a><span data-ttu-id="ac429-158">响应</span><span class="sxs-lookup"><span data-stu-id="ac429-158">Response</span></span>

<span data-ttu-id="ac429-159">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ac429-159">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "14m1b9c38qe647f6a",
  "type": "group",
  "identitySource": "external"
}
```
