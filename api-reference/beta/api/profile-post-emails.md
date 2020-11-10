---
title: 创建 itemEmail
description: 创建新的 itemEmail。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9da1d19a99182e7b242e162ae67b933db74cd995
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969673"
---
# <a name="create-itememail"></a><span data-ttu-id="e391e-103">创建 itemEmail</span><span class="sxs-lookup"><span data-stu-id="e391e-103">Create itemEmail</span></span>

<span data-ttu-id="e391e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e391e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e391e-105">在用户的[配置文件](../resources/profile.md)中创建新的[itemEmail](../resources/itememail.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e391e-105">Create a new [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e391e-106">权限</span><span class="sxs-lookup"><span data-stu-id="e391e-106">Permissions</span></span>

<span data-ttu-id="e391e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e391e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e391e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e391e-109">Permission type</span></span>                        | <span data-ttu-id="e391e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e391e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e391e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e391e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e391e-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="e391e-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e391e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e391e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e391e-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="e391e-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e391e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e391e-115">Application</span></span>                            | <span data-ttu-id="e391e-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e391e-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e391e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e391e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/emails
POST /users/{id | userPrincipalName}/profile/emails
```

## <a name="request-headers"></a><span data-ttu-id="e391e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e391e-118">Request headers</span></span>
|<span data-ttu-id="e391e-119">名称</span><span class="sxs-lookup"><span data-stu-id="e391e-119">Name</span></span>|<span data-ttu-id="e391e-120">说明</span><span class="sxs-lookup"><span data-stu-id="e391e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e391e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e391e-121">Authorization</span></span>|<span data-ttu-id="e391e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e391e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e391e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e391e-124">Content-Type</span></span>|<span data-ttu-id="e391e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e391e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e391e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e391e-127">Request body</span></span>
<span data-ttu-id="e391e-128">在请求正文中，提供 [itemEmail](../resources/itememail.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e391e-128">In the request body, supply a JSON representation of the [itemEmail](../resources/itememail.md) object.</span></span>

<span data-ttu-id="e391e-129">下表显示了在用户[配置文件](../resources/profile.md)中创建新的[itemEmail](../resources/itememail.md)对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="e391e-129">The following table shows the properties that are possible to set when creating a new [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="e391e-130">属性</span><span class="sxs-lookup"><span data-stu-id="e391e-130">Property</span></span>|<span data-ttu-id="e391e-131">类型</span><span class="sxs-lookup"><span data-stu-id="e391e-131">Type</span></span>|<span data-ttu-id="e391e-132">说明</span><span class="sxs-lookup"><span data-stu-id="e391e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e391e-133">address</span><span class="sxs-lookup"><span data-stu-id="e391e-133">address</span></span>|<span data-ttu-id="e391e-134">String</span><span class="sxs-lookup"><span data-stu-id="e391e-134">String</span></span>|<span data-ttu-id="e391e-135">电子邮件地址本身。</span><span class="sxs-lookup"><span data-stu-id="e391e-135">The email address itself.</span></span>|
|<span data-ttu-id="e391e-136">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="e391e-136">allowedAudiences</span></span>|<span data-ttu-id="e391e-137">String</span><span class="sxs-lookup"><span data-stu-id="e391e-137">String</span></span>|<span data-ttu-id="e391e-138">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="e391e-138">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="e391e-139">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="e391e-139">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="e391e-140">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e391e-140">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e391e-141">displayName</span><span class="sxs-lookup"><span data-stu-id="e391e-141">displayName</span></span>|<span data-ttu-id="e391e-142">String</span><span class="sxs-lookup"><span data-stu-id="e391e-142">String</span></span>|<span data-ttu-id="e391e-143">用户与特定电子邮件地址相关联的名称或标签。</span><span class="sxs-lookup"><span data-stu-id="e391e-143">The name or label a user has associated with a particular email address.</span></span>|
|<span data-ttu-id="e391e-144">推导</span><span class="sxs-lookup"><span data-stu-id="e391e-144">inference</span></span>|[<span data-ttu-id="e391e-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="e391e-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="e391e-146">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="e391e-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="e391e-147">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="e391e-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e391e-148">source</span><span class="sxs-lookup"><span data-stu-id="e391e-148">source</span></span>|[<span data-ttu-id="e391e-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="e391e-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="e391e-150">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="e391e-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="e391e-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="e391e-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e391e-152">type</span><span class="sxs-lookup"><span data-stu-id="e391e-152">type</span></span>|<span data-ttu-id="e391e-153">emailType</span><span class="sxs-lookup"><span data-stu-id="e391e-153">emailType</span></span>|<span data-ttu-id="e391e-154">电子邮件地址的类型。</span><span class="sxs-lookup"><span data-stu-id="e391e-154">The type of email address.</span></span> <span data-ttu-id="e391e-155">可取值为：`unknown`、`work`、`personal`、`main`、`other`。</span><span class="sxs-lookup"><span data-stu-id="e391e-155">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>|



## <a name="response"></a><span data-ttu-id="e391e-156">响应</span><span class="sxs-lookup"><span data-stu-id="e391e-156">Response</span></span>

<span data-ttu-id="e391e-157">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [itemEmail](../resources/itememail.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e391e-157">If successful, this method returns a `201 Created` response code and an [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e391e-158">示例</span><span class="sxs-lookup"><span data-stu-id="e391e-158">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="e391e-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="e391e-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e391e-160">C#</span><span class="sxs-lookup"><span data-stu-id="e391e-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itememail-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e391e-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e391e-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itememail-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e391e-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e391e-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itememail-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e391e-163">Java</span><span class="sxs-lookup"><span data-stu-id="e391e-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-itememail-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e391e-164">响应</span><span class="sxs-lookup"><span data-stu-id="e391e-164">Response</span></span>
<span data-ttu-id="e391e-165">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e391e-165">**Note:** The response object shown here might be shortened for readability.</span></span>
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


