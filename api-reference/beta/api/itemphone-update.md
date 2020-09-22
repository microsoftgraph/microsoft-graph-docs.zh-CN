---
title: 更新 itemphone
description: 更新 itemPhone 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 823dbabbe2936cc7c75af4a480610c7c5d71085c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999348"
---
# <a name="update-itemphonenumber"></a><span data-ttu-id="8b729-103">更新 itemphonenumber</span><span class="sxs-lookup"><span data-stu-id="8b729-103">Update itemphonenumber</span></span>

<span data-ttu-id="8b729-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b729-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b729-105">更新用户的[配置文件](../resources/profile.md)中的[itemPhone](../resources/itemphone.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8b729-105">Update the properties of an [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8b729-106">权限</span><span class="sxs-lookup"><span data-stu-id="8b729-106">Permissions</span></span>

<span data-ttu-id="8b729-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b729-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8b729-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b729-109">Permission type</span></span>                        | <span data-ttu-id="8b729-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b729-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8b729-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b729-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b729-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="8b729-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8b729-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b729-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b729-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="8b729-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="8b729-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b729-115">Application</span></span>                            | <span data-ttu-id="8b729-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b729-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="8b729-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b729-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/phones/{id}
PATCH /user/{userId}/profile/phones/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8b729-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b729-118">Request headers</span></span>
|<span data-ttu-id="8b729-119">名称</span><span class="sxs-lookup"><span data-stu-id="8b729-119">Name</span></span>|<span data-ttu-id="8b729-120">说明</span><span class="sxs-lookup"><span data-stu-id="8b729-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8b729-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b729-121">Authorization</span></span>|<span data-ttu-id="8b729-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8b729-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8b729-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b729-124">Content-Type</span></span>|<span data-ttu-id="8b729-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8b729-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b729-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b729-127">Request body</span></span>

<span data-ttu-id="8b729-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="8b729-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8b729-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="8b729-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8b729-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8b729-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="8b729-131">下表显示了在更新用户配置文件中的 [itemPhone](../resources/itemphone.md) 对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="8b729-131">The following table shows the properties that are possible to set when you update an [itemPhone](../resources/itemphone.md) object in a users profile.</span></span>

|<span data-ttu-id="8b729-132">属性</span><span class="sxs-lookup"><span data-stu-id="8b729-132">Property</span></span>|<span data-ttu-id="8b729-133">类型</span><span class="sxs-lookup"><span data-stu-id="8b729-133">Type</span></span>|<span data-ttu-id="8b729-134">说明</span><span class="sxs-lookup"><span data-stu-id="8b729-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b729-135">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="8b729-135">allowedAudiences</span></span>|<span data-ttu-id="8b729-136">String</span><span class="sxs-lookup"><span data-stu-id="8b729-136">String</span></span>|<span data-ttu-id="8b729-137">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="8b729-137">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="8b729-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="8b729-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="8b729-139">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8b729-139">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8b729-140">displayName</span><span class="sxs-lookup"><span data-stu-id="8b729-140">displayName</span></span>|<span data-ttu-id="8b729-141">String</span><span class="sxs-lookup"><span data-stu-id="8b729-141">String</span></span>|<span data-ttu-id="8b729-142">友好名称用户已分配了此电话号码。</span><span class="sxs-lookup"><span data-stu-id="8b729-142">Friendly name the user has assigned this phone number.</span></span> |
|<span data-ttu-id="8b729-143">推导</span><span class="sxs-lookup"><span data-stu-id="8b729-143">inference</span></span>|[<span data-ttu-id="8b729-144">inferenceData</span><span class="sxs-lookup"><span data-stu-id="8b729-144">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="8b729-145">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="8b729-145">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="8b729-146">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="8b729-146">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8b729-147">数字</span><span class="sxs-lookup"><span data-stu-id="8b729-147">number</span></span>|<span data-ttu-id="8b729-148">String</span><span class="sxs-lookup"><span data-stu-id="8b729-148">String</span></span>|<span data-ttu-id="8b729-149">用户提供的电话号码。</span><span class="sxs-lookup"><span data-stu-id="8b729-149">Phone number provided by the user.</span></span>|
|<span data-ttu-id="8b729-150">source</span><span class="sxs-lookup"><span data-stu-id="8b729-150">source</span></span>|[<span data-ttu-id="8b729-151">personDataSource</span><span class="sxs-lookup"><span data-stu-id="8b729-151">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="8b729-152">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="8b729-152">Where the values originated if synced from another service.</span></span> <span data-ttu-id="8b729-153">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="8b729-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8b729-154">type</span><span class="sxs-lookup"><span data-stu-id="8b729-154">type</span></span>|<span data-ttu-id="8b729-155">phoneType</span><span class="sxs-lookup"><span data-stu-id="8b729-155">phoneType</span></span>|<span data-ttu-id="8b729-156">对象中的电话号码的类型。</span><span class="sxs-lookup"><span data-stu-id="8b729-156">The type of phone number within the object.</span></span> <span data-ttu-id="8b729-157">可取值为：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="8b729-157">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="response"></a><span data-ttu-id="8b729-158">响应</span><span class="sxs-lookup"><span data-stu-id="8b729-158">Response</span></span>

<span data-ttu-id="8b729-159">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [itemPhone](../resources/itemphone.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8b729-159">If successful, this method returns a `200 OK` response code and an updated [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b729-160">示例</span><span class="sxs-lookup"><span data-stu-id="8b729-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8b729-161">请求</span><span class="sxs-lookup"><span data-stu-id="8b729-161">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="8b729-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b729-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itemphone"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/user/{userId}/profile/phones/{id}
Content-Type: application/json
Content-length: 382

{
  "type": "other"
}
```
# <a name="c"></a>[<span data-ttu-id="8b729-163">C#</span><span class="sxs-lookup"><span data-stu-id="8b729-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b729-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b729-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b729-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b729-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8b729-166">响应</span><span class="sxs-lookup"><span data-stu-id="8b729-166">Response</span></span>
<span data-ttu-id="8b729-167">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8b729-167">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
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
  "displayName": "Car Phone",
  "type": "other",
  "number": "+7 499 342 22 13"
}
```


