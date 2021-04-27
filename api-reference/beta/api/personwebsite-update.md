---
title: 更新 personWebsite
description: 更新用户配置文件中 personWebsite 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8f7b5787469cb4af5964fe6f2ea8b4ad8b135823
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050043"
---
# <a name="update-personwebsite"></a><span data-ttu-id="460e5-103">更新 personwebsite</span><span class="sxs-lookup"><span data-stu-id="460e5-103">Update personwebsite</span></span>

<span data-ttu-id="460e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="460e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="460e5-105">更新用户配置文件中的 [personWebsite](../resources/personwebsite.md) 对象 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="460e5-105">Update the properties of [personWebsite](../resources/personwebsite.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="460e5-106">权限</span><span class="sxs-lookup"><span data-stu-id="460e5-106">Permissions</span></span>

<span data-ttu-id="460e5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="460e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="460e5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="460e5-109">Permission type</span></span>                        | <span data-ttu-id="460e5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="460e5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="460e5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="460e5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="460e5-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="460e5-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="460e5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="460e5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="460e5-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="460e5-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="460e5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="460e5-115">Application</span></span>                            | <span data-ttu-id="460e5-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="460e5-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="460e5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="460e5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/websites/{id}
PATCH /users/{id | userPrincipalName}/profile/websites/{id}
```

## <a name="request-headers"></a><span data-ttu-id="460e5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="460e5-118">Request headers</span></span>

| <span data-ttu-id="460e5-119">名称</span><span class="sxs-lookup"><span data-stu-id="460e5-119">Name</span></span>           |<span data-ttu-id="460e5-120">说明</span><span class="sxs-lookup"><span data-stu-id="460e5-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="460e5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="460e5-121">Authorization</span></span>  | <span data-ttu-id="460e5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="460e5-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="460e5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="460e5-124">Content-Type</span></span>   | <span data-ttu-id="460e5-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="460e5-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="460e5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="460e5-127">Request body</span></span>

<span data-ttu-id="460e5-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="460e5-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="460e5-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="460e5-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="460e5-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="460e5-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="460e5-131">属性</span><span class="sxs-lookup"><span data-stu-id="460e5-131">Property</span></span>|<span data-ttu-id="460e5-132">类型</span><span class="sxs-lookup"><span data-stu-id="460e5-132">Type</span></span>|<span data-ttu-id="460e5-133">说明</span><span class="sxs-lookup"><span data-stu-id="460e5-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="460e5-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="460e5-134">allowedAudiences</span></span>|<span data-ttu-id="460e5-135">String</span><span class="sxs-lookup"><span data-stu-id="460e5-135">String</span></span>|<span data-ttu-id="460e5-136">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="460e5-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="460e5-137">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="460e5-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="460e5-138">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="460e5-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="460e5-139">categories</span><span class="sxs-lookup"><span data-stu-id="460e5-139">categories</span></span>|<span data-ttu-id="460e5-140">String 集合</span><span class="sxs-lookup"><span data-stu-id="460e5-140">String collection</span></span>|<span data-ttu-id="460e5-141">包含用户与网站网站关联的类别 (例如个人、食谱) 。</span><span class="sxs-lookup"><span data-stu-id="460e5-141">Contains categories a user has associated with the website (for example, personal, recipes).</span></span>|
|<span data-ttu-id="460e5-142">说明</span><span class="sxs-lookup"><span data-stu-id="460e5-142">description</span></span>|<span data-ttu-id="460e5-143">String</span><span class="sxs-lookup"><span data-stu-id="460e5-143">String</span></span>|<span data-ttu-id="460e5-144">包含网站的说明。</span><span class="sxs-lookup"><span data-stu-id="460e5-144">Contains a description of the website.</span></span>|
|<span data-ttu-id="460e5-145">displayName</span><span class="sxs-lookup"><span data-stu-id="460e5-145">displayName</span></span>|<span data-ttu-id="460e5-146">String</span><span class="sxs-lookup"><span data-stu-id="460e5-146">String</span></span>|<span data-ttu-id="460e5-147">包含网站的友好名称。</span><span class="sxs-lookup"><span data-stu-id="460e5-147">Contains a friendly name for the website.</span></span>|
|<span data-ttu-id="460e5-148">inference</span><span class="sxs-lookup"><span data-stu-id="460e5-148">inference</span></span>|[<span data-ttu-id="460e5-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="460e5-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="460e5-150">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="460e5-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="460e5-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="460e5-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="460e5-152">webUrl</span><span class="sxs-lookup"><span data-stu-id="460e5-152">webUrl</span></span>|<span data-ttu-id="460e5-153">String</span><span class="sxs-lookup"><span data-stu-id="460e5-153">String</span></span>|<span data-ttu-id="460e5-154">包含指向网站本身的链接。</span><span class="sxs-lookup"><span data-stu-id="460e5-154">Contains a link to the website itself.</span></span>|

## <a name="response"></a><span data-ttu-id="460e5-155">响应</span><span class="sxs-lookup"><span data-stu-id="460e5-155">Response</span></span>

<span data-ttu-id="460e5-156">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [personWebsite](../resources/personwebsite.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="460e5-156">If successful, this method returns a `200 OK` response code and an updated [personWebsite](../resources/personwebsite.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="460e5-157">示例</span><span class="sxs-lookup"><span data-stu-id="460e5-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="460e5-158">请求</span><span class="sxs-lookup"><span data-stu-id="460e5-158">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="460e5-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="460e5-159">HTTP</span></span>](#tab/http)

<span data-ttu-id="460e5-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="460e5-160">The following is an example of the request.</span></span>
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
# <a name="c"></a>[<span data-ttu-id="460e5-161">C#</span><span class="sxs-lookup"><span data-stu-id="460e5-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personwebsite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="460e5-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="460e5-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personwebsite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="460e5-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="460e5-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personwebsite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="460e5-164">Java</span><span class="sxs-lookup"><span data-stu-id="460e5-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-personwebsite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="460e5-165">响应</span><span class="sxs-lookup"><span data-stu-id="460e5-165">Response</span></span>

<span data-ttu-id="460e5-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="460e5-166">The following is an example of the response.</span></span>

> <span data-ttu-id="460e5-167">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="460e5-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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


