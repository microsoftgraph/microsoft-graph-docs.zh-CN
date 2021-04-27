---
title: 创建 personWebsite
description: 创建新的 personWebsite。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f05a1cab47ef5500242cbda9fd0452a4e78a4750
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036700"
---
# <a name="create-personwebsite"></a><span data-ttu-id="91b2a-103">创建 personWebsite</span><span class="sxs-lookup"><span data-stu-id="91b2a-103">Create personWebsite</span></span>

<span data-ttu-id="91b2a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91b2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91b2a-105">在用户配置文件 [中创建新的 personWebsite](../resources/personwebsite.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="91b2a-105">Create a new [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="91b2a-106">权限</span><span class="sxs-lookup"><span data-stu-id="91b2a-106">Permissions</span></span>

<span data-ttu-id="91b2a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91b2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91b2a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="91b2a-109">Permission type</span></span>                        | <span data-ttu-id="91b2a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91b2a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="91b2a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91b2a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="91b2a-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91b2a-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="91b2a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91b2a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91b2a-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91b2a-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="91b2a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="91b2a-115">Application</span></span>                            | <span data-ttu-id="91b2a-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91b2a-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="91b2a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91b2a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/websites
POST /users/{id | userPrincipalName}/profile/websites
```

## <a name="request-headers"></a><span data-ttu-id="91b2a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="91b2a-118">Request headers</span></span>

| <span data-ttu-id="91b2a-119">名称</span><span class="sxs-lookup"><span data-stu-id="91b2a-119">Name</span></span>           | <span data-ttu-id="91b2a-120">说明</span><span class="sxs-lookup"><span data-stu-id="91b2a-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="91b2a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="91b2a-121">Authorization</span></span>  | <span data-ttu-id="91b2a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="91b2a-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="91b2a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91b2a-124">Content-Type</span></span>   | <span data-ttu-id="91b2a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="91b2a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91b2a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="91b2a-127">Request body</span></span>

<span data-ttu-id="91b2a-128">在请求正文中，提供 [personWebsite](../resources/personwebsite.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91b2a-128">In the request body, supply a JSON representation of the [personWebsite](../resources/personwebsite.md) object.</span></span>

<span data-ttu-id="91b2a-129">下表显示了在用户配置文件中的新 [personWebsite](../resources/personwebsite.md) 对象中可以设置 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="91b2a-129">The following table shows the properties that are possible to set within a new [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="91b2a-130">属性</span><span class="sxs-lookup"><span data-stu-id="91b2a-130">Property</span></span>|<span data-ttu-id="91b2a-131">类型</span><span class="sxs-lookup"><span data-stu-id="91b2a-131">Type</span></span>|<span data-ttu-id="91b2a-132">说明</span><span class="sxs-lookup"><span data-stu-id="91b2a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91b2a-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="91b2a-133">allowedAudiences</span></span>|<span data-ttu-id="91b2a-134">String</span><span class="sxs-lookup"><span data-stu-id="91b2a-134">String</span></span>|<span data-ttu-id="91b2a-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="91b2a-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="91b2a-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="91b2a-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="91b2a-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="91b2a-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="91b2a-138">categories</span><span class="sxs-lookup"><span data-stu-id="91b2a-138">categories</span></span>|<span data-ttu-id="91b2a-139">String 集合</span><span class="sxs-lookup"><span data-stu-id="91b2a-139">String collection</span></span>|<span data-ttu-id="91b2a-140">包含用户与网站网站关联的类别 (例如个人、食谱) 。</span><span class="sxs-lookup"><span data-stu-id="91b2a-140">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>|
|<span data-ttu-id="91b2a-141">说明</span><span class="sxs-lookup"><span data-stu-id="91b2a-141">description</span></span>|<span data-ttu-id="91b2a-142">String</span><span class="sxs-lookup"><span data-stu-id="91b2a-142">String</span></span>|<span data-ttu-id="91b2a-143">包含网站的说明。</span><span class="sxs-lookup"><span data-stu-id="91b2a-143">Contains a description of the website.</span></span>|
|<span data-ttu-id="91b2a-144">displayName</span><span class="sxs-lookup"><span data-stu-id="91b2a-144">displayName</span></span>|<span data-ttu-id="91b2a-145">String</span><span class="sxs-lookup"><span data-stu-id="91b2a-145">String</span></span>|<span data-ttu-id="91b2a-146">包含网站的友好名称。</span><span class="sxs-lookup"><span data-stu-id="91b2a-146">Contains a friendly name for the website.</span></span>|
|<span data-ttu-id="91b2a-147">inference</span><span class="sxs-lookup"><span data-stu-id="91b2a-147">inference</span></span>|[<span data-ttu-id="91b2a-148">inferenceData</span><span class="sxs-lookup"><span data-stu-id="91b2a-148">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="91b2a-149">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="91b2a-149">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="91b2a-150">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="91b2a-150">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="91b2a-151">source</span><span class="sxs-lookup"><span data-stu-id="91b2a-151">source</span></span>|[<span data-ttu-id="91b2a-152">personDataSource</span><span class="sxs-lookup"><span data-stu-id="91b2a-152">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="91b2a-153">如果从另一个服务同步，则值源自何处。</span><span class="sxs-lookup"><span data-stu-id="91b2a-153">Where the values originated if synced from another service.</span></span> <span data-ttu-id="91b2a-154">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="91b2a-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="91b2a-155">webUrl</span><span class="sxs-lookup"><span data-stu-id="91b2a-155">webUrl</span></span>|<span data-ttu-id="91b2a-156">String</span><span class="sxs-lookup"><span data-stu-id="91b2a-156">String</span></span>|<span data-ttu-id="91b2a-157">包含指向网站本身的链接。</span><span class="sxs-lookup"><span data-stu-id="91b2a-157">Contains a link to the website itself.</span></span>|

## <a name="response"></a><span data-ttu-id="91b2a-158">响应</span><span class="sxs-lookup"><span data-stu-id="91b2a-158">Response</span></span>

<span data-ttu-id="91b2a-159">如果成功，此方法在 `201, Created` 响应正文中返回 响应代码和新 [personWebsite](../resources/personwebsite.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="91b2a-159">If successful, this method returns `201, Created` response code and a new [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91b2a-160">示例</span><span class="sxs-lookup"><span data-stu-id="91b2a-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91b2a-161">请求</span><span class="sxs-lookup"><span data-stu-id="91b2a-161">Request</span></span>

<span data-ttu-id="91b2a-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="91b2a-162">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91b2a-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="91b2a-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personwebsite_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/websites
Content-type: application/json

{
  "categories": [
    "football"
  ],
  "displayName": "Lyn Damer",
  "webUrl": "www.lyndamer.no"
}
```
# <a name="c"></a>[<span data-ttu-id="91b2a-164">C#</span><span class="sxs-lookup"><span data-stu-id="91b2a-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personwebsite-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91b2a-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91b2a-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personwebsite-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91b2a-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91b2a-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personwebsite-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91b2a-167">Java</span><span class="sxs-lookup"><span data-stu-id="91b2a-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personwebsite-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="91b2a-168">响应</span><span class="sxs-lookup"><span data-stu-id="91b2a-168">Response</span></span>

<span data-ttu-id="91b2a-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="91b2a-169">The following is an example of the response.</span></span>

> <span data-ttu-id="91b2a-170">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="91b2a-170">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
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
  "categories": [
    "football"
  ],
  "description": null,
  "displayName": "Lyn Damer",
  "webUrl": "www.lyndamer.no"
}
```


