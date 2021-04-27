---
title: 创建 webAccount
description: 创建新的 webAccount 对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 2d41cb9fe650fa8d506f8ea9c218a01d4f2c0605
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036763"
---
# <a name="create-webaccount"></a><span data-ttu-id="38d78-103">创建 webAccount</span><span class="sxs-lookup"><span data-stu-id="38d78-103">Create webAccount</span></span>

<span data-ttu-id="38d78-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38d78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38d78-105">在用户配置文件中创建新的 [webAccount](../resources/webaccount.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="38d78-105">Create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="38d78-106">权限</span><span class="sxs-lookup"><span data-stu-id="38d78-106">Permissions</span></span>

<span data-ttu-id="38d78-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38d78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38d78-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="38d78-109">Permission type</span></span>                        | <span data-ttu-id="38d78-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38d78-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="38d78-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38d78-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="38d78-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38d78-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="38d78-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38d78-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38d78-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38d78-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="38d78-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="38d78-115">Application</span></span>                            | <span data-ttu-id="38d78-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38d78-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="38d78-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38d78-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/webAccounts
POST /users/{id | userPrincipalName}/profile/webAccounts
```

## <a name="request-headers"></a><span data-ttu-id="38d78-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="38d78-118">Request headers</span></span>

| <span data-ttu-id="38d78-119">名称</span><span class="sxs-lookup"><span data-stu-id="38d78-119">Name</span></span>           | <span data-ttu-id="38d78-120">说明</span><span class="sxs-lookup"><span data-stu-id="38d78-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="38d78-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="38d78-121">Authorization</span></span>  | <span data-ttu-id="38d78-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38d78-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="38d78-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38d78-124">Content-Type</span></span>   | <span data-ttu-id="38d78-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="38d78-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38d78-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="38d78-127">Request body</span></span>

<span data-ttu-id="38d78-128">在请求正文中，提供 [webAccount](../resources/webaccount.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38d78-128">In the request body, supply a JSON representation of [webAccount](../resources/webaccount.md) object.</span></span>

<span data-ttu-id="38d78-129">下表显示了在用户配置文件中创建新的 [webAccount](../resources/webaccount.md) 对象时可以设置 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="38d78-129">The following table shows the properties that are possible to set when you create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="38d78-130">属性</span><span class="sxs-lookup"><span data-stu-id="38d78-130">Property</span></span>|<span data-ttu-id="38d78-131">类型</span><span class="sxs-lookup"><span data-stu-id="38d78-131">Type</span></span>|<span data-ttu-id="38d78-132">说明</span><span class="sxs-lookup"><span data-stu-id="38d78-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38d78-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="38d78-133">allowedAudiences</span></span>|<span data-ttu-id="38d78-134">String</span><span class="sxs-lookup"><span data-stu-id="38d78-134">String</span></span>|<span data-ttu-id="38d78-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="38d78-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="38d78-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="38d78-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="38d78-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="38d78-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="38d78-138">说明</span><span class="sxs-lookup"><span data-stu-id="38d78-138">description</span></span>|<span data-ttu-id="38d78-139">String</span><span class="sxs-lookup"><span data-stu-id="38d78-139">String</span></span>|<span data-ttu-id="38d78-140">包含用户为引用的服务上的帐户提供的说明。</span><span class="sxs-lookup"><span data-stu-id="38d78-140">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="38d78-141">inference</span><span class="sxs-lookup"><span data-stu-id="38d78-141">inference</span></span>|[<span data-ttu-id="38d78-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="38d78-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="38d78-143">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="38d78-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="38d78-144">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="38d78-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="38d78-145">服务</span><span class="sxs-lookup"><span data-stu-id="38d78-145">service</span></span>|[<span data-ttu-id="38d78-146">serviceInformation</span><span class="sxs-lookup"><span data-stu-id="38d78-146">serviceInformation</span></span>](../resources/serviceinformation.md)| <span data-ttu-id="38d78-147">包含有关要关联的服务的基本详细信息。</span><span class="sxs-lookup"><span data-stu-id="38d78-147">Contains basic detail about the service that is being associated.</span></span> |
|<span data-ttu-id="38d78-148">source</span><span class="sxs-lookup"><span data-stu-id="38d78-148">source</span></span>|[<span data-ttu-id="38d78-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="38d78-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="38d78-150">如果从另一个服务同步，则值源自何处。</span><span class="sxs-lookup"><span data-stu-id="38d78-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="38d78-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="38d78-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="38d78-152">statusMessage</span><span class="sxs-lookup"><span data-stu-id="38d78-152">statusMessage</span></span>|<span data-ttu-id="38d78-153">String</span><span class="sxs-lookup"><span data-stu-id="38d78-153">String</span></span>|<span data-ttu-id="38d78-154">包含来自云服务的状态消息（如果提供或同步）。</span><span class="sxs-lookup"><span data-stu-id="38d78-154">Contains a status message from the cloud service if provided or synchronized.</span></span> |
|<span data-ttu-id="38d78-155">userId</span><span class="sxs-lookup"><span data-stu-id="38d78-155">userId</span></span>|<span data-ttu-id="38d78-156">String</span><span class="sxs-lookup"><span data-stu-id="38d78-156">String</span></span>|<span data-ttu-id="38d78-157">为 webaccount 显示的用户名。</span><span class="sxs-lookup"><span data-stu-id="38d78-157">The user name  displayed for the webaccount.</span></span>  |
|<span data-ttu-id="38d78-158">webUrl</span><span class="sxs-lookup"><span data-stu-id="38d78-158">webUrl</span></span>|<span data-ttu-id="38d78-159">String</span><span class="sxs-lookup"><span data-stu-id="38d78-159">String</span></span>|<span data-ttu-id="38d78-160">包含指向云服务上的用户配置文件的链接（如果存在）。</span><span class="sxs-lookup"><span data-stu-id="38d78-160">Contains a link to the user's profile on the cloud service if one exists.</span></span>|

## <a name="response"></a><span data-ttu-id="38d78-161">响应</span><span class="sxs-lookup"><span data-stu-id="38d78-161">Response</span></span>

<span data-ttu-id="38d78-162">如果成功，此方法在 `201, Created` 响应正文中返回 响应代码和新 [webAccount](../resources/webaccount.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="38d78-162">If successful, this method returns `201, Created` response code and a new [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="38d78-163">示例</span><span class="sxs-lookup"><span data-stu-id="38d78-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="38d78-164">请求</span><span class="sxs-lookup"><span data-stu-id="38d78-164">Request</span></span>

<span data-ttu-id="38d78-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="38d78-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="38d78-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="38d78-166">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="38d78-167">C#</span><span class="sxs-lookup"><span data-stu-id="38d78-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-webaccount-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38d78-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38d78-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-webaccount-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38d78-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38d78-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-webaccount-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38d78-170">Java</span><span class="sxs-lookup"><span data-stu-id="38d78-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-webaccount-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="38d78-171">响应</span><span class="sxs-lookup"><span data-stu-id="38d78-171">Response</span></span>

<span data-ttu-id="38d78-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="38d78-172">The following is an example of the response.</span></span>

> <span data-ttu-id="38d78-173">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="38d78-173">**Note:** The response object shown here might be shortened for readability.</span></span>

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


