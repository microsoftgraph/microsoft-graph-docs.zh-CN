---
title: 更新 personWebsite
description: 更新用户的配置文件中的 personWebsite 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 2b09a39d5821d095e8e3a27eb1ec1bf95dda754a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811608"
---
# <a name="update-personwebsite"></a><span data-ttu-id="bdfbb-103">更新 personwebsite</span><span class="sxs-lookup"><span data-stu-id="bdfbb-103">Update personwebsite</span></span>

<span data-ttu-id="bdfbb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdfbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdfbb-105">更新用户的[配置文件](../resources/profile.md)中的[personWebsite](../resources/personwebsite.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-105">Update the properties of [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bdfbb-106">权限</span><span class="sxs-lookup"><span data-stu-id="bdfbb-106">Permissions</span></span>

<span data-ttu-id="bdfbb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bdfbb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bdfbb-109">Permission type</span></span>                        | <span data-ttu-id="bdfbb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bdfbb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bdfbb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bdfbb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bdfbb-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="bdfbb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bdfbb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdfbb-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="bdfbb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bdfbb-115">Application</span></span>                            | <span data-ttu-id="bdfbb-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdfbb-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="bdfbb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bdfbb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/websites/{id}
PATCH /users/{id | userPrincipalName}/profile/websites/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bdfbb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bdfbb-118">Request headers</span></span>

| <span data-ttu-id="bdfbb-119">名称</span><span class="sxs-lookup"><span data-stu-id="bdfbb-119">Name</span></span>           |<span data-ttu-id="bdfbb-120">说明</span><span class="sxs-lookup"><span data-stu-id="bdfbb-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="bdfbb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdfbb-121">Authorization</span></span>  | <span data-ttu-id="bdfbb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="bdfbb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bdfbb-124">Content-Type</span></span>   | <span data-ttu-id="bdfbb-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bdfbb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdfbb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bdfbb-127">Request body</span></span>

<span data-ttu-id="bdfbb-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bdfbb-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bdfbb-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="bdfbb-131">属性</span><span class="sxs-lookup"><span data-stu-id="bdfbb-131">Property</span></span>|<span data-ttu-id="bdfbb-132">类型</span><span class="sxs-lookup"><span data-stu-id="bdfbb-132">Type</span></span>|<span data-ttu-id="bdfbb-133">说明</span><span class="sxs-lookup"><span data-stu-id="bdfbb-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdfbb-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="bdfbb-134">allowedAudiences</span></span>|<span data-ttu-id="bdfbb-135">String</span><span class="sxs-lookup"><span data-stu-id="bdfbb-135">String</span></span>|<span data-ttu-id="bdfbb-136">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="bdfbb-137">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="bdfbb-138">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bdfbb-139">categories</span><span class="sxs-lookup"><span data-stu-id="bdfbb-139">categories</span></span>|<span data-ttu-id="bdfbb-140">String collection</span><span class="sxs-lookup"><span data-stu-id="bdfbb-140">String collection</span></span>|<span data-ttu-id="bdfbb-141">包含用户与网站相关联的类别 (例如，个人、食谱) 。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-141">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>|
|<span data-ttu-id="bdfbb-142">description</span><span class="sxs-lookup"><span data-stu-id="bdfbb-142">description</span></span>|<span data-ttu-id="bdfbb-143">String</span><span class="sxs-lookup"><span data-stu-id="bdfbb-143">String</span></span>|<span data-ttu-id="bdfbb-144">包含网站的说明。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-144">Contains a description of the website.</span></span>|
|<span data-ttu-id="bdfbb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="bdfbb-145">displayName</span></span>|<span data-ttu-id="bdfbb-146">String</span><span class="sxs-lookup"><span data-stu-id="bdfbb-146">String</span></span>|<span data-ttu-id="bdfbb-147">包含网站的友好名称。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-147">Contains a friendly name for the website.</span></span>|
|<span data-ttu-id="bdfbb-148">推导</span><span class="sxs-lookup"><span data-stu-id="bdfbb-148">inference</span></span>|[<span data-ttu-id="bdfbb-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="bdfbb-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="bdfbb-150">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="bdfbb-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="bdfbb-152">webUrl</span><span class="sxs-lookup"><span data-stu-id="bdfbb-152">webUrl</span></span>|<span data-ttu-id="bdfbb-153">String</span><span class="sxs-lookup"><span data-stu-id="bdfbb-153">String</span></span>|<span data-ttu-id="bdfbb-154">包含指向网站本身的链接。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-154">Contains a link to the website itself.</span></span>|

## <a name="response"></a><span data-ttu-id="bdfbb-155">响应</span><span class="sxs-lookup"><span data-stu-id="bdfbb-155">Response</span></span>

<span data-ttu-id="bdfbb-156">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [personWebsite](../resources/personwebsite.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-156">If successful, this method returns a `200 OK` response code and an updated [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bdfbb-157">示例</span><span class="sxs-lookup"><span data-stu-id="bdfbb-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bdfbb-158">请求</span><span class="sxs-lookup"><span data-stu-id="bdfbb-158">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="bdfbb-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdfbb-159">HTTP</span></span>](#tab/http)

<span data-ttu-id="bdfbb-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-160">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_personwebsite"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/websites/{id}
Content-type: application/json

{
  "description": "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway"
}
```
# <a name="c"></a>[<span data-ttu-id="bdfbb-161">C#</span><span class="sxs-lookup"><span data-stu-id="bdfbb-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personwebsite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bdfbb-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdfbb-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personwebsite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bdfbb-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bdfbb-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personwebsite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="bdfbb-164">响应</span><span class="sxs-lookup"><span data-stu-id="bdfbb-164">Response</span></span>

<span data-ttu-id="bdfbb-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-165">The following is an example of the response.</span></span>

> <span data-ttu-id="bdfbb-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bdfbb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personWebsite"
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
  "categories": [
    "football"
  ],
  "description": "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway",
  "displayName": "Lyn Damer",
  "webUrl": "www.lyndamer.no"
}
```
