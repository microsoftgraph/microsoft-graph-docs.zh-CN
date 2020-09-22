---
title: 更新 personAnniversary
description: 更新 personAnniversary 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0365abe159184e7d492d24de644663ffdd183775
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019819"
---
# <a name="update-personanniversary"></a><span data-ttu-id="a9804-103">更新 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="a9804-103">Update personAnniversary</span></span>

<span data-ttu-id="a9804-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9804-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9804-105">更新用户的[配置文件](../resources/profile.md)中的[personAnniversary](../resources/personanniversary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a9804-105">Update the properties of a [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a9804-106">权限</span><span class="sxs-lookup"><span data-stu-id="a9804-106">Permissions</span></span>

<span data-ttu-id="a9804-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9804-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9804-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9804-109">Permission type</span></span>                        | <span data-ttu-id="a9804-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9804-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a9804-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9804-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9804-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="a9804-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="a9804-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9804-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9804-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="a9804-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="a9804-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9804-115">Application</span></span>                            | <span data-ttu-id="a9804-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9804-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="a9804-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9804-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/anniversaries/{id}
PATCH /users/{id | userPrincipalName}/profile/anniversaries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a9804-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9804-118">Request headers</span></span>

| <span data-ttu-id="a9804-119">名称</span><span class="sxs-lookup"><span data-stu-id="a9804-119">Name</span></span>           |<span data-ttu-id="a9804-120">说明</span><span class="sxs-lookup"><span data-stu-id="a9804-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="a9804-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9804-121">Authorization</span></span>  | <span data-ttu-id="a9804-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9804-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="a9804-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a9804-124">Content-Type</span></span>   | <span data-ttu-id="a9804-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a9804-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9804-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9804-127">Request body</span></span>

<span data-ttu-id="a9804-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="a9804-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a9804-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="a9804-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a9804-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a9804-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="a9804-131">下表显示了可以在用户[配置文件](../resources/profile.md)中的现有[personAnniversary](../resources/personanniversary.md)对象内进行更新的属性。</span><span class="sxs-lookup"><span data-stu-id="a9804-131">The following table shows the properties that are possible to update within an existing [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="a9804-132">属性</span><span class="sxs-lookup"><span data-stu-id="a9804-132">Property</span></span>|<span data-ttu-id="a9804-133">类型</span><span class="sxs-lookup"><span data-stu-id="a9804-133">Type</span></span>|<span data-ttu-id="a9804-134">说明</span><span class="sxs-lookup"><span data-stu-id="a9804-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9804-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="a9804-135">allowedAudiences</span></span>|<span data-ttu-id="a9804-136">String</span><span class="sxs-lookup"><span data-stu-id="a9804-136">String</span></span>|<span data-ttu-id="a9804-137">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="a9804-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="a9804-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a9804-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="a9804-139">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="a9804-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a9804-140">date</span><span class="sxs-lookup"><span data-stu-id="a9804-140">date</span></span>|<span data-ttu-id="a9804-141">Date</span><span class="sxs-lookup"><span data-stu-id="a9804-141">Date</span></span>|<span data-ttu-id="a9804-142">包含与周年纪念类型相关联的日期。</span><span class="sxs-lookup"><span data-stu-id="a9804-142">Contains the date associated with the anniversary type.</span></span>|
|<span data-ttu-id="a9804-143">推导</span><span class="sxs-lookup"><span data-stu-id="a9804-143">inference</span></span>|[<span data-ttu-id="a9804-144">inferenceData</span><span class="sxs-lookup"><span data-stu-id="a9804-144">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="a9804-145">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="a9804-145">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="a9804-146">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a9804-146">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a9804-147">type</span><span class="sxs-lookup"><span data-stu-id="a9804-147">type</span></span>|<span data-ttu-id="a9804-148">anniversaryType</span><span class="sxs-lookup"><span data-stu-id="a9804-148">anniversaryType</span></span>|<span data-ttu-id="a9804-149">日期所代表的周年纪念的类型。</span><span class="sxs-lookup"><span data-stu-id="a9804-149">The type of anniversary the date represents.</span></span> <span data-ttu-id="a9804-150">可取值为：`birthday`、`wedding`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="a9804-150">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="a9804-151">响应</span><span class="sxs-lookup"><span data-stu-id="a9804-151">Response</span></span>

<span data-ttu-id="a9804-152">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [personAnniversary](../resources/personanniversary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a9804-152">If successful, this method returns a `200 OK` response code and an updated [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9804-153">示例</span><span class="sxs-lookup"><span data-stu-id="a9804-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a9804-154">请求</span><span class="sxs-lookup"><span data-stu-id="a9804-154">Request</span></span>

<span data-ttu-id="a9804-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a9804-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9804-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9804-156">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a9804-157">C#</span><span class="sxs-lookup"><span data-stu-id="a9804-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9804-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9804-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9804-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9804-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a9804-160">响应</span><span class="sxs-lookup"><span data-stu-id="a9804-160">Response</span></span>

<span data-ttu-id="a9804-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a9804-161">The following is an example of the response.</span></span>

> <span data-ttu-id="a9804-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a9804-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


