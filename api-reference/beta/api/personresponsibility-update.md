---
title: 更新 personResponsibility
description: 更新 personResponsibility 对象的属性。
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 62948aa9accfa79997e9a119f32d200cca507051
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292698"
---
# <a name="update-personresponsibility"></a><span data-ttu-id="79ad4-103">更新 personResponsibility</span><span class="sxs-lookup"><span data-stu-id="79ad4-103">Update personResponsibility</span></span>
<span data-ttu-id="79ad4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79ad4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79ad4-105">更新用户配置文件 [中的 personResponsibility](../resources/personresponsibility.md) 对象 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="79ad4-105">Update the properties of a [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="79ad4-106">权限</span><span class="sxs-lookup"><span data-stu-id="79ad4-106">Permissions</span></span>

<span data-ttu-id="79ad4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79ad4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79ad4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="79ad4-109">Permission type</span></span>                        | <span data-ttu-id="79ad4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79ad4-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="79ad4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79ad4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="79ad4-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79ad4-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="79ad4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79ad4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79ad4-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79ad4-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="79ad4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="79ad4-115">Application</span></span>                            | <span data-ttu-id="79ad4-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79ad4-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="79ad4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79ad4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/responsibilities/{id}
PATCH /users/{id | userPrincipalName}/responsibilities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="79ad4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="79ad4-118">Request headers</span></span>
|<span data-ttu-id="79ad4-119">名称</span><span class="sxs-lookup"><span data-stu-id="79ad4-119">Name</span></span>|<span data-ttu-id="79ad4-120">说明</span><span class="sxs-lookup"><span data-stu-id="79ad4-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="79ad4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="79ad4-121">Authorization</span></span>|<span data-ttu-id="79ad4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79ad4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="79ad4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79ad4-124">Content-Type</span></span>|<span data-ttu-id="79ad4-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="79ad4-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79ad4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="79ad4-127">Request body</span></span>
<span data-ttu-id="79ad4-128">在请求正文中，提供 [personResponsibility](../resources/personresponsibility.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79ad4-128">In the request body, supply a JSON representation of the [personResponsibility](../resources/personresponsibility.md) object.</span></span>

<span data-ttu-id="79ad4-129">下表显示创建 [personResponsibility 时所需的属性](../resources/personresponsibility.md)。</span><span class="sxs-lookup"><span data-stu-id="79ad4-129">The following table shows the properties that are required when you create the [personResponsibility](../resources/personresponsibility.md).</span></span>

|<span data-ttu-id="79ad4-130">属性</span><span class="sxs-lookup"><span data-stu-id="79ad4-130">Property</span></span>|<span data-ttu-id="79ad4-131">类型</span><span class="sxs-lookup"><span data-stu-id="79ad4-131">Type</span></span>|<span data-ttu-id="79ad4-132">说明</span><span class="sxs-lookup"><span data-stu-id="79ad4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79ad4-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="79ad4-133">allowedAudiences</span></span>|<span data-ttu-id="79ad4-134">String</span><span class="sxs-lookup"><span data-stu-id="79ad4-134">String</span></span>|<span data-ttu-id="79ad4-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="79ad4-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="79ad4-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="79ad4-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="79ad4-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="79ad4-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="79ad4-138">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="79ad4-138">collaborationTags</span></span>|<span data-ttu-id="79ad4-139">String collection</span><span class="sxs-lookup"><span data-stu-id="79ad4-139">String collection</span></span>|<span data-ttu-id="79ad4-140">包含用户与兴趣相关联的体验方案标记。</span><span class="sxs-lookup"><span data-stu-id="79ad4-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="79ad4-141">集合中允许的值是： `askMeAbout` ， `ableToMentor` ， `wantsToLearn` `wantsToImprove` 。</span><span class="sxs-lookup"><span data-stu-id="79ad4-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="79ad4-142">description</span><span class="sxs-lookup"><span data-stu-id="79ad4-142">description</span></span>|<span data-ttu-id="79ad4-143">String</span><span class="sxs-lookup"><span data-stu-id="79ad4-143">String</span></span>|<span data-ttu-id="79ad4-144">责任说明。</span><span class="sxs-lookup"><span data-stu-id="79ad4-144">Description of the responsibility.</span></span>|
|<span data-ttu-id="79ad4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="79ad4-145">displayName</span></span>|<span data-ttu-id="79ad4-146">String</span><span class="sxs-lookup"><span data-stu-id="79ad4-146">String</span></span>|<span data-ttu-id="79ad4-147">包含责任的友好名称。</span><span class="sxs-lookup"><span data-stu-id="79ad4-147">Contains a friendly name for the responsibility.</span></span> |
|<span data-ttu-id="79ad4-148">推断</span><span class="sxs-lookup"><span data-stu-id="79ad4-148">inference</span></span>|[<span data-ttu-id="79ad4-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="79ad4-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="79ad4-150">如果实体是由创建或修改应用程序推断的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="79ad4-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="79ad4-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="79ad4-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="79ad4-152">WebUrl</span><span class="sxs-lookup"><span data-stu-id="79ad4-152">webUrl</span></span>|<span data-ttu-id="79ad4-153">String</span><span class="sxs-lookup"><span data-stu-id="79ad4-153">String</span></span>|<span data-ttu-id="79ad4-154">包含指向有关该责任的网页或资源的链接。</span><span class="sxs-lookup"><span data-stu-id="79ad4-154">Contains a link to a web page or resource about the responsibility.</span></span>|



## <a name="response"></a><span data-ttu-id="79ad4-155">响应</span><span class="sxs-lookup"><span data-stu-id="79ad4-155">Response</span></span>

<span data-ttu-id="79ad4-156">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [personResponsibility](../resources/personresponsibility.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79ad4-156">If successful, this method returns a `200 OK` response code and an updated [personResponsibility](../resources/personresponsibility.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79ad4-157">示例</span><span class="sxs-lookup"><span data-stu-id="79ad4-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="79ad4-158">请求</span><span class="sxs-lookup"><span data-stu-id="79ad4-158">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "update_personresponsibility"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
Content-Type: application/json
Content-length: 446

{
  "collaborationTags": [
    "askMeAbout"
  ]
}
```

### <a name="response"></a><span data-ttu-id="79ad4-159">响应</span><span class="sxs-lookup"><span data-stu-id="79ad4-159">Response</span></span>
<span data-ttu-id="79ad4-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="79ad4-160">**Note:** The response object shown here might be shortened for readability.</span></span>
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


