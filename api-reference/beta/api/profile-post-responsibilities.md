---
title: 创建责任
description: 创建新的责任对象。
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 086bc8af800c70a9282a04606f82818a135d65de
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440955"
---
# <a name="create-personresponsibility"></a><span data-ttu-id="5c5bf-103">创建 personResponsibility</span><span class="sxs-lookup"><span data-stu-id="5c5bf-103">Create personResponsibility</span></span>
<span data-ttu-id="5c5bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c5bf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5c5bf-105">在用户配置文件中创建新的 [personResponsibility](../resources/personresponsibility.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-105">Create a new [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5c5bf-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="5c5bf-106">Permissions</span></span>

<span data-ttu-id="5c5bf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c5bf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c5bf-109">Permission type</span></span>                        | <span data-ttu-id="5c5bf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c5bf-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="5c5bf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c5bf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c5bf-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5bf-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5c5bf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c5bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c5bf-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5bf-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5c5bf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c5bf-115">Application</span></span>                            | <span data-ttu-id="5c5bf-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5bf-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="5c5bf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c5bf-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/responsibilities
POST /users/{id | userPrincipalName}/responsibilities
```

## <a name="request-headers"></a><span data-ttu-id="5c5bf-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c5bf-118">Request headers</span></span>
|<span data-ttu-id="5c5bf-119">名称</span><span class="sxs-lookup"><span data-stu-id="5c5bf-119">Name</span></span>|<span data-ttu-id="5c5bf-120">说明</span><span class="sxs-lookup"><span data-stu-id="5c5bf-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5c5bf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c5bf-121">Authorization</span></span>|<span data-ttu-id="5c5bf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5c5bf-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c5bf-124">Content-Type</span></span>|<span data-ttu-id="5c5bf-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5c5bf-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c5bf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c5bf-127">Request body</span></span>
<span data-ttu-id="5c5bf-128">在请求正文中，提供 [personResponsibility](../resources/personresponsibility.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-128">In the request body, supply a JSON representation of the [personResponsibility](../resources/personresponsibility.md) object.</span></span>

<span data-ttu-id="5c5bf-129">下表显示了在用户配置文件中的新 [personResponsibility](../resources/personresponsibility.md) 对象中可以设置 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-129">The following table shows the properties that are possible to set within a new [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="5c5bf-130">属性</span><span class="sxs-lookup"><span data-stu-id="5c5bf-130">Property</span></span>|<span data-ttu-id="5c5bf-131">类型</span><span class="sxs-lookup"><span data-stu-id="5c5bf-131">Type</span></span>|<span data-ttu-id="5c5bf-132">说明</span><span class="sxs-lookup"><span data-stu-id="5c5bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c5bf-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="5c5bf-133">allowedAudiences</span></span>|<span data-ttu-id="5c5bf-134">String</span><span class="sxs-lookup"><span data-stu-id="5c5bf-134">String</span></span>|<span data-ttu-id="5c5bf-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="5c5bf-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="5c5bf-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5c5bf-138">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="5c5bf-138">collaborationTags</span></span>|<span data-ttu-id="5c5bf-139">字符串集合</span><span class="sxs-lookup"><span data-stu-id="5c5bf-139">String collection</span></span>|<span data-ttu-id="5c5bf-140">包含用户与兴趣相关联的体验方案标记。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="5c5bf-141">集合中允许的值是： `askMeAbout` ， `ableToMentor` ， `wantsToLearn` `wantsToImprove` 。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="5c5bf-142">说明</span><span class="sxs-lookup"><span data-stu-id="5c5bf-142">description</span></span>|<span data-ttu-id="5c5bf-143">String</span><span class="sxs-lookup"><span data-stu-id="5c5bf-143">String</span></span>|<span data-ttu-id="5c5bf-144">责任说明。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-144">Description of the responsibility.</span></span>|
|<span data-ttu-id="5c5bf-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5c5bf-145">displayName</span></span>|<span data-ttu-id="5c5bf-146">String</span><span class="sxs-lookup"><span data-stu-id="5c5bf-146">String</span></span>|<span data-ttu-id="5c5bf-147">包含责任的友好名称。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-147">Contains a friendly name for the responsibility.</span></span> |
|<span data-ttu-id="5c5bf-148">推断</span><span class="sxs-lookup"><span data-stu-id="5c5bf-148">inference</span></span>|[<span data-ttu-id="5c5bf-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="5c5bf-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="5c5bf-150">包含实体是否由创建或修改应用程序推断的推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="5c5bf-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5c5bf-152">source</span><span class="sxs-lookup"><span data-stu-id="5c5bf-152">source</span></span>|[<span data-ttu-id="5c5bf-153">personDataSource</span><span class="sxs-lookup"><span data-stu-id="5c5bf-153">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="5c5bf-154">如果从另一个服务同步，则值源自何处。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-154">Where the values originated if synced from another service.</span></span> <span data-ttu-id="5c5bf-155">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-155">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="5c5bf-156">WebUrl</span><span class="sxs-lookup"><span data-stu-id="5c5bf-156">webUrl</span></span>|<span data-ttu-id="5c5bf-157">String</span><span class="sxs-lookup"><span data-stu-id="5c5bf-157">String</span></span>|<span data-ttu-id="5c5bf-158">包含指向有关该责任的网页或资源的链接。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-158">Contains a link to a web page or resource about the responsibility.</span></span>|

## <a name="response"></a><span data-ttu-id="5c5bf-159">响应</span><span class="sxs-lookup"><span data-stu-id="5c5bf-159">Response</span></span>

<span data-ttu-id="5c5bf-160">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [personResponsibility](../resources/personannotation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-160">If successful, this method returns a `201 Created` response code and a [personResponsibility](../resources/personannotation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c5bf-161">示例</span><span class="sxs-lookup"><span data-stu-id="5c5bf-161">Examples</span></span>


# <a name="http"></a>[<span data-ttu-id="5c5bf-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c5bf-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personresponsibility_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/responsibilities
Content-Type: application/json
Content-length: 413

{
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "collaborationTags": [
    "askMeAbout"
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="5c5bf-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c5bf-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personresponsibility-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c5bf-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c5bf-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personresponsibility-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5c5bf-165">响应</span><span class="sxs-lookup"><span data-stu-id="5c5bf-165">Response</span></span>
<span data-ttu-id="5c5bf-166">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5c5bf-166">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personResponsibility"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

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
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "webUrl": null,
  "collaborationTags": [
    "askMeAbout"
  ]
}
```


