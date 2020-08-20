---
title: 创建 itemEmail
description: 新建 itemEmail。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 3577a0daa807c7f5016ae34b22174ffd1c2fe813
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819526"
---
# <a name="create-itememail"></a><span data-ttu-id="44b1b-103">创建 itemEmail</span><span class="sxs-lookup"><span data-stu-id="44b1b-103">Create itemEmail</span></span>

<span data-ttu-id="44b1b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44b1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44b1b-105">在用户配置文件 [中新建 itemEmail](../resources/itememail.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="44b1b-105">Create a new [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="44b1b-106">权限</span><span class="sxs-lookup"><span data-stu-id="44b1b-106">Permissions</span></span>

<span data-ttu-id="44b1b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44b1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44b1b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="44b1b-109">Permission type</span></span>                        | <span data-ttu-id="44b1b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44b1b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="44b1b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44b1b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="44b1b-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44b1b-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="44b1b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44b1b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44b1b-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44b1b-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="44b1b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="44b1b-115">Application</span></span>                            | <span data-ttu-id="44b1b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44b1b-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="44b1b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44b1b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/emails
POST /users/{id | userPrincipalName}/profile/emails
```

## <a name="request-headers"></a><span data-ttu-id="44b1b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="44b1b-118">Request headers</span></span>
|<span data-ttu-id="44b1b-119">名称</span><span class="sxs-lookup"><span data-stu-id="44b1b-119">Name</span></span>|<span data-ttu-id="44b1b-120">说明</span><span class="sxs-lookup"><span data-stu-id="44b1b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="44b1b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="44b1b-121">Authorization</span></span>|<span data-ttu-id="44b1b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="44b1b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="44b1b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="44b1b-124">Content-Type</span></span>|<span data-ttu-id="44b1b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="44b1b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44b1b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="44b1b-127">Request body</span></span>
<span data-ttu-id="44b1b-128">在请求正文中，提供 [itemEmail](../resources/itememail.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44b1b-128">In the request body, supply a JSON representation of the [itemEmail](../resources/itememail.md) object.</span></span>

<span data-ttu-id="44b1b-129">下表显示了在用户的配置文件中创建新 [itemEmail](../resources/itememail.md) 对象时可能设置 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="44b1b-129">The following table shows the properties that are possible to set when creating a new [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="44b1b-130">属性</span><span class="sxs-lookup"><span data-stu-id="44b1b-130">Property</span></span>|<span data-ttu-id="44b1b-131">类型</span><span class="sxs-lookup"><span data-stu-id="44b1b-131">Type</span></span>|<span data-ttu-id="44b1b-132">说明</span><span class="sxs-lookup"><span data-stu-id="44b1b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44b1b-133">address</span><span class="sxs-lookup"><span data-stu-id="44b1b-133">address</span></span>|<span data-ttu-id="44b1b-134">String</span><span class="sxs-lookup"><span data-stu-id="44b1b-134">String</span></span>|<span data-ttu-id="44b1b-135">电子邮件地址本身。</span><span class="sxs-lookup"><span data-stu-id="44b1b-135">The email address itself.</span></span>|
|<span data-ttu-id="44b1b-136">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="44b1b-136">allowedAudiences</span></span>|<span data-ttu-id="44b1b-137">String</span><span class="sxs-lookup"><span data-stu-id="44b1b-137">String</span></span>|<span data-ttu-id="44b1b-138">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="44b1b-138">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="44b1b-139">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="44b1b-139">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="44b1b-140">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="44b1b-140">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="44b1b-141">displayName</span><span class="sxs-lookup"><span data-stu-id="44b1b-141">displayName</span></span>|<span data-ttu-id="44b1b-142">String</span><span class="sxs-lookup"><span data-stu-id="44b1b-142">String</span></span>|<span data-ttu-id="44b1b-143">用户与特定电子邮件地址关联的名称或标签。</span><span class="sxs-lookup"><span data-stu-id="44b1b-143">The name or label a user has associated with a particular email address.</span></span>|
|<span data-ttu-id="44b1b-144">推据</span><span class="sxs-lookup"><span data-stu-id="44b1b-144">inference</span></span>|[<span data-ttu-id="44b1b-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="44b1b-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="44b1b-146">如果实体受到创建或修改的应用程序的推理，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="44b1b-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="44b1b-147">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="44b1b-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="44b1b-148">source</span><span class="sxs-lookup"><span data-stu-id="44b1b-148">source</span></span>|[<span data-ttu-id="44b1b-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="44b1b-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="44b1b-150">同步到其他服务时从哪个位置发送值。</span><span class="sxs-lookup"><span data-stu-id="44b1b-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="44b1b-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="44b1b-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="44b1b-152">type</span><span class="sxs-lookup"><span data-stu-id="44b1b-152">type</span></span>|<span data-ttu-id="44b1b-153">emailType</span><span class="sxs-lookup"><span data-stu-id="44b1b-153">emailType</span></span>|<span data-ttu-id="44b1b-154">电子邮件地址的类型。</span><span class="sxs-lookup"><span data-stu-id="44b1b-154">The type of email address.</span></span> <span data-ttu-id="44b1b-155">可取值为：`unknown`、`work`、`personal`、`main`、`other`。</span><span class="sxs-lookup"><span data-stu-id="44b1b-155">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>|



## <a name="response"></a><span data-ttu-id="44b1b-156">响应</span><span class="sxs-lookup"><span data-stu-id="44b1b-156">Response</span></span>

<span data-ttu-id="44b1b-157">如果成功，此方法在响应 `201 Created` 正文中返回响应代码和 [itemEmail](../resources/itememail.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="44b1b-157">If successful, this method returns a `201 Created` response code and an [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="44b1b-158">示例</span><span class="sxs-lookup"><span data-stu-id="44b1b-158">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="44b1b-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="44b1b-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itememail_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/emails
Content-Type: application/json
Content-length: 383

{
  "address": "Innocenty.Popov@adventureworks.com",
}
```
# <a name="c"></a>[<span data-ttu-id="44b1b-160">C#</span><span class="sxs-lookup"><span data-stu-id="44b1b-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itememail-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44b1b-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44b1b-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itememail-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44b1b-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44b1b-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itememail-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="44b1b-163">响应</span><span class="sxs-lookup"><span data-stu-id="44b1b-163">Response</span></span>
<span data-ttu-id="44b1b-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="44b1b-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
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
  "address": "Innocenty.Popov@adventureworks.com",
  "displayName": null,
  "type": null
}
```
