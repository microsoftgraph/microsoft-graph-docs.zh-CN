---
title: 创建出版物
description: 创建新的出版物对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5ae8e81167828ee644e14c4ba92216c2aba43160
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812927"
---
# <a name="create-itempublication"></a><span data-ttu-id="a6fb0-103">创建 itemPublication</span><span class="sxs-lookup"><span data-stu-id="a6fb0-103">Create itemPublication</span></span>
<span data-ttu-id="a6fb0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6fb0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a6fb0-105">在用户的[配置文件](../resources/profile.md)中创建新的[itemPublication](../resources/itempublication.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-105">Create a new [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a6fb0-106">权限</span><span class="sxs-lookup"><span data-stu-id="a6fb0-106">Permissions</span></span>

<span data-ttu-id="a6fb0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6fb0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6fb0-109">Permission type</span></span>                        | <span data-ttu-id="a6fb0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a6fb0-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="a6fb0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6fb0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6fb0-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a6fb0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6fb0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6fb0-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a6fb0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6fb0-115">Application</span></span>                            | <span data-ttu-id="a6fb0-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6fb0-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="a6fb0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6fb0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/publications
POST /users/{id | userPrincipalName}/profile/publications
```

## <a name="request-headers"></a><span data-ttu-id="a6fb0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6fb0-118">Request headers</span></span>
|<span data-ttu-id="a6fb0-119">名称</span><span class="sxs-lookup"><span data-stu-id="a6fb0-119">Name</span></span>|<span data-ttu-id="a6fb0-120">说明</span><span class="sxs-lookup"><span data-stu-id="a6fb0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a6fb0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6fb0-121">Authorization</span></span>|<span data-ttu-id="a6fb0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a6fb0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6fb0-124">Content-Type</span></span>|<span data-ttu-id="a6fb0-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a6fb0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6fb0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6fb0-127">Request body</span></span>
<span data-ttu-id="a6fb0-128">在请求正文中，提供 [itemPublication](../resources/itempublication.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-128">In the request body, supply a JSON representation of the [itemPublication](../resources/itempublication.md) object.</span></span>

<span data-ttu-id="a6fb0-129">下表显示了在用户[配置文件](../resources/profile.md)中创建新的[itemPublication](../resources/itempublication.md)对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-129">The following table shows the properties that are possible to set when creating a new [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="a6fb0-130">属性</span><span class="sxs-lookup"><span data-stu-id="a6fb0-130">Property</span></span>|<span data-ttu-id="a6fb0-131">类型</span><span class="sxs-lookup"><span data-stu-id="a6fb0-131">Type</span></span>|<span data-ttu-id="a6fb0-132">说明</span><span class="sxs-lookup"><span data-stu-id="a6fb0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6fb0-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="a6fb0-133">allowedAudiences</span></span>|<span data-ttu-id="a6fb0-134">String</span><span class="sxs-lookup"><span data-stu-id="a6fb0-134">String</span></span>|<span data-ttu-id="a6fb0-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="a6fb0-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="a6fb0-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a6fb0-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="a6fb0-138">createdBy</span></span>|[<span data-ttu-id="a6fb0-139">identitySet</span><span class="sxs-lookup"><span data-stu-id="a6fb0-139">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="a6fb0-140">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-140">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="a6fb0-141">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-141">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a6fb0-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6fb0-142">createdDateTime</span></span>|<span data-ttu-id="a6fb0-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6fb0-143">DateTimeOffset</span></span>|<span data-ttu-id="a6fb0-144">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-144">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="a6fb0-145">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a6fb0-146">description</span><span class="sxs-lookup"><span data-stu-id="a6fb0-146">description</span></span>    |<span data-ttu-id="a6fb0-147">String</span><span class="sxs-lookup"><span data-stu-id="a6fb0-147">String</span></span>      |<span data-ttu-id="a6fb0-148">出版物的说明。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-148">Description of the publication.</span></span>                   |
|<span data-ttu-id="a6fb0-149">displayName</span><span class="sxs-lookup"><span data-stu-id="a6fb0-149">displayName</span></span>    |<span data-ttu-id="a6fb0-150">String</span><span class="sxs-lookup"><span data-stu-id="a6fb0-150">String</span></span>      |<span data-ttu-id="a6fb0-151">出版物的标题。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-151">Title of the publication.</span></span>                         |
|<span data-ttu-id="a6fb0-152">id</span><span class="sxs-lookup"><span data-stu-id="a6fb0-152">id</span></span>|<span data-ttu-id="a6fb0-153">String</span><span class="sxs-lookup"><span data-stu-id="a6fb0-153">String</span></span>|<span data-ttu-id="a6fb0-154">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-154">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="a6fb0-155">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="a6fb0-155">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="a6fb0-156">推导</span><span class="sxs-lookup"><span data-stu-id="a6fb0-156">inference</span></span>|[<span data-ttu-id="a6fb0-157">inferenceData</span><span class="sxs-lookup"><span data-stu-id="a6fb0-157">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="a6fb0-158">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-158">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="a6fb0-159">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a6fb0-160">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a6fb0-160">lastModifiedBy</span></span>|[<span data-ttu-id="a6fb0-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="a6fb0-161">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="a6fb0-162">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-162">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="a6fb0-163">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a6fb0-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6fb0-164">lastModifiedDateTime</span></span>|<span data-ttu-id="a6fb0-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6fb0-165">DateTimeOffset</span></span>|<span data-ttu-id="a6fb0-166">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-166">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="a6fb0-167">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a6fb0-168">publishedDate</span><span class="sxs-lookup"><span data-stu-id="a6fb0-168">publishedDate</span></span>  |<span data-ttu-id="a6fb0-169">日期</span><span class="sxs-lookup"><span data-stu-id="a6fb0-169">Date</span></span>        |<span data-ttu-id="a6fb0-170">发布出版物的日期。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-170">The date that the publication was published.</span></span>      |
|<span data-ttu-id="a6fb0-171">发布者</span><span class="sxs-lookup"><span data-stu-id="a6fb0-171">publisher</span></span>      |<span data-ttu-id="a6fb0-172">String</span><span class="sxs-lookup"><span data-stu-id="a6fb0-172">String</span></span>      |<span data-ttu-id="a6fb0-173">出版物的出版物或发布者。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-173">Publication or Publisher for the publication.</span></span>     |
|<span data-ttu-id="a6fb0-174">source</span><span class="sxs-lookup"><span data-stu-id="a6fb0-174">source</span></span>|[<span data-ttu-id="a6fb0-175">personDataSource</span><span class="sxs-lookup"><span data-stu-id="a6fb0-175">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="a6fb0-176">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-176">Where the values originated if synced from another service.</span></span> <span data-ttu-id="a6fb0-177">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-177">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a6fb0-178">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="a6fb0-178">thumbnailUrl</span></span>   |<span data-ttu-id="a6fb0-179">String</span><span class="sxs-lookup"><span data-stu-id="a6fb0-179">String</span></span>      |<span data-ttu-id="a6fb0-180">URL 引用出版物的缩略图。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-180">URL referencing a thumbnail of the publication.</span></span>   |
|<span data-ttu-id="a6fb0-181">webUrl</span><span class="sxs-lookup"><span data-stu-id="a6fb0-181">webUrl</span></span>         |<span data-ttu-id="a6fb0-182">String</span><span class="sxs-lookup"><span data-stu-id="a6fb0-182">String</span></span>      |<span data-ttu-id="a6fb0-183">引用发布的 URL。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-183">URL referencing the publication.</span></span>                  |

## <a name="response"></a><span data-ttu-id="a6fb0-184">响应</span><span class="sxs-lookup"><span data-stu-id="a6fb0-184">Response</span></span>

<span data-ttu-id="a6fb0-185">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [itemPublication](../resources/itempublication.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-185">If successful, this method returns a `201 Created` response code and an [itemPublication](../resources/itempublication.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a6fb0-186">示例</span><span class="sxs-lookup"><span data-stu-id="a6fb0-186">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="a6fb0-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6fb0-187">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a6fb0-188">C#</span><span class="sxs-lookup"><span data-stu-id="a6fb0-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6fb0-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6fb0-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6fb0-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6fb0-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a6fb0-191">响应</span><span class="sxs-lookup"><span data-stu-id="a6fb0-191">Response</span></span>
<span data-ttu-id="a6fb0-192">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a6fb0-192">**Note:** The response object shown here might be shortened for readability.</span></span>
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
