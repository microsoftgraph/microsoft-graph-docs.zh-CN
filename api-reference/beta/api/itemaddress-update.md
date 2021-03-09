---
title: 更新 itemAddress
description: 更新 itemAddress 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f53f5ad68919898dc337ed9b7c0f106ed3fa6c41
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578694"
---
# <a name="update-itemaddress"></a><span data-ttu-id="0fa62-103">更新 itemAddress</span><span class="sxs-lookup"><span data-stu-id="0fa62-103">Update itemAddress</span></span>
<span data-ttu-id="0fa62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fa62-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0fa62-105">更新 [itemAddress 对象](../resources/itemaddress.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="0fa62-105">Update the properties of an [itemAddress](../resources/itemaddress.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fa62-106">权限</span><span class="sxs-lookup"><span data-stu-id="0fa62-106">Permissions</span></span>

<span data-ttu-id="0fa62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0fa62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0fa62-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0fa62-109">Permission type</span></span>                        | <span data-ttu-id="0fa62-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0fa62-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="0fa62-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0fa62-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0fa62-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fa62-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0fa62-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0fa62-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fa62-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fa62-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0fa62-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0fa62-115">Application</span></span>                            | <span data-ttu-id="0fa62-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fa62-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="0fa62-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0fa62-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/addresses/{id}
PATCH /users/{id | userPrincipalName}/profile/addresses/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0fa62-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0fa62-118">Request headers</span></span>
|<span data-ttu-id="0fa62-119">名称</span><span class="sxs-lookup"><span data-stu-id="0fa62-119">Name</span></span>|<span data-ttu-id="0fa62-120">说明</span><span class="sxs-lookup"><span data-stu-id="0fa62-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0fa62-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fa62-121">Authorization</span></span>|<span data-ttu-id="0fa62-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0fa62-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0fa62-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fa62-124">Content-Type</span></span>|<span data-ttu-id="0fa62-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0fa62-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fa62-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0fa62-127">Request body</span></span>

<span data-ttu-id="0fa62-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="0fa62-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0fa62-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="0fa62-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0fa62-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0fa62-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="0fa62-131">属性</span><span class="sxs-lookup"><span data-stu-id="0fa62-131">Property</span></span>|<span data-ttu-id="0fa62-132">类型</span><span class="sxs-lookup"><span data-stu-id="0fa62-132">Type</span></span>|<span data-ttu-id="0fa62-133">说明</span><span class="sxs-lookup"><span data-stu-id="0fa62-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fa62-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="0fa62-134">allowedAudiences</span></span>|<span data-ttu-id="0fa62-135">字符串</span><span class="sxs-lookup"><span data-stu-id="0fa62-135">String</span></span>|<span data-ttu-id="0fa62-136">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="0fa62-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="0fa62-137">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0fa62-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="0fa62-138">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0fa62-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0fa62-139">detail</span><span class="sxs-lookup"><span data-stu-id="0fa62-139">detail</span></span>|[<span data-ttu-id="0fa62-140">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="0fa62-140">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="0fa62-141">有关地址本身的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0fa62-141">Details about the address itself.</span></span>|
|<span data-ttu-id="0fa62-142">displayName</span><span class="sxs-lookup"><span data-stu-id="0fa62-142">displayName</span></span>|<span data-ttu-id="0fa62-143">字符串</span><span class="sxs-lookup"><span data-stu-id="0fa62-143">String</span></span>|<span data-ttu-id="0fa62-144">用户已分配给此地址的友好名称。</span><span class="sxs-lookup"><span data-stu-id="0fa62-144">Friendly name the user has assigned to this address.</span></span> |
|<span data-ttu-id="0fa62-145">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="0fa62-145">geoCoordinates</span></span>|[<span data-ttu-id="0fa62-146">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="0fa62-146">geoCoordinates</span></span>](../resources/geocoordinates.md)|<span data-ttu-id="0fa62-147">地址的地理coordinates。</span><span class="sxs-lookup"><span data-stu-id="0fa62-147">The geocoordinates of the address.</span></span>|
|<span data-ttu-id="0fa62-148">推断</span><span class="sxs-lookup"><span data-stu-id="0fa62-148">inference</span></span>|[<span data-ttu-id="0fa62-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="0fa62-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="0fa62-150">包含实体是否由创建或修改应用程序推断的推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="0fa62-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="0fa62-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0fa62-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0fa62-152">source</span><span class="sxs-lookup"><span data-stu-id="0fa62-152">source</span></span>|[<span data-ttu-id="0fa62-153">personDataSource</span><span class="sxs-lookup"><span data-stu-id="0fa62-153">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="0fa62-154">如果从另一个服务同步，则值源自何处。</span><span class="sxs-lookup"><span data-stu-id="0fa62-154">Where the values originated if synced from another service.</span></span> <span data-ttu-id="0fa62-155">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0fa62-155">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="0fa62-156">响应</span><span class="sxs-lookup"><span data-stu-id="0fa62-156">Response</span></span>

<span data-ttu-id="0fa62-157">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [itemAddress](../resources/itemaddress.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0fa62-157">If successful, this method returns a `200 OK` response code and an updated [itemAddress](../resources/itemaddress.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0fa62-158">示例</span><span class="sxs-lookup"><span data-stu-id="0fa62-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0fa62-159">请求</span><span class="sxs-lookup"><span data-stu-id="0fa62-159">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="0fa62-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fa62-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itemaddress"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{userId}/profile/addresses/{id}
Content-Type: application/json
Content-length: 497

{
  "allowedAudiences": "me",
  "displayName": "Secret Hideout",
}
```
# <a name="c"></a>[<span data-ttu-id="0fa62-161">C#</span><span class="sxs-lookup"><span data-stu-id="0fa62-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fa62-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fa62-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fa62-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fa62-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0fa62-164">响应</span><span class="sxs-lookup"><span data-stu-id="0fa62-164">Response</span></span>
<span data-ttu-id="0fa62-165">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0fa62-165">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAddress"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "me",
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
  "displayName": "Secret Hideout",
  "detail": {
    "type": "home",
    "postOfficeBox": null,
    "street": "221B Baker Street",
    "city": "London",
    "state": null,
    "countryOrRegion": "United Kingdom",
    "postalCode": "E14 3TD"
  },
  "geoCoordinates": null
}
```



