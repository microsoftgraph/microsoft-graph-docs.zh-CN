---
title: 创建地址
description: 创建一个新的地址对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a7338e553b483d4833c93036bf580aea4c9e4b00
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812913"
---
# <a name="create-addresses"></a><span data-ttu-id="9d491-103">创建地址</span><span class="sxs-lookup"><span data-stu-id="9d491-103">Create addresses</span></span>
<span data-ttu-id="9d491-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d491-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d491-105">在用户的[配置文件](../resources/profile.md)中创建新的[itemAddress](../resources/itemaddress.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9d491-105">Create a new [itemAddress](../resources/itemaddress.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9d491-106">权限</span><span class="sxs-lookup"><span data-stu-id="9d491-106">Permissions</span></span>

<span data-ttu-id="9d491-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d491-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d491-109">Permission type</span></span>                        | <span data-ttu-id="9d491-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d491-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="9d491-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d491-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d491-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="9d491-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9d491-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d491-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d491-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="9d491-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9d491-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d491-115">Application</span></span>                            | <span data-ttu-id="9d491-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d491-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="9d491-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d491-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/addresses
POST /users/{id | userPrincipalName}/profile/addresses
```

## <a name="request-headers"></a><span data-ttu-id="9d491-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d491-118">Request headers</span></span>
|<span data-ttu-id="9d491-119">名称</span><span class="sxs-lookup"><span data-stu-id="9d491-119">Name</span></span>|<span data-ttu-id="9d491-120">说明</span><span class="sxs-lookup"><span data-stu-id="9d491-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9d491-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d491-121">Authorization</span></span>|<span data-ttu-id="9d491-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9d491-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9d491-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9d491-124">Content-Type</span></span>|<span data-ttu-id="9d491-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9d491-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d491-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d491-127">Request body</span></span>
<span data-ttu-id="9d491-128">在请求正文中，提供 [itemAddress](../resources/itemaddress.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d491-128">In the request body, supply a JSON representation of the [itemAddress](../resources/itemaddress.md) object.</span></span>

<span data-ttu-id="9d491-129">下表显示了在用户[配置文件](../resources/profile.md)中创建新的[itemAddress](../resources/itemaddress.md)对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="9d491-129">The following table shows the properties that are possible to set when creating a new [itemAddress](../resources/itemaddress.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="9d491-130">属性</span><span class="sxs-lookup"><span data-stu-id="9d491-130">Property</span></span>|<span data-ttu-id="9d491-131">类型</span><span class="sxs-lookup"><span data-stu-id="9d491-131">Type</span></span>|<span data-ttu-id="9d491-132">说明</span><span class="sxs-lookup"><span data-stu-id="9d491-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d491-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="9d491-133">allowedAudiences</span></span>|<span data-ttu-id="9d491-134">String</span><span class="sxs-lookup"><span data-stu-id="9d491-134">String</span></span>|<span data-ttu-id="9d491-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="9d491-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="9d491-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="9d491-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="9d491-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="9d491-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9d491-138">介绍</span><span class="sxs-lookup"><span data-stu-id="9d491-138">detail</span></span>|[<span data-ttu-id="9d491-139">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="9d491-139">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="9d491-140">地址本身的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9d491-140">Details about the address itself.</span></span>|
|<span data-ttu-id="9d491-141">displayName</span><span class="sxs-lookup"><span data-stu-id="9d491-141">displayName</span></span>|<span data-ttu-id="9d491-142">String</span><span class="sxs-lookup"><span data-stu-id="9d491-142">String</span></span>|<span data-ttu-id="9d491-143">用户已分配到此地址的友好名称。</span><span class="sxs-lookup"><span data-stu-id="9d491-143">Friendly name the user has assigned to this address.</span></span> |
|<span data-ttu-id="9d491-144">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="9d491-144">geoCoordinates</span></span>|[<span data-ttu-id="9d491-145">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="9d491-145">geoCoordinates</span></span>](../resources/geocoordinates.md)|<span data-ttu-id="9d491-146">地址的 geocoordinates。</span><span class="sxs-lookup"><span data-stu-id="9d491-146">The geocoordinates of the address.</span></span>|
|<span data-ttu-id="9d491-147">推导</span><span class="sxs-lookup"><span data-stu-id="9d491-147">inference</span></span>|[<span data-ttu-id="9d491-148">inferenceData</span><span class="sxs-lookup"><span data-stu-id="9d491-148">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="9d491-149">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="9d491-149">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="9d491-150">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="9d491-150">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="9d491-151">source</span><span class="sxs-lookup"><span data-stu-id="9d491-151">source</span></span>|[<span data-ttu-id="9d491-152">personDataSource</span><span class="sxs-lookup"><span data-stu-id="9d491-152">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="9d491-153">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="9d491-153">Where the values originated if synced from another service.</span></span> <span data-ttu-id="9d491-154">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="9d491-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
## <a name="response"></a><span data-ttu-id="9d491-155">响应</span><span class="sxs-lookup"><span data-stu-id="9d491-155">Response</span></span>

<span data-ttu-id="9d491-156">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [itemAddress](../resources/itemaddress.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9d491-156">If successful, this method returns a `201 Created` response code and an [itemAddress](../resources/itemaddress.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9d491-157">示例</span><span class="sxs-lookup"><span data-stu-id="9d491-157">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="9d491-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d491-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itemaddress_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/addresses
Content-Type: application/json
Content-length: 497

{
  "displayName": "Home",
  "detail": {
    "type": "home",
    "postOfficeBox": null,
    "street": "221B Baker Street",
    "city": "London",
    "state": null,
    "countryOrRegion": "United Kingdom",
    "postalCode": "E14 3TD"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="9d491-159">C#</span><span class="sxs-lookup"><span data-stu-id="9d491-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d491-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d491-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d491-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d491-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9d491-162">响应</span><span class="sxs-lookup"><span data-stu-id="9d491-162">Response</span></span>
<span data-ttu-id="9d491-163">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9d491-163">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAddress"
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
  "source": null,
  "displayName": "Home",
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
