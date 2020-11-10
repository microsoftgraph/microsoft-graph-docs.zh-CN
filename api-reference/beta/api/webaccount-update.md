---
title: 更新 webAccount
description: 更新 webAccount 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6df75e05761d47e513272a222e956ee64235bde3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973949"
---
# <a name="update-webaccount"></a><span data-ttu-id="d6ccb-103">更新 webAccount</span><span class="sxs-lookup"><span data-stu-id="d6ccb-103">Update webAccount</span></span>

<span data-ttu-id="d6ccb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6ccb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6ccb-105">更新用户的[配置文件](../resources/profile.md)中的[webAccount](../resources/webaccount.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-105">Update the properties of a [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d6ccb-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6ccb-106">Permissions</span></span>

<span data-ttu-id="d6ccb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d6ccb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6ccb-109">Permission type</span></span>                        | <span data-ttu-id="d6ccb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6ccb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d6ccb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6ccb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6ccb-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d6ccb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6ccb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6ccb-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d6ccb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6ccb-115">Application</span></span>                            | <span data-ttu-id="d6ccb-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6ccb-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="d6ccb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6ccb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/webAccounts/{id}
PATCH /users/{id | userPrincipalName}/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d6ccb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6ccb-118">Request headers</span></span>

| <span data-ttu-id="d6ccb-119">名称</span><span class="sxs-lookup"><span data-stu-id="d6ccb-119">Name</span></span>           |<span data-ttu-id="d6ccb-120">说明</span><span class="sxs-lookup"><span data-stu-id="d6ccb-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="d6ccb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6ccb-121">Authorization</span></span>  | <span data-ttu-id="d6ccb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d6ccb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6ccb-124">Content-Type</span></span>   | <span data-ttu-id="d6ccb-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d6ccb-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d6ccb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6ccb-127">Request body</span></span>

<span data-ttu-id="d6ccb-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d6ccb-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d6ccb-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="d6ccb-131">属性</span><span class="sxs-lookup"><span data-stu-id="d6ccb-131">Property</span></span>|<span data-ttu-id="d6ccb-132">类型</span><span class="sxs-lookup"><span data-stu-id="d6ccb-132">Type</span></span>|<span data-ttu-id="d6ccb-133">说明</span><span class="sxs-lookup"><span data-stu-id="d6ccb-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6ccb-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="d6ccb-134">allowedAudiences</span></span>|<span data-ttu-id="d6ccb-135">String</span><span class="sxs-lookup"><span data-stu-id="d6ccb-135">String</span></span>|<span data-ttu-id="d6ccb-136">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="d6ccb-137">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="d6ccb-138">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d6ccb-139">说明</span><span class="sxs-lookup"><span data-stu-id="d6ccb-139">description</span></span>|<span data-ttu-id="d6ccb-140">String</span><span class="sxs-lookup"><span data-stu-id="d6ccb-140">String</span></span>|<span data-ttu-id="d6ccb-141">包含用户为所引用服务上的帐户提供的说明。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-141">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="d6ccb-142">推导</span><span class="sxs-lookup"><span data-stu-id="d6ccb-142">inference</span></span>|[<span data-ttu-id="d6ccb-143">inferenceData</span><span class="sxs-lookup"><span data-stu-id="d6ccb-143">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="d6ccb-144">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-144">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="d6ccb-145">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d6ccb-146">服务</span><span class="sxs-lookup"><span data-stu-id="d6ccb-146">service</span></span>|[<span data-ttu-id="d6ccb-147">serviceInformation</span><span class="sxs-lookup"><span data-stu-id="d6ccb-147">serviceInformation</span></span>](../resources/serviceinformation.md)| <span data-ttu-id="d6ccb-148">包含有关要关联的服务的基本详细信息。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-148">Contains basic detail about the service that is being associated.</span></span> |
|<span data-ttu-id="d6ccb-149">statusMessage</span><span class="sxs-lookup"><span data-stu-id="d6ccb-149">statusMessage</span></span>|<span data-ttu-id="d6ccb-150">String</span><span class="sxs-lookup"><span data-stu-id="d6ccb-150">String</span></span>|<span data-ttu-id="d6ccb-151">包含来自云服务的状态邮件（如果提供或已同步）。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-151">Contains a status message from the cloud service if provided or synchronized.</span></span> |
|<span data-ttu-id="d6ccb-152">userId</span><span class="sxs-lookup"><span data-stu-id="d6ccb-152">userId</span></span>|<span data-ttu-id="d6ccb-153">String</span><span class="sxs-lookup"><span data-stu-id="d6ccb-153">String</span></span>|<span data-ttu-id="d6ccb-154">为 webaccount 显示的用户名。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-154">The user name  displayed for the webaccount.</span></span>  |
|<span data-ttu-id="d6ccb-155">webUrl</span><span class="sxs-lookup"><span data-stu-id="d6ccb-155">webUrl</span></span>|<span data-ttu-id="d6ccb-156">String</span><span class="sxs-lookup"><span data-stu-id="d6ccb-156">String</span></span>|<span data-ttu-id="d6ccb-157">包含指向云服务上的用户配置文件的链接（如果存在）。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-157">Contains a link to the user's profile on the cloud service if one exists.</span></span>|

## <a name="response"></a><span data-ttu-id="d6ccb-158">响应</span><span class="sxs-lookup"><span data-stu-id="d6ccb-158">Response</span></span>

<span data-ttu-id="d6ccb-159">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [webAccount](../resources/webaccount.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-159">If successful, this method returns a `200 OK` response code and an updated [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6ccb-160">示例</span><span class="sxs-lookup"><span data-stu-id="d6ccb-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6ccb-161">请求</span><span class="sxs-lookup"><span data-stu-id="d6ccb-161">Request</span></span>

<span data-ttu-id="d6ccb-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-162">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d6ccb-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6ccb-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_webaccount"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/webAccounts/{id}
Content-type: application/json

{
  "webUrl": "https://github.com/innocenty.popov"
}
```
# <a name="c"></a>[<span data-ttu-id="d6ccb-164">C#</span><span class="sxs-lookup"><span data-stu-id="d6ccb-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6ccb-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6ccb-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6ccb-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6ccb-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6ccb-167">Java</span><span class="sxs-lookup"><span data-stu-id="d6ccb-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-webaccount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d6ccb-168">响应</span><span class="sxs-lookup"><span data-stu-id="d6ccb-168">Response</span></span>

<span data-ttu-id="d6ccb-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-169">The following is an example of the response.</span></span>

> <span data-ttu-id="d6ccb-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d6ccb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
} -->

```http
HTTP/1.1 200 OK
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


