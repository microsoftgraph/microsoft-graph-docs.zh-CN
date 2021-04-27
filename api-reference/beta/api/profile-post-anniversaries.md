---
title: 创建 personAnniversary
description: 使用此 API 创建新的 personAnniversary。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c28e988290c239c8a7977df8eab6d3ae3a945372
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036966"
---
# <a name="create-personanniversary"></a><span data-ttu-id="e62f9-103">创建 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="e62f9-103">Create personAnniversary</span></span>

<span data-ttu-id="e62f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e62f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e62f9-105">使用此 API 在用户配置文件中创建新的 [personAnniversary](../resources/personanniversary.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="e62f9-105">Use this API to create a new [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e62f9-106">权限</span><span class="sxs-lookup"><span data-stu-id="e62f9-106">Permissions</span></span>

<span data-ttu-id="e62f9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e62f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e62f9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e62f9-109">Permission type</span></span>                        | <span data-ttu-id="e62f9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e62f9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e62f9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e62f9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e62f9-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e62f9-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e62f9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e62f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e62f9-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e62f9-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e62f9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e62f9-115">Application</span></span>                            | <span data-ttu-id="e62f9-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e62f9-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e62f9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e62f9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/anniversaries
POST /users/{id | userPrincipalName}/profile/anniversaries
```

## <a name="request-headers"></a><span data-ttu-id="e62f9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e62f9-118">Request headers</span></span>

| <span data-ttu-id="e62f9-119">名称</span><span class="sxs-lookup"><span data-stu-id="e62f9-119">Name</span></span>      |<span data-ttu-id="e62f9-120">说明</span><span class="sxs-lookup"><span data-stu-id="e62f9-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e62f9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e62f9-121">Authorization</span></span>  | <span data-ttu-id="e62f9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e62f9-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e62f9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e62f9-124">Content-Type</span></span>   | <span data-ttu-id="e62f9-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e62f9-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e62f9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e62f9-127">Request body</span></span>

<span data-ttu-id="e62f9-128">在请求正文中，提供 [personAnniversary](../resources/personanniversary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e62f9-128">In the request body, supply a JSON representation of [personAnniversary](../resources/personanniversary.md) object.</span></span>

<span data-ttu-id="e62f9-129">下表显示了在用户配置文件中的新 \*\*personAnniversary\*\*\*\* 对象中可以设置 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="e62f9-129">The following table shows the properties that are possible to set within a new \*\*personAnniversary\*\*\*\* object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="e62f9-130">属性</span><span class="sxs-lookup"><span data-stu-id="e62f9-130">Property</span></span>|<span data-ttu-id="e62f9-131">类型</span><span class="sxs-lookup"><span data-stu-id="e62f9-131">Type</span></span>|<span data-ttu-id="e62f9-132">说明</span><span class="sxs-lookup"><span data-stu-id="e62f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e62f9-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="e62f9-133">allowedAudiences</span></span>|<span data-ttu-id="e62f9-134">String</span><span class="sxs-lookup"><span data-stu-id="e62f9-134">String</span></span>|<span data-ttu-id="e62f9-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="e62f9-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="e62f9-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="e62f9-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="e62f9-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e62f9-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e62f9-138">date</span><span class="sxs-lookup"><span data-stu-id="e62f9-138">date</span></span>|<span data-ttu-id="e62f9-139">Date</span><span class="sxs-lookup"><span data-stu-id="e62f9-139">Date</span></span>|<span data-ttu-id="e62f9-140">包含与周年类型关联的日期。</span><span class="sxs-lookup"><span data-stu-id="e62f9-140">Contains the date associated with the anniversary type.</span></span>|
|<span data-ttu-id="e62f9-141">inference</span><span class="sxs-lookup"><span data-stu-id="e62f9-141">inference</span></span>|[<span data-ttu-id="e62f9-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="e62f9-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="e62f9-143">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="e62f9-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="e62f9-144">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="e62f9-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e62f9-145">source</span><span class="sxs-lookup"><span data-stu-id="e62f9-145">source</span></span>|[<span data-ttu-id="e62f9-146">personDataSource</span><span class="sxs-lookup"><span data-stu-id="e62f9-146">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="e62f9-147">如果从另一个服务同步，则值源自何处。</span><span class="sxs-lookup"><span data-stu-id="e62f9-147">Where the values originated if synced from another service.</span></span> <span data-ttu-id="e62f9-148">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="e62f9-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="e62f9-149">type</span><span class="sxs-lookup"><span data-stu-id="e62f9-149">type</span></span>|<span data-ttu-id="e62f9-150">anniversaryType</span><span class="sxs-lookup"><span data-stu-id="e62f9-150">anniversaryType</span></span>|<span data-ttu-id="e62f9-151">日期表示的周年纪念日的类型。</span><span class="sxs-lookup"><span data-stu-id="e62f9-151">The type of anniversary the date represents.</span></span> <span data-ttu-id="e62f9-152">可取值为：`birthday`、`wedding`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e62f9-152">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="e62f9-153">响应</span><span class="sxs-lookup"><span data-stu-id="e62f9-153">Response</span></span>

<span data-ttu-id="e62f9-154">如果成功，此方法在 `201, Created` 响应正文中返回 响应代码和新 [personAnniversary](../resources/personanniversary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e62f9-154">If successful, this method returns `201, Created` response code and a new [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e62f9-155">示例</span><span class="sxs-lookup"><span data-stu-id="e62f9-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e62f9-156">请求</span><span class="sxs-lookup"><span data-stu-id="e62f9-156">Request</span></span>

<span data-ttu-id="e62f9-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e62f9-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e62f9-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="e62f9-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personanniversary_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/anniversaries
Content-type: application/json

{
  "type": "birthday",
  "date": "1980-01-08"
}
```
# <a name="c"></a>[<span data-ttu-id="e62f9-159">C#</span><span class="sxs-lookup"><span data-stu-id="e62f9-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personanniversary-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e62f9-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e62f9-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personanniversary-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e62f9-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e62f9-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personanniversary-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e62f9-162">Java</span><span class="sxs-lookup"><span data-stu-id="e62f9-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-personanniversary-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="e62f9-163">响应</span><span class="sxs-lookup"><span data-stu-id="e62f9-163">Response</span></span>

<span data-ttu-id="e62f9-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e62f9-164">The following is an example of the response.</span></span>

> <span data-ttu-id="e62f9-165">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e62f9-165">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
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
  "type": "birthday",
  "date": "Date"
}
```


