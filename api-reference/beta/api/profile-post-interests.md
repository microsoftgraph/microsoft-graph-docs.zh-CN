---
title: 创建 personInterest
description: 创建新的 personInterest。
localization_priority: Normal
author: kevinbellinger
ms.prod: People
doc_type: apiPageType
ms.openlocfilehash: 156e9f6cef6c0b0f6e9def42fc4d2417706e426b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975371"
---
# <a name="create-personinterest"></a><span data-ttu-id="961db-103">创建 personInterest</span><span class="sxs-lookup"><span data-stu-id="961db-103">Create personInterest</span></span>

<span data-ttu-id="961db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="961db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="961db-105">创建新的 [personInterest] ( .。。/resources/personinterest.md] 在用户的 [配置文件](../resources/profile.md)中。</span><span class="sxs-lookup"><span data-stu-id="961db-105">Create a new [personInterest](../resources/personinterest.md] in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="961db-106">权限</span><span class="sxs-lookup"><span data-stu-id="961db-106">Permissions</span></span>

<span data-ttu-id="961db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="961db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="961db-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="961db-109">Permission type</span></span>                        | <span data-ttu-id="961db-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="961db-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="961db-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="961db-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="961db-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="961db-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="961db-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="961db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="961db-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="961db-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="961db-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="961db-115">Application</span></span>                            | <span data-ttu-id="961db-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="961db-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="961db-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="961db-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/interests
POST /users/{id | userPrincipalName}/profile/interests
```

## <a name="request-headers"></a><span data-ttu-id="961db-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="961db-118">Request headers</span></span>

| <span data-ttu-id="961db-119">名称</span><span class="sxs-lookup"><span data-stu-id="961db-119">Name</span></span>      |<span data-ttu-id="961db-120">说明</span><span class="sxs-lookup"><span data-stu-id="961db-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="961db-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="961db-121">Authorization</span></span>  | <span data-ttu-id="961db-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="961db-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="961db-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="961db-124">Content-Type</span></span>   | <span data-ttu-id="961db-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="961db-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="961db-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="961db-127">Request body</span></span>

<span data-ttu-id="961db-128">在请求正文中，提供 [personInterest](../resources/personinterest.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="961db-128">In the request body, supply a JSON representation of the [personInterest](../resources/personinterest.md) object.</span></span>

<span data-ttu-id="961db-129">下表显示了可以在用户[配置文件](../resources/profile.md)中的新[personInterest](../resources/personinterest.md)对象内设置的属性。</span><span class="sxs-lookup"><span data-stu-id="961db-129">The following table shows the properties that are possible to set within a new [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="961db-130">属性</span><span class="sxs-lookup"><span data-stu-id="961db-130">Property</span></span>|<span data-ttu-id="961db-131">类型</span><span class="sxs-lookup"><span data-stu-id="961db-131">Type</span></span>|<span data-ttu-id="961db-132">说明</span><span class="sxs-lookup"><span data-stu-id="961db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="961db-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="961db-133">allowedAudiences</span></span>|<span data-ttu-id="961db-134">String</span><span class="sxs-lookup"><span data-stu-id="961db-134">String</span></span>|<span data-ttu-id="961db-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="961db-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="961db-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="961db-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="961db-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="961db-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="961db-138">categories</span><span class="sxs-lookup"><span data-stu-id="961db-138">categories</span></span>|<span data-ttu-id="961db-139">String collection</span><span class="sxs-lookup"><span data-stu-id="961db-139">String collection</span></span>|<span data-ttu-id="961db-140">包含用户与兴趣相关联的类别 (例如，个人 recipies) 。</span><span class="sxs-lookup"><span data-stu-id="961db-140">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="961db-141">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="961db-141">collaborationTags</span></span>|<span data-ttu-id="961db-142">String collection</span><span class="sxs-lookup"><span data-stu-id="961db-142">String collection</span></span>|<span data-ttu-id="961db-143">包含用户与兴趣相关的体验方案标记。</span><span class="sxs-lookup"><span data-stu-id="961db-143">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="961db-144">集合中允许的值为： `askMeAbout` 、 `ableToMentor` 、 `wantsToLearn` 、 `wantsToImprove` 。</span><span class="sxs-lookup"><span data-stu-id="961db-144">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="961db-145">说明</span><span class="sxs-lookup"><span data-stu-id="961db-145">description</span></span>|<span data-ttu-id="961db-146">String</span><span class="sxs-lookup"><span data-stu-id="961db-146">String</span></span>|<span data-ttu-id="961db-147">包含对利息的说明。</span><span class="sxs-lookup"><span data-stu-id="961db-147">Contains a description of the interest.</span></span>|
|<span data-ttu-id="961db-148">displayName</span><span class="sxs-lookup"><span data-stu-id="961db-148">displayName</span></span>|<span data-ttu-id="961db-149">String</span><span class="sxs-lookup"><span data-stu-id="961db-149">String</span></span>|<span data-ttu-id="961db-150">包含利息的友好名称。</span><span class="sxs-lookup"><span data-stu-id="961db-150">Contains a friendly name for the interest.</span></span>  |
|<span data-ttu-id="961db-151">推导</span><span class="sxs-lookup"><span data-stu-id="961db-151">inference</span></span>|[<span data-ttu-id="961db-152">inferenceData</span><span class="sxs-lookup"><span data-stu-id="961db-152">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="961db-153">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="961db-153">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="961db-154">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="961db-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="961db-155">source</span><span class="sxs-lookup"><span data-stu-id="961db-155">source</span></span>|[<span data-ttu-id="961db-156">personDataSource</span><span class="sxs-lookup"><span data-stu-id="961db-156">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="961db-157">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="961db-157">Where the values originated if synced from another service.</span></span> <span data-ttu-id="961db-158">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="961db-158">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="961db-159">webUrl</span><span class="sxs-lookup"><span data-stu-id="961db-159">webUrl</span></span>|<span data-ttu-id="961db-160">String</span><span class="sxs-lookup"><span data-stu-id="961db-160">String</span></span>|<span data-ttu-id="961db-161">包含指向有关该兴趣的网页或资源的链接。</span><span class="sxs-lookup"><span data-stu-id="961db-161">Contains a link to a web page or resource about the interest.</span></span> |

## <a name="response"></a><span data-ttu-id="961db-162">响应</span><span class="sxs-lookup"><span data-stu-id="961db-162">Response</span></span>

<span data-ttu-id="961db-163">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的 [personInterest](../resources/personinterest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="961db-163">If successful, this method returns a `201 Created` response code and a new [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="961db-164">示例</span><span class="sxs-lookup"><span data-stu-id="961db-164">Examples</span></span>

### <a name="request"></a><span data-ttu-id="961db-165">请求</span><span class="sxs-lookup"><span data-stu-id="961db-165">Request</span></span>

<span data-ttu-id="961db-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="961db-166">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="961db-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="961db-167">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="961db-168">C#</span><span class="sxs-lookup"><span data-stu-id="961db-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personinterest-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="961db-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="961db-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personinterest-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="961db-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="961db-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personinterest-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="961db-171">Java</span><span class="sxs-lookup"><span data-stu-id="961db-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personinterest-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="961db-172">响应</span><span class="sxs-lookup"><span data-stu-id="961db-172">Response</span></span>

<span data-ttu-id="961db-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="961db-173">The following is an example of the response.</span></span>

> <span data-ttu-id="961db-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="961db-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


