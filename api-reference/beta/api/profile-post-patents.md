---
title: 创建首要项目
description: 创建新的父对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 8345de1ca41dfd5e338b77c667ef06ae4b3bf31c
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820285"
---
# <a name="create-itempatent"></a><span data-ttu-id="6831d-103">创建 itemPatent</span><span class="sxs-lookup"><span data-stu-id="6831d-103">Create itemPatent</span></span>

<span data-ttu-id="6831d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6831d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6831d-105">在用户的 [配置文件中创建新的 itemPatent](../resources/itempatent.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="6831d-105">Create a new [itemPatent](../resources/itempatent.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6831d-106">权限</span><span class="sxs-lookup"><span data-stu-id="6831d-106">Permissions</span></span>

<span data-ttu-id="6831d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6831d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6831d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6831d-109">Permission type</span></span>                        | <span data-ttu-id="6831d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6831d-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="6831d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6831d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6831d-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6831d-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6831d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6831d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6831d-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6831d-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6831d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6831d-115">Application</span></span>                            | <span data-ttu-id="6831d-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6831d-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="6831d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6831d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/patents
POST /users/{id | userPrincipalName}/profile/patents
```

## <a name="request-headers"></a><span data-ttu-id="6831d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6831d-118">Request headers</span></span>
|<span data-ttu-id="6831d-119">名称</span><span class="sxs-lookup"><span data-stu-id="6831d-119">Name</span></span>|<span data-ttu-id="6831d-120">说明</span><span class="sxs-lookup"><span data-stu-id="6831d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6831d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6831d-121">Authorization</span></span>|<span data-ttu-id="6831d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6831d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6831d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6831d-124">Content-Type</span></span>|<span data-ttu-id="6831d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6831d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6831d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6831d-127">Request body</span></span>
<span data-ttu-id="6831d-128">在请求正文中，提供 [itemPatent 对象的](../resources/itempatent.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6831d-128">In the request body, supply a JSON representation of the [itemPatent](../resources/itempatent.md) object.</span></span>

<span data-ttu-id="6831d-129">下表显示在用户的配置文件中创建新 [itemPatent](../resources/itempatent.md) 对象时可能设置 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="6831d-129">The following table shows the properties that are possible to set when creating a new [itemPatent](../resources/itempatent.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="6831d-130">属性</span><span class="sxs-lookup"><span data-stu-id="6831d-130">Property</span></span>|<span data-ttu-id="6831d-131">类型</span><span class="sxs-lookup"><span data-stu-id="6831d-131">Type</span></span>|<span data-ttu-id="6831d-132">说明</span><span class="sxs-lookup"><span data-stu-id="6831d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6831d-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="6831d-133">allowedAudiences</span></span>|<span data-ttu-id="6831d-134">String</span><span class="sxs-lookup"><span data-stu-id="6831d-134">String</span></span>|<span data-ttu-id="6831d-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="6831d-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="6831d-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="6831d-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="6831d-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="6831d-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6831d-138">description</span><span class="sxs-lookup"><span data-stu-id="6831d-138">description</span></span>|<span data-ttu-id="6831d-139">String</span><span class="sxs-lookup"><span data-stu-id="6831d-139">String</span></span>|<span data-ttu-id="6831d-140">专利或分级说明。</span><span class="sxs-lookup"><span data-stu-id="6831d-140">Descpription of the patent or filing.</span></span> |
|<span data-ttu-id="6831d-141">displayName</span><span class="sxs-lookup"><span data-stu-id="6831d-141">displayName</span></span>|<span data-ttu-id="6831d-142">String</span><span class="sxs-lookup"><span data-stu-id="6831d-142">String</span></span>|<span data-ttu-id="6831d-143">表示属性或下事的标题。</span><span class="sxs-lookup"><span data-stu-id="6831d-143">Title of the patent or filing.</span></span> |
|<span data-ttu-id="6831d-144">推据</span><span class="sxs-lookup"><span data-stu-id="6831d-144">inference</span></span>|[<span data-ttu-id="6831d-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="6831d-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="6831d-146">如果实体受到创建或修改的应用程序的推理，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="6831d-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="6831d-147">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="6831d-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="6831d-148">isPending</span><span class="sxs-lookup"><span data-stu-id="6831d-148">isPending</span></span>        |<span data-ttu-id="6831d-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="6831d-149">Boolean</span></span>     |<span data-ttu-id="6831d-150">表示 Patent 正在挂起。</span><span class="sxs-lookup"><span data-stu-id="6831d-150">Indicates the patent is pending.</span></span>        |
|<span data-ttu-id="6831d-151">issuedDate</span><span class="sxs-lookup"><span data-stu-id="6831d-151">issuedDate</span></span>       |<span data-ttu-id="6831d-152">日期</span><span class="sxs-lookup"><span data-stu-id="6831d-152">Date</span></span>        |<span data-ttu-id="6831d-153">获取该属性的日期。</span><span class="sxs-lookup"><span data-stu-id="6831d-153">The date that the patent was granted.</span></span>   |
|<span data-ttu-id="6831d-154">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="6831d-154">issuingAuthority</span></span> |<span data-ttu-id="6831d-155">String</span><span class="sxs-lookup"><span data-stu-id="6831d-155">String</span></span>      |<span data-ttu-id="6831d-156">授予 Patent 权限的颁发机构。</span><span class="sxs-lookup"><span data-stu-id="6831d-156">Authority which granted the patent.</span></span>     |
|<span data-ttu-id="6831d-157">数字</span><span class="sxs-lookup"><span data-stu-id="6831d-157">number</span></span>           |<span data-ttu-id="6831d-158">String</span><span class="sxs-lookup"><span data-stu-id="6831d-158">String</span></span>      |<span data-ttu-id="6831d-159">Patent 数。</span><span class="sxs-lookup"><span data-stu-id="6831d-159">The patent number.</span></span>                      |
|<span data-ttu-id="6831d-160">source</span><span class="sxs-lookup"><span data-stu-id="6831d-160">source</span></span>|[<span data-ttu-id="6831d-161">personDataSource</span><span class="sxs-lookup"><span data-stu-id="6831d-161">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="6831d-162">同步到其他服务时从哪个位置发送值。</span><span class="sxs-lookup"><span data-stu-id="6831d-162">Where the values originated if synced from another service.</span></span> <span data-ttu-id="6831d-163">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="6831d-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="6831d-164">webUrl</span><span class="sxs-lookup"><span data-stu-id="6831d-164">webUrl</span></span>           |<span data-ttu-id="6831d-165">String</span><span class="sxs-lookup"><span data-stu-id="6831d-165">String</span></span>      |<span data-ttu-id="6831d-166">引用 patent 或 Filing 的 URL。</span><span class="sxs-lookup"><span data-stu-id="6831d-166">URL referencing the patent or filing.</span></span> |

## <a name="response"></a><span data-ttu-id="6831d-167">响应</span><span class="sxs-lookup"><span data-stu-id="6831d-167">Response</span></span>

<span data-ttu-id="6831d-168">如果成功，此方法在响应 `201 Created` 正文中返回 [响应代码和 itemPatent](../resources/itempatent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6831d-168">If successful, this method returns a `201 Created` response code and an [itemPatent](../resources/itempatent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6831d-169">示例</span><span class="sxs-lookup"><span data-stu-id="6831d-169">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="6831d-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="6831d-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itempatent_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/patents
Content-Type: application/json
Content-length: 497

{
  "description": "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
  "displayName": "Inferring User Intent through browsing behaviors",
  "isPending": true,
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```
# <a name="c"></a>[<span data-ttu-id="6831d-171">C#</span><span class="sxs-lookup"><span data-stu-id="6831d-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itempatent-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6831d-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6831d-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itempatent-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6831d-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6831d-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itempatent-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6831d-174">响应</span><span class="sxs-lookup"><span data-stu-id="6831d-174">Response</span></span>
<span data-ttu-id="6831d-175">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6831d-175">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPatent"
}
-->
``` http
HTTP/1.1 201 Created
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
  "description": "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
  "displayName": "Inferring User Intent through browsing behaviors",
  "isPending": true,
  "issuedDate": "Date",
  "issuingAuthority": null,
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```
