---
title: 创建 personInterest
description: 创建新的 personInterest。
localization_priority: Normal
author: kevinbellinger
ms.prod: People
doc_type: apiPageType
ms.openlocfilehash: e4f5648901ff1ed904d5e02fa278b6b9be329de8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036924"
---
# <a name="create-personinterest"></a><span data-ttu-id="3aa0f-103">创建 personInterest</span><span class="sxs-lookup"><span data-stu-id="3aa0f-103">Create personInterest</span></span>

<span data-ttu-id="3aa0f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aa0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3aa0f-105">创建新的 [personInterest] (。/resources/personinterest.md] in a [user's profile](../resources/profile.md).</span><span class="sxs-lookup"><span data-stu-id="3aa0f-105">Create a new [personInterest](../resources/personinterest.md] in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3aa0f-106">权限</span><span class="sxs-lookup"><span data-stu-id="3aa0f-106">Permissions</span></span>

<span data-ttu-id="3aa0f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3aa0f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3aa0f-109">Permission type</span></span>                        | <span data-ttu-id="3aa0f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3aa0f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3aa0f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3aa0f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3aa0f-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3aa0f-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3aa0f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3aa0f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aa0f-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3aa0f-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3aa0f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3aa0f-115">Application</span></span>                            | <span data-ttu-id="3aa0f-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3aa0f-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="3aa0f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3aa0f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/interests
POST /users/{id | userPrincipalName}/profile/interests
```

## <a name="request-headers"></a><span data-ttu-id="3aa0f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3aa0f-118">Request headers</span></span>

| <span data-ttu-id="3aa0f-119">名称</span><span class="sxs-lookup"><span data-stu-id="3aa0f-119">Name</span></span>      |<span data-ttu-id="3aa0f-120">说明</span><span class="sxs-lookup"><span data-stu-id="3aa0f-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3aa0f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3aa0f-121">Authorization</span></span>  | <span data-ttu-id="3aa0f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="3aa0f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3aa0f-124">Content-Type</span></span>   | <span data-ttu-id="3aa0f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3aa0f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3aa0f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3aa0f-127">Request body</span></span>

<span data-ttu-id="3aa0f-128">在请求正文中，提供 [personInterest](../resources/personinterest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-128">In the request body, supply a JSON representation of the [personInterest](../resources/personinterest.md) object.</span></span>

<span data-ttu-id="3aa0f-129">下表显示了在用户配置文件中的新 [personInterest](../resources/personinterest.md) 对象中可以设置 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-129">The following table shows the properties that are possible to set within a new [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="3aa0f-130">属性</span><span class="sxs-lookup"><span data-stu-id="3aa0f-130">Property</span></span>|<span data-ttu-id="3aa0f-131">类型</span><span class="sxs-lookup"><span data-stu-id="3aa0f-131">Type</span></span>|<span data-ttu-id="3aa0f-132">说明</span><span class="sxs-lookup"><span data-stu-id="3aa0f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3aa0f-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="3aa0f-133">allowedAudiences</span></span>|<span data-ttu-id="3aa0f-134">String</span><span class="sxs-lookup"><span data-stu-id="3aa0f-134">String</span></span>|<span data-ttu-id="3aa0f-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="3aa0f-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="3aa0f-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3aa0f-138">categories</span><span class="sxs-lookup"><span data-stu-id="3aa0f-138">categories</span></span>|<span data-ttu-id="3aa0f-139">String 集合</span><span class="sxs-lookup"><span data-stu-id="3aa0f-139">String collection</span></span>|<span data-ttu-id="3aa0f-140">包含用户与兴趣类别关联的类别 (例如个人、) 。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-140">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="3aa0f-141">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="3aa0f-141">collaborationTags</span></span>|<span data-ttu-id="3aa0f-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="3aa0f-142">String collection</span></span>|<span data-ttu-id="3aa0f-143">包含用户与兴趣相关联的体验方案标记。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-143">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="3aa0f-144">集合中允许的值为 `askMeAbout` `ableToMentor` ：、、、。 `wantsToLearn` `wantsToImprove`</span><span class="sxs-lookup"><span data-stu-id="3aa0f-144">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="3aa0f-145">说明</span><span class="sxs-lookup"><span data-stu-id="3aa0f-145">description</span></span>|<span data-ttu-id="3aa0f-146">String</span><span class="sxs-lookup"><span data-stu-id="3aa0f-146">String</span></span>|<span data-ttu-id="3aa0f-147">包含感兴趣的说明。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-147">Contains a description of the interest.</span></span>|
|<span data-ttu-id="3aa0f-148">displayName</span><span class="sxs-lookup"><span data-stu-id="3aa0f-148">displayName</span></span>|<span data-ttu-id="3aa0f-149">String</span><span class="sxs-lookup"><span data-stu-id="3aa0f-149">String</span></span>|<span data-ttu-id="3aa0f-150">包含兴趣的友好名称。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-150">Contains a friendly name for the interest.</span></span>  |
|<span data-ttu-id="3aa0f-151">inference</span><span class="sxs-lookup"><span data-stu-id="3aa0f-151">inference</span></span>|[<span data-ttu-id="3aa0f-152">inferenceData</span><span class="sxs-lookup"><span data-stu-id="3aa0f-152">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="3aa0f-153">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-153">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="3aa0f-154">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="3aa0f-155">source</span><span class="sxs-lookup"><span data-stu-id="3aa0f-155">source</span></span>|[<span data-ttu-id="3aa0f-156">personDataSource</span><span class="sxs-lookup"><span data-stu-id="3aa0f-156">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="3aa0f-157">如果从另一个服务同步，则值源自何处。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-157">Where the values originated if synced from another service.</span></span> <span data-ttu-id="3aa0f-158">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-158">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="3aa0f-159">webUrl</span><span class="sxs-lookup"><span data-stu-id="3aa0f-159">webUrl</span></span>|<span data-ttu-id="3aa0f-160">String</span><span class="sxs-lookup"><span data-stu-id="3aa0f-160">String</span></span>|<span data-ttu-id="3aa0f-161">包含指向有关感兴趣的网页或资源的链接。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-161">Contains a link to a web page or resource about the interest.</span></span> |

## <a name="response"></a><span data-ttu-id="3aa0f-162">响应</span><span class="sxs-lookup"><span data-stu-id="3aa0f-162">Response</span></span>

<span data-ttu-id="3aa0f-163">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [personInterest](../resources/personinterest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-163">If successful, this method returns a `201 Created` response code and a new [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3aa0f-164">示例</span><span class="sxs-lookup"><span data-stu-id="3aa0f-164">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3aa0f-165">请求</span><span class="sxs-lookup"><span data-stu-id="3aa0f-165">Request</span></span>

<span data-ttu-id="3aa0f-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-166">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3aa0f-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="3aa0f-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personinterest_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/interests
Content-type: application/json

{
  "categories": [
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com"
}
```
# <a name="c"></a>[<span data-ttu-id="3aa0f-168">C#</span><span class="sxs-lookup"><span data-stu-id="3aa0f-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personinterest-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3aa0f-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3aa0f-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personinterest-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3aa0f-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3aa0f-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personinterest-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3aa0f-171">Java</span><span class="sxs-lookup"><span data-stu-id="3aa0f-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personinterest-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3aa0f-172">响应</span><span class="sxs-lookup"><span data-stu-id="3aa0f-172">Response</span></span>

<span data-ttu-id="3aa0f-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-173">The following is an example of the response.</span></span>

> <span data-ttu-id="3aa0f-174">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3aa0f-174">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
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
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com",
  "collaborationTags": null
}
```


