---
title: 更新 personAnniversary
description: 更新 personAnniversary 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 7506a62e45246de610ab31d6cd04fa042b0492c4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037849"
---
# <a name="update-personanniversary"></a><span data-ttu-id="0a91b-103">更新 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="0a91b-103">Update personAnniversary</span></span>

<span data-ttu-id="0a91b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a91b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a91b-105">更新用户配置文件 [中的 personAnniversary](../resources/personanniversary.md) 对象 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="0a91b-105">Update the properties of a [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0a91b-106">权限</span><span class="sxs-lookup"><span data-stu-id="0a91b-106">Permissions</span></span>

<span data-ttu-id="0a91b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a91b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a91b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a91b-109">Permission type</span></span>                        | <span data-ttu-id="0a91b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a91b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0a91b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a91b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a91b-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a91b-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0a91b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a91b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a91b-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a91b-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0a91b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a91b-115">Application</span></span>                            | <span data-ttu-id="0a91b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a91b-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="0a91b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a91b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/anniversaries/{id}
PATCH /users/{id | userPrincipalName}/profile/anniversaries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0a91b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a91b-118">Request headers</span></span>

| <span data-ttu-id="0a91b-119">名称</span><span class="sxs-lookup"><span data-stu-id="0a91b-119">Name</span></span>           |<span data-ttu-id="0a91b-120">说明</span><span class="sxs-lookup"><span data-stu-id="0a91b-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="0a91b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a91b-121">Authorization</span></span>  | <span data-ttu-id="0a91b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a91b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0a91b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0a91b-124">Content-Type</span></span>   | <span data-ttu-id="0a91b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0a91b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a91b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a91b-127">Request body</span></span>

<span data-ttu-id="0a91b-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="0a91b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0a91b-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="0a91b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0a91b-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0a91b-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="0a91b-131">下表显示了在用户配置文件中的现有 [personAnniversary](../resources/personanniversary.md) 对象中可以更新 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="0a91b-131">The following table shows the properties that are possible to update within an existing [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="0a91b-132">属性</span><span class="sxs-lookup"><span data-stu-id="0a91b-132">Property</span></span>|<span data-ttu-id="0a91b-133">类型</span><span class="sxs-lookup"><span data-stu-id="0a91b-133">Type</span></span>|<span data-ttu-id="0a91b-134">说明</span><span class="sxs-lookup"><span data-stu-id="0a91b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a91b-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="0a91b-135">allowedAudiences</span></span>|<span data-ttu-id="0a91b-136">String</span><span class="sxs-lookup"><span data-stu-id="0a91b-136">String</span></span>|<span data-ttu-id="0a91b-137">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="0a91b-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="0a91b-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0a91b-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="0a91b-139">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0a91b-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0a91b-140">date</span><span class="sxs-lookup"><span data-stu-id="0a91b-140">date</span></span>|<span data-ttu-id="0a91b-141">Date</span><span class="sxs-lookup"><span data-stu-id="0a91b-141">Date</span></span>|<span data-ttu-id="0a91b-142">包含与周年类型关联的日期。</span><span class="sxs-lookup"><span data-stu-id="0a91b-142">Contains the date associated with the anniversary type.</span></span>|
|<span data-ttu-id="0a91b-143">inference</span><span class="sxs-lookup"><span data-stu-id="0a91b-143">inference</span></span>|[<span data-ttu-id="0a91b-144">inferenceData</span><span class="sxs-lookup"><span data-stu-id="0a91b-144">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="0a91b-145">如果实体是由创建或修改应用程序推断出来的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="0a91b-145">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="0a91b-146">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0a91b-146">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0a91b-147">type</span><span class="sxs-lookup"><span data-stu-id="0a91b-147">type</span></span>|<span data-ttu-id="0a91b-148">anniversaryType</span><span class="sxs-lookup"><span data-stu-id="0a91b-148">anniversaryType</span></span>|<span data-ttu-id="0a91b-149">日期表示的周年纪念日的类型。</span><span class="sxs-lookup"><span data-stu-id="0a91b-149">The type of anniversary the date represents.</span></span> <span data-ttu-id="0a91b-150">可取值为：`birthday`、`wedding`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0a91b-150">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="0a91b-151">响应</span><span class="sxs-lookup"><span data-stu-id="0a91b-151">Response</span></span>

<span data-ttu-id="0a91b-152">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [personAnniversary](../resources/personanniversary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0a91b-152">If successful, this method returns a `200 OK` response code and an updated [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0a91b-153">示例</span><span class="sxs-lookup"><span data-stu-id="0a91b-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0a91b-154">请求</span><span class="sxs-lookup"><span data-stu-id="0a91b-154">Request</span></span>

<span data-ttu-id="0a91b-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0a91b-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0a91b-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a91b-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personanniversary"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/anniversaries/{id}
Content-type: application/json

{
  "allowedAudiences": "contacts"
}
```
# <a name="c"></a>[<span data-ttu-id="0a91b-157">C#</span><span class="sxs-lookup"><span data-stu-id="0a91b-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a91b-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a91b-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a91b-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a91b-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a91b-160">Java</span><span class="sxs-lookup"><span data-stu-id="0a91b-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-personanniversary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0a91b-161">响应</span><span class="sxs-lookup"><span data-stu-id="0a91b-161">Response</span></span>

<span data-ttu-id="0a91b-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0a91b-162">The following is an example of the response.</span></span>

> <span data-ttu-id="0a91b-163">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0a91b-163">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "contacts",
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


