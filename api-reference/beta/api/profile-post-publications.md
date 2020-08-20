---
title: 创建出版物
description: 创建新的出版物对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 75692418ae2d54650f4ae6c616c727fab5b040e2
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819729"
---
# <a name="create-itempublication"></a><span data-ttu-id="ea5f3-103">创建 itemPublication</span><span class="sxs-lookup"><span data-stu-id="ea5f3-103">Create itemPublication</span></span>
<span data-ttu-id="ea5f3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea5f3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea5f3-105">在用户的配置文件中创建新的 [itemPublication](../resources/itempublication.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-105">Create a new [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ea5f3-106">权限</span><span class="sxs-lookup"><span data-stu-id="ea5f3-106">Permissions</span></span>

<span data-ttu-id="ea5f3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea5f3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea5f3-109">Permission type</span></span>                        | <span data-ttu-id="ea5f3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea5f3-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="ea5f3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea5f3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea5f3-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea5f3-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ea5f3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea5f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea5f3-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea5f3-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ea5f3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea5f3-115">Application</span></span>                            | <span data-ttu-id="ea5f3-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea5f3-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="ea5f3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea5f3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/publications
POST /users/{id | userPrincipalName}/profile/publications
```

## <a name="request-headers"></a><span data-ttu-id="ea5f3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea5f3-118">Request headers</span></span>
|<span data-ttu-id="ea5f3-119">名称</span><span class="sxs-lookup"><span data-stu-id="ea5f3-119">Name</span></span>|<span data-ttu-id="ea5f3-120">说明</span><span class="sxs-lookup"><span data-stu-id="ea5f3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ea5f3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea5f3-121">Authorization</span></span>|<span data-ttu-id="ea5f3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ea5f3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ea5f3-124">Content-Type</span></span>|<span data-ttu-id="ea5f3-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ea5f3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea5f3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea5f3-127">Request body</span></span>
<span data-ttu-id="ea5f3-128">在请求正文中，提供 [itemPublication](../resources/itempublication.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-128">In the request body, supply a JSON representation of the [itemPublication](../resources/itempublication.md) object.</span></span>

<span data-ttu-id="ea5f3-129">下表显示了在用户的配置文件中创建新 [itemPublication](../resources/itempublication.md) 对象时可能设置 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-129">The following table shows the properties that are possible to set when creating a new [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="ea5f3-130">属性</span><span class="sxs-lookup"><span data-stu-id="ea5f3-130">Property</span></span>|<span data-ttu-id="ea5f3-131">类型</span><span class="sxs-lookup"><span data-stu-id="ea5f3-131">Type</span></span>|<span data-ttu-id="ea5f3-132">说明</span><span class="sxs-lookup"><span data-stu-id="ea5f3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea5f3-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="ea5f3-133">allowedAudiences</span></span>|<span data-ttu-id="ea5f3-134">String</span><span class="sxs-lookup"><span data-stu-id="ea5f3-134">String</span></span>|<span data-ttu-id="ea5f3-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="ea5f3-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="ea5f3-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ea5f3-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="ea5f3-138">createdBy</span></span>|[<span data-ttu-id="ea5f3-139">identitySet</span><span class="sxs-lookup"><span data-stu-id="ea5f3-139">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="ea5f3-140">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-140">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="ea5f3-141">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-141">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ea5f3-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea5f3-142">createdDateTime</span></span>|<span data-ttu-id="ea5f3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea5f3-143">DateTimeOffset</span></span>|<span data-ttu-id="ea5f3-144">提供创建实体时的 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-144">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="ea5f3-145">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ea5f3-146">description</span><span class="sxs-lookup"><span data-stu-id="ea5f3-146">description</span></span>    |<span data-ttu-id="ea5f3-147">String</span><span class="sxs-lookup"><span data-stu-id="ea5f3-147">String</span></span>      |<span data-ttu-id="ea5f3-148">出版物的说明。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-148">Description of the publication.</span></span>                   |
|<span data-ttu-id="ea5f3-149">displayName</span><span class="sxs-lookup"><span data-stu-id="ea5f3-149">displayName</span></span>    |<span data-ttu-id="ea5f3-150">String</span><span class="sxs-lookup"><span data-stu-id="ea5f3-150">String</span></span>      |<span data-ttu-id="ea5f3-151">出版物的标题。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-151">Title of the publication.</span></span>                         |
|<span data-ttu-id="ea5f3-152">id</span><span class="sxs-lookup"><span data-stu-id="ea5f3-152">id</span></span>|<span data-ttu-id="ea5f3-153">String</span><span class="sxs-lookup"><span data-stu-id="ea5f3-153">String</span></span>|<span data-ttu-id="ea5f3-154">单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-154">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="ea5f3-155">从实体 [继承](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="ea5f3-155">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="ea5f3-156">推据</span><span class="sxs-lookup"><span data-stu-id="ea5f3-156">inference</span></span>|[<span data-ttu-id="ea5f3-157">inferenceData</span><span class="sxs-lookup"><span data-stu-id="ea5f3-157">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="ea5f3-158">如果实体受到创建或修改的应用程序的推理，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-158">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="ea5f3-159">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ea5f3-160">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ea5f3-160">lastModifiedBy</span></span>|[<span data-ttu-id="ea5f3-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="ea5f3-161">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="ea5f3-162">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-162">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="ea5f3-163">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ea5f3-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea5f3-164">lastModifiedDateTime</span></span>|<span data-ttu-id="ea5f3-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea5f3-165">DateTimeOffset</span></span>|<span data-ttu-id="ea5f3-166">提供创建实体时的 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-166">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="ea5f3-167">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ea5f3-168">publishedDate</span><span class="sxs-lookup"><span data-stu-id="ea5f3-168">publishedDate</span></span>  |<span data-ttu-id="ea5f3-169">日期</span><span class="sxs-lookup"><span data-stu-id="ea5f3-169">Date</span></span>        |<span data-ttu-id="ea5f3-170">发布出版物的日期。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-170">The date that the publication was published.</span></span>      |
|<span data-ttu-id="ea5f3-171">发布者</span><span class="sxs-lookup"><span data-stu-id="ea5f3-171">publisher</span></span>      |<span data-ttu-id="ea5f3-172">String</span><span class="sxs-lookup"><span data-stu-id="ea5f3-172">String</span></span>      |<span data-ttu-id="ea5f3-173">发布服务器或发布服务器。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-173">Publication or Publisher for the publication.</span></span>     |
|<span data-ttu-id="ea5f3-174">source</span><span class="sxs-lookup"><span data-stu-id="ea5f3-174">source</span></span>|[<span data-ttu-id="ea5f3-175">personDataSource</span><span class="sxs-lookup"><span data-stu-id="ea5f3-175">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="ea5f3-176">同步到其他服务时从哪个位置发送值。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-176">Where the values originated if synced from another service.</span></span> <span data-ttu-id="ea5f3-177">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-177">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ea5f3-178">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="ea5f3-178">thumbnailUrl</span></span>   |<span data-ttu-id="ea5f3-179">String</span><span class="sxs-lookup"><span data-stu-id="ea5f3-179">String</span></span>      |<span data-ttu-id="ea5f3-180">引用出版物缩略图的 URL。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-180">URL referencing a thumbnail of the publication.</span></span>   |
|<span data-ttu-id="ea5f3-181">webUrl</span><span class="sxs-lookup"><span data-stu-id="ea5f3-181">webUrl</span></span>         |<span data-ttu-id="ea5f3-182">String</span><span class="sxs-lookup"><span data-stu-id="ea5f3-182">String</span></span>      |<span data-ttu-id="ea5f3-183">引用出版物的 URL。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-183">URL referencing the publication.</span></span>                  |

## <a name="response"></a><span data-ttu-id="ea5f3-184">响应</span><span class="sxs-lookup"><span data-stu-id="ea5f3-184">Response</span></span>

<span data-ttu-id="ea5f3-185">如果成功，此方法在 `201 Created` 响应正文中 [返回响应代码和 itemPublication](../resources/itempublication.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-185">If successful, this method returns a `201 Created` response code and an [itemPublication](../resources/itempublication.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ea5f3-186">示例</span><span class="sxs-lookup"><span data-stu-id="ea5f3-186">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="ea5f3-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea5f3-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_itemPublication_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/publications
Content-Type: application/json
Content-length: 497

{
  "description": "One persons journey to the top of the branding management field.",
  "displayName": "Got Brands? The story of Innocenty Popov and his journey to the top.",
  "publishedDate": "Date",
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
# <a name="c"></a>[<span data-ttu-id="ea5f3-188">C#</span><span class="sxs-lookup"><span data-stu-id="ea5f3-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itempublication-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea5f3-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea5f3-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itempublication-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea5f3-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea5f3-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itempublication-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ea5f3-191">响应</span><span class="sxs-lookup"><span data-stu-id="ea5f3-191">Response</span></span>
<span data-ttu-id="ea5f3-192">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ea5f3-192">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPublication"
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
  "description": "One persons journey to the top of the branding management field.",
  "displayName": "Got Brands? The story of Innocenty Popov and his journey to the top.",
  "publishedDate": "Date",
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
