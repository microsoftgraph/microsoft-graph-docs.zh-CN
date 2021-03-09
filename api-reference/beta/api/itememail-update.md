---
title: 更新 itememail
description: 更新用户配置文件中的 itemEmail 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e37adabbb0fc9ce8e355d2ab6e8d6a302fe14918
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577497"
---
# <a name="update-itememail"></a><span data-ttu-id="d3a45-103">更新 itememail</span><span class="sxs-lookup"><span data-stu-id="d3a45-103">Update itememail</span></span>

<span data-ttu-id="d3a45-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3a45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3a45-105">更新用户配置文件 [中的 itemEmail](../resources/itememail.md) 对象 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="d3a45-105">Update the properties of an [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d3a45-106">权限</span><span class="sxs-lookup"><span data-stu-id="d3a45-106">Permissions</span></span>

<span data-ttu-id="d3a45-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3a45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3a45-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3a45-109">Permission type</span></span>                        | <span data-ttu-id="d3a45-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3a45-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d3a45-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3a45-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3a45-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3a45-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d3a45-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3a45-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3a45-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3a45-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d3a45-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3a45-115">Application</span></span>                            | <span data-ttu-id="d3a45-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3a45-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="d3a45-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3a45-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/emails/{id}
PATCH /users/{id | userPrincipalName}/profile/emails/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d3a45-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3a45-118">Request headers</span></span>
|<span data-ttu-id="d3a45-119">名称</span><span class="sxs-lookup"><span data-stu-id="d3a45-119">Name</span></span>|<span data-ttu-id="d3a45-120">说明</span><span class="sxs-lookup"><span data-stu-id="d3a45-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d3a45-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3a45-121">Authorization</span></span>|<span data-ttu-id="d3a45-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d3a45-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d3a45-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3a45-124">Content-Type</span></span>|<span data-ttu-id="d3a45-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d3a45-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3a45-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3a45-127">Request body</span></span>

<span data-ttu-id="d3a45-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="d3a45-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d3a45-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="d3a45-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d3a45-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d3a45-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="d3a45-131">下表显示了在用户配置文件中的现有 [itemEmail](../resources/itememail.md) 对象中可以更新 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="d3a45-131">The following table shows the properties that are possible to update within an existing [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="d3a45-132">属性</span><span class="sxs-lookup"><span data-stu-id="d3a45-132">Property</span></span>|<span data-ttu-id="d3a45-133">类型</span><span class="sxs-lookup"><span data-stu-id="d3a45-133">Type</span></span>|<span data-ttu-id="d3a45-134">说明</span><span class="sxs-lookup"><span data-stu-id="d3a45-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3a45-135">address</span><span class="sxs-lookup"><span data-stu-id="d3a45-135">address</span></span>|<span data-ttu-id="d3a45-136">String</span><span class="sxs-lookup"><span data-stu-id="d3a45-136">String</span></span>|<span data-ttu-id="d3a45-137">电子邮件地址本身。</span><span class="sxs-lookup"><span data-stu-id="d3a45-137">The email address itself.</span></span>|
|<span data-ttu-id="d3a45-138">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="d3a45-138">allowedAudiences</span></span>|<span data-ttu-id="d3a45-139">字符串</span><span class="sxs-lookup"><span data-stu-id="d3a45-139">String</span></span>|<span data-ttu-id="d3a45-140">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="d3a45-140">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="d3a45-141">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d3a45-141">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="d3a45-142">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d3a45-142">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d3a45-143">displayName</span><span class="sxs-lookup"><span data-stu-id="d3a45-143">displayName</span></span>|<span data-ttu-id="d3a45-144">字符串</span><span class="sxs-lookup"><span data-stu-id="d3a45-144">String</span></span>|<span data-ttu-id="d3a45-145">用户与特定电子邮件地址关联的名称或标签。</span><span class="sxs-lookup"><span data-stu-id="d3a45-145">The name or label a user has associated with a particular email address.</span></span>|
|<span data-ttu-id="d3a45-146">推断</span><span class="sxs-lookup"><span data-stu-id="d3a45-146">inference</span></span>|[<span data-ttu-id="d3a45-147">inferenceData</span><span class="sxs-lookup"><span data-stu-id="d3a45-147">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="d3a45-148">包含实体是否由创建或修改应用程序推断的推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="d3a45-148">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="d3a45-149">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d3a45-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d3a45-150">source</span><span class="sxs-lookup"><span data-stu-id="d3a45-150">source</span></span>|[<span data-ttu-id="d3a45-151">personDataSource</span><span class="sxs-lookup"><span data-stu-id="d3a45-151">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="d3a45-152">如果从另一个服务同步，则值源自何处。</span><span class="sxs-lookup"><span data-stu-id="d3a45-152">Where the values originated if synced from another service.</span></span> <span data-ttu-id="d3a45-153">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d3a45-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d3a45-154">type</span><span class="sxs-lookup"><span data-stu-id="d3a45-154">type</span></span>|<span data-ttu-id="d3a45-155">emailType</span><span class="sxs-lookup"><span data-stu-id="d3a45-155">emailType</span></span>|<span data-ttu-id="d3a45-156">电子邮件地址的类型。</span><span class="sxs-lookup"><span data-stu-id="d3a45-156">The type of email address.</span></span> <span data-ttu-id="d3a45-157">可取值为：`unknown`、`work`、`personal`、`main`、`other`。</span><span class="sxs-lookup"><span data-stu-id="d3a45-157">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="d3a45-158">响应</span><span class="sxs-lookup"><span data-stu-id="d3a45-158">Response</span></span>

<span data-ttu-id="d3a45-159">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [itemEmail](../resources/itememail.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d3a45-159">If successful, this method returns a `200 OK` response code and an updated [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3a45-160">示例</span><span class="sxs-lookup"><span data-stu-id="d3a45-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3a45-161">请求</span><span class="sxs-lookup"><span data-stu-id="d3a45-161">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="d3a45-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3a45-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itememail"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{userId}/profile/emails/{id}
Content-Type: application/json
Content-length: 383

{
  "displayName": "Business Email",
  "type": "work"
}
```
# <a name="c"></a>[<span data-ttu-id="d3a45-163">C#</span><span class="sxs-lookup"><span data-stu-id="d3a45-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3a45-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3a45-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3a45-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3a45-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d3a45-166">响应</span><span class="sxs-lookup"><span data-stu-id="d3a45-166">Response</span></span>
<span data-ttu-id="d3a45-167">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d3a45-167">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
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
  "address": "Innocenty.Popov@adventureworks.com",
  "displayName": "Business Email",
  "type": "work"
}
```


