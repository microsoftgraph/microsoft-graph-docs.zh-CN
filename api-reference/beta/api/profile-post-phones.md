---
title: 创建 itemPhone
description: 使用此 API 创建新的 itemPhone。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f0d2b947c2045499f91d405ddef4eb79b39430ad
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811593"
---
# <a name="create-itemphonenumber"></a><span data-ttu-id="ebf39-103">创建 itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ebf39-103">Create itemPhoneNumber</span></span>

<span data-ttu-id="ebf39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebf39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebf39-105">使用此 API 在用户的[配置文件](../resources/profile.md)中创建新的[itemPhone](../resources/itemphone.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ebf39-105">Use this API to create a new [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ebf39-106">权限</span><span class="sxs-lookup"><span data-stu-id="ebf39-106">Permissions</span></span>

<span data-ttu-id="ebf39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ebf39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ebf39-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ebf39-109">Permission type</span></span>                        | <span data-ttu-id="ebf39-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ebf39-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ebf39-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebf39-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ebf39-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="ebf39-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ebf39-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ebf39-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebf39-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="ebf39-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ebf39-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ebf39-115">Application</span></span>                            | <span data-ttu-id="ebf39-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebf39-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="ebf39-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebf39-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/phones
POST /users/{userId}/profile/phones
```

## <a name="request-headers"></a><span data-ttu-id="ebf39-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ebf39-118">Request headers</span></span>
|<span data-ttu-id="ebf39-119">名称</span><span class="sxs-lookup"><span data-stu-id="ebf39-119">Name</span></span>|<span data-ttu-id="ebf39-120">说明</span><span class="sxs-lookup"><span data-stu-id="ebf39-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ebf39-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebf39-121">Authorization</span></span>|<span data-ttu-id="ebf39-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ebf39-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ebf39-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ebf39-124">Content-Type</span></span>|<span data-ttu-id="ebf39-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ebf39-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebf39-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebf39-127">Request body</span></span>
<span data-ttu-id="ebf39-128">在请求正文中，提供 [itemPhone](../resources/itemphone.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebf39-128">In the request body, supply a JSON representation of the [itemPhone](../resources/itemphone.md) object.</span></span>

<span data-ttu-id="ebf39-129">下表显示了在用户配置文件中创建新的 [itemPhone](../resources/itemphone.md) 对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="ebf39-129">The following table shows the properties that are possible to set when you create a new [itemPhone](../resources/itemphone.md) object in a users profile.</span></span>

|<span data-ttu-id="ebf39-130">属性</span><span class="sxs-lookup"><span data-stu-id="ebf39-130">Property</span></span>|<span data-ttu-id="ebf39-131">类型</span><span class="sxs-lookup"><span data-stu-id="ebf39-131">Type</span></span>|<span data-ttu-id="ebf39-132">说明</span><span class="sxs-lookup"><span data-stu-id="ebf39-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebf39-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="ebf39-133">allowedAudiences</span></span>|<span data-ttu-id="ebf39-134">String</span><span class="sxs-lookup"><span data-stu-id="ebf39-134">String</span></span>|<span data-ttu-id="ebf39-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="ebf39-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="ebf39-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ebf39-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="ebf39-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ebf39-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ebf39-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ebf39-138">displayName</span></span>|<span data-ttu-id="ebf39-139">String</span><span class="sxs-lookup"><span data-stu-id="ebf39-139">String</span></span>|<span data-ttu-id="ebf39-140">友好名称用户已分配了此电话号码。</span><span class="sxs-lookup"><span data-stu-id="ebf39-140">Friendly name the user has assigned this phone number.</span></span> |
|<span data-ttu-id="ebf39-141">推导</span><span class="sxs-lookup"><span data-stu-id="ebf39-141">inference</span></span>|[<span data-ttu-id="ebf39-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="ebf39-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="ebf39-143">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="ebf39-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="ebf39-144">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ebf39-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ebf39-145">数字</span><span class="sxs-lookup"><span data-stu-id="ebf39-145">number</span></span>|<span data-ttu-id="ebf39-146">String</span><span class="sxs-lookup"><span data-stu-id="ebf39-146">String</span></span>|<span data-ttu-id="ebf39-147">用户提供的电话号码。</span><span class="sxs-lookup"><span data-stu-id="ebf39-147">Phone number provided by the user.</span></span>|
|<span data-ttu-id="ebf39-148">source</span><span class="sxs-lookup"><span data-stu-id="ebf39-148">source</span></span>|[<span data-ttu-id="ebf39-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="ebf39-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="ebf39-150">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="ebf39-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="ebf39-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ebf39-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ebf39-152">type</span><span class="sxs-lookup"><span data-stu-id="ebf39-152">type</span></span>|<span data-ttu-id="ebf39-153">phoneType</span><span class="sxs-lookup"><span data-stu-id="ebf39-153">phoneType</span></span>|<span data-ttu-id="ebf39-154">对象中的电话号码的类型。</span><span class="sxs-lookup"><span data-stu-id="ebf39-154">The type of phone number within the object.</span></span> <span data-ttu-id="ebf39-155">可取值为：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="ebf39-155">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="response"></a><span data-ttu-id="ebf39-156">响应</span><span class="sxs-lookup"><span data-stu-id="ebf39-156">Response</span></span>

<span data-ttu-id="ebf39-157">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [itemPhone](../resources/itemphone.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ebf39-157">If successful, this method returns a `201 Created` response code and an [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ebf39-158">示例</span><span class="sxs-lookup"><span data-stu-id="ebf39-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ebf39-159">请求</span><span class="sxs-lookup"><span data-stu-id="ebf39-159">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_itemphone_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/phones
Content-Type: application/json
Content-length: 382

{
  "displayName": "Car Phone",
  "number": "+7 499 342 22 13"
}
```


### <a name="response"></a><span data-ttu-id="ebf39-160">响应</span><span class="sxs-lookup"><span data-stu-id="ebf39-160">Response</span></span>
<span data-ttu-id="ebf39-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ebf39-161">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
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
  "displayName": "Car Phone",
  "type": null,
  "number": "+7 499 342 22 13"
}
```
