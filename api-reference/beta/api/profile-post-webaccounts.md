---
title: 创建 webAccount
description: 创建新的 webAccount 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b1bcf743737616ac5c48d3b8c3132b57d11464ac
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812195"
---
# <a name="create-webaccount"></a><span data-ttu-id="218ed-103">创建 webAccount</span><span class="sxs-lookup"><span data-stu-id="218ed-103">Create webAccount</span></span>

<span data-ttu-id="218ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="218ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="218ed-105">在用户的[配置文件](../resources/profile.md)中创建新的[webAccount](../resources/webaccount.md)对象。</span><span class="sxs-lookup"><span data-stu-id="218ed-105">Create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="218ed-106">权限</span><span class="sxs-lookup"><span data-stu-id="218ed-106">Permissions</span></span>

<span data-ttu-id="218ed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="218ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="218ed-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="218ed-109">Permission type</span></span>                        | <span data-ttu-id="218ed-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="218ed-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="218ed-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="218ed-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="218ed-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="218ed-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="218ed-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="218ed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="218ed-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="218ed-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="218ed-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="218ed-115">Application</span></span>                            | <span data-ttu-id="218ed-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="218ed-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="218ed-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="218ed-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/webAccounts
POST /users/{id | userPrincipalName}/profile/webAccounts
```

## <a name="request-headers"></a><span data-ttu-id="218ed-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="218ed-118">Request headers</span></span>

| <span data-ttu-id="218ed-119">名称</span><span class="sxs-lookup"><span data-stu-id="218ed-119">Name</span></span>           | <span data-ttu-id="218ed-120">说明</span><span class="sxs-lookup"><span data-stu-id="218ed-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="218ed-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="218ed-121">Authorization</span></span>  | <span data-ttu-id="218ed-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="218ed-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="218ed-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="218ed-124">Content-Type</span></span>   | <span data-ttu-id="218ed-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="218ed-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="218ed-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="218ed-127">Request body</span></span>

<span data-ttu-id="218ed-128">在请求正文中，提供 [webAccount](../resources/webaccount.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="218ed-128">In the request body, supply a JSON representation of [webAccount](../resources/webaccount.md) object.</span></span>

<span data-ttu-id="218ed-129">下表显示了在用户的[配置文件](../resources/profile.md)中创建新的[webAccount](../resources/webaccount.md)对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="218ed-129">The following table shows the properties that are possible to set when you create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="218ed-130">属性</span><span class="sxs-lookup"><span data-stu-id="218ed-130">Property</span></span>|<span data-ttu-id="218ed-131">类型</span><span class="sxs-lookup"><span data-stu-id="218ed-131">Type</span></span>|<span data-ttu-id="218ed-132">说明</span><span class="sxs-lookup"><span data-stu-id="218ed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="218ed-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="218ed-133">allowedAudiences</span></span>|<span data-ttu-id="218ed-134">String</span><span class="sxs-lookup"><span data-stu-id="218ed-134">String</span></span>|<span data-ttu-id="218ed-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="218ed-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="218ed-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="218ed-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="218ed-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="218ed-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="218ed-138">description</span><span class="sxs-lookup"><span data-stu-id="218ed-138">description</span></span>|<span data-ttu-id="218ed-139">String</span><span class="sxs-lookup"><span data-stu-id="218ed-139">String</span></span>|<span data-ttu-id="218ed-140">包含用户为所引用服务上的帐户提供的说明。</span><span class="sxs-lookup"><span data-stu-id="218ed-140">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="218ed-141">推导</span><span class="sxs-lookup"><span data-stu-id="218ed-141">inference</span></span>|[<span data-ttu-id="218ed-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="218ed-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="218ed-143">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="218ed-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="218ed-144">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="218ed-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="218ed-145">service</span><span class="sxs-lookup"><span data-stu-id="218ed-145">service</span></span>|[<span data-ttu-id="218ed-146">serviceInformation</span><span class="sxs-lookup"><span data-stu-id="218ed-146">serviceInformation</span></span>](../resources/serviceinformation.md)| <span data-ttu-id="218ed-147">包含有关要关联的服务的基本详细信息。</span><span class="sxs-lookup"><span data-stu-id="218ed-147">Contains basic detail about the service that is being associated.</span></span> |
|<span data-ttu-id="218ed-148">source</span><span class="sxs-lookup"><span data-stu-id="218ed-148">source</span></span>|[<span data-ttu-id="218ed-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="218ed-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="218ed-150">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="218ed-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="218ed-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="218ed-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="218ed-152">statusMessage</span><span class="sxs-lookup"><span data-stu-id="218ed-152">statusMessage</span></span>|<span data-ttu-id="218ed-153">String</span><span class="sxs-lookup"><span data-stu-id="218ed-153">String</span></span>|<span data-ttu-id="218ed-154">包含来自云服务的状态邮件（如果提供或已同步）。</span><span class="sxs-lookup"><span data-stu-id="218ed-154">Contains a status message from the cloud service if provided or synchronized.</span></span> |
|<span data-ttu-id="218ed-155">userId</span><span class="sxs-lookup"><span data-stu-id="218ed-155">userId</span></span>|<span data-ttu-id="218ed-156">String</span><span class="sxs-lookup"><span data-stu-id="218ed-156">String</span></span>|<span data-ttu-id="218ed-157">为 webaccount 显示的用户名。</span><span class="sxs-lookup"><span data-stu-id="218ed-157">The user name  displayed for the webaccount.</span></span>  |
|<span data-ttu-id="218ed-158">webUrl</span><span class="sxs-lookup"><span data-stu-id="218ed-158">webUrl</span></span>|<span data-ttu-id="218ed-159">String</span><span class="sxs-lookup"><span data-stu-id="218ed-159">String</span></span>|<span data-ttu-id="218ed-160">包含指向云服务上的用户配置文件的链接（如果存在）。</span><span class="sxs-lookup"><span data-stu-id="218ed-160">Contains a link to the user's profile on the cloud service if one exists.</span></span>|

## <a name="response"></a><span data-ttu-id="218ed-161">响应</span><span class="sxs-lookup"><span data-stu-id="218ed-161">Response</span></span>

<span data-ttu-id="218ed-162">如果成功，此方法 `201, Created` 在响应正文中返回响应代码和新的 [webAccount](../resources/webaccount.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="218ed-162">If successful, this method returns `201, Created` response code and a new [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="218ed-163">示例</span><span class="sxs-lookup"><span data-stu-id="218ed-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="218ed-164">请求</span><span class="sxs-lookup"><span data-stu-id="218ed-164">Request</span></span>

<span data-ttu-id="218ed-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="218ed-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="218ed-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="218ed-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_webaccount_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/webAccounts
Content-type: application/json

{
  "description": "My Github contributions!",
  "userId": "innocenty.popov",
  "service": {
    "name": "GitHub",
    "webUrl": "https://github.com"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="218ed-167">C#</span><span class="sxs-lookup"><span data-stu-id="218ed-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-webaccount-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="218ed-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="218ed-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-webaccount-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="218ed-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="218ed-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-webaccount-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="218ed-170">响应</span><span class="sxs-lookup"><span data-stu-id="218ed-170">Response</span></span>

<span data-ttu-id="218ed-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="218ed-171">The following is an example of the response.</span></span>

> <span data-ttu-id="218ed-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="218ed-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "description": "My Github contributions!",
  "userId": "innocenty.popov",
  "service": {
    "name": "GitHub",
    "webUrl": "https://github.com"
  },
  "statusMessage": null,
  "webUrl": "https://github.com/innocenty.popov"
}
```
