---
title: 更新 personResponsibility
description: 更新 personResponsibility 对象的属性。
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 38ca672825c49f0149dcf9b06b4c57d8df92c0e5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017365"
---
# <a name="update-personresponsibility"></a><span data-ttu-id="65b7c-103">更新 personResponsibility</span><span class="sxs-lookup"><span data-stu-id="65b7c-103">Update personResponsibility</span></span>
<span data-ttu-id="65b7c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65b7c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65b7c-105">更新用户的[配置文件](../resources/profile.md)中的[personResponsibility](../resources/personresponsibility.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="65b7c-105">Update the properties of a [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="65b7c-106">权限</span><span class="sxs-lookup"><span data-stu-id="65b7c-106">Permissions</span></span>

<span data-ttu-id="65b7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65b7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65b7c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="65b7c-109">Permission type</span></span>                        | <span data-ttu-id="65b7c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65b7c-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="65b7c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65b7c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="65b7c-112">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="65b7c-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="65b7c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65b7c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65b7c-114">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="65b7c-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="65b7c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="65b7c-115">Application</span></span>                            | <span data-ttu-id="65b7c-116">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="65b7c-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="65b7c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65b7c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/responsibilities/{id}
PATCH /users/{id | userPrincipalName}/profile/responsibilities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="65b7c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="65b7c-118">Request headers</span></span>
|<span data-ttu-id="65b7c-119">名称</span><span class="sxs-lookup"><span data-stu-id="65b7c-119">Name</span></span>|<span data-ttu-id="65b7c-120">说明</span><span class="sxs-lookup"><span data-stu-id="65b7c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="65b7c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="65b7c-121">Authorization</span></span>|<span data-ttu-id="65b7c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65b7c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="65b7c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65b7c-124">Content-Type</span></span>|<span data-ttu-id="65b7c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="65b7c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65b7c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="65b7c-127">Request body</span></span>
<span data-ttu-id="65b7c-128">在请求正文中，提供 [personResponsibility](../resources/personresponsibility.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65b7c-128">In the request body, supply a JSON representation of the [personResponsibility](../resources/personresponsibility.md) object.</span></span>

<span data-ttu-id="65b7c-129">下表显示创建 [personResponsibility](../resources/personresponsibility.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="65b7c-129">The following table shows the properties that are required when you create the [personResponsibility](../resources/personresponsibility.md).</span></span>

|<span data-ttu-id="65b7c-130">属性</span><span class="sxs-lookup"><span data-stu-id="65b7c-130">Property</span></span>|<span data-ttu-id="65b7c-131">类型</span><span class="sxs-lookup"><span data-stu-id="65b7c-131">Type</span></span>|<span data-ttu-id="65b7c-132">说明</span><span class="sxs-lookup"><span data-stu-id="65b7c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65b7c-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="65b7c-133">allowedAudiences</span></span>|<span data-ttu-id="65b7c-134">String</span><span class="sxs-lookup"><span data-stu-id="65b7c-134">String</span></span>|<span data-ttu-id="65b7c-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="65b7c-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="65b7c-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="65b7c-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="65b7c-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="65b7c-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="65b7c-138">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="65b7c-138">collaborationTags</span></span>|<span data-ttu-id="65b7c-139">String 集合</span><span class="sxs-lookup"><span data-stu-id="65b7c-139">String collection</span></span>|<span data-ttu-id="65b7c-140">包含用户与兴趣相关的体验方案标记。</span><span class="sxs-lookup"><span data-stu-id="65b7c-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="65b7c-141">集合中允许的值为： `askMeAbout` 、 `ableToMentor` 、 `wantsToLearn` 、 `wantsToImprove` 。</span><span class="sxs-lookup"><span data-stu-id="65b7c-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="65b7c-142">description</span><span class="sxs-lookup"><span data-stu-id="65b7c-142">description</span></span>|<span data-ttu-id="65b7c-143">String</span><span class="sxs-lookup"><span data-stu-id="65b7c-143">String</span></span>|<span data-ttu-id="65b7c-144">责任的说明。</span><span class="sxs-lookup"><span data-stu-id="65b7c-144">Description of the responsibility.</span></span>|
|<span data-ttu-id="65b7c-145">displayName</span><span class="sxs-lookup"><span data-stu-id="65b7c-145">displayName</span></span>|<span data-ttu-id="65b7c-146">String</span><span class="sxs-lookup"><span data-stu-id="65b7c-146">String</span></span>|<span data-ttu-id="65b7c-147">包含责任的友好名称。</span><span class="sxs-lookup"><span data-stu-id="65b7c-147">Contains a friendly name for the responsibility.</span></span> |
|<span data-ttu-id="65b7c-148">推导</span><span class="sxs-lookup"><span data-stu-id="65b7c-148">inference</span></span>|[<span data-ttu-id="65b7c-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="65b7c-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="65b7c-150">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="65b7c-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="65b7c-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="65b7c-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="65b7c-152">WebUrl</span><span class="sxs-lookup"><span data-stu-id="65b7c-152">webUrl</span></span>|<span data-ttu-id="65b7c-153">String</span><span class="sxs-lookup"><span data-stu-id="65b7c-153">String</span></span>|<span data-ttu-id="65b7c-154">包含指向有关责任的网页或资源的链接。</span><span class="sxs-lookup"><span data-stu-id="65b7c-154">Contains a link to a web page or resource about the responsibility.</span></span>|



## <a name="response"></a><span data-ttu-id="65b7c-155">响应</span><span class="sxs-lookup"><span data-stu-id="65b7c-155">Response</span></span>

<span data-ttu-id="65b7c-156">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [personResponsibility](../resources/personresponsibility.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65b7c-156">If successful, this method returns a `200 OK` response code and an updated [personResponsibility](../resources/personresponsibility.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65b7c-157">示例</span><span class="sxs-lookup"><span data-stu-id="65b7c-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65b7c-158">请求</span><span class="sxs-lookup"><span data-stu-id="65b7c-158">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="65b7c-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="65b7c-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "update_personresponsibility"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/profile/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
Content-Type: application/json
Content-length: 446

{
  "collaborationTags": [
    "askMeAbout"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="65b7c-160">C#</span><span class="sxs-lookup"><span data-stu-id="65b7c-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65b7c-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65b7c-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65b7c-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65b7c-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="65b7c-163">响应</span><span class="sxs-lookup"><span data-stu-id="65b7c-163">Response</span></span>
<span data-ttu-id="65b7c-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="65b7c-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personResponsibility"
}
-->
``` http
HTTP/1.1 200 OK
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


