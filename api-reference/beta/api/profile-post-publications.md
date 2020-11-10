---
title: 创建出版物
description: 创建新的出版物对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f01b936250b57307713b8156a415c90ab7ce6c42
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976260"
---
# <a name="create-itempublication"></a><span data-ttu-id="da833-103">创建 itemPublication</span><span class="sxs-lookup"><span data-stu-id="da833-103">Create itemPublication</span></span>
<span data-ttu-id="da833-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da833-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da833-105">在用户的[配置文件](../resources/profile.md)中创建新的[itemPublication](../resources/itempublication.md)对象。</span><span class="sxs-lookup"><span data-stu-id="da833-105">Create a new [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="da833-106">权限</span><span class="sxs-lookup"><span data-stu-id="da833-106">Permissions</span></span>

<span data-ttu-id="da833-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da833-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da833-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="da833-109">Permission type</span></span>                        | <span data-ttu-id="da833-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="da833-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="da833-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da833-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="da833-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="da833-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="da833-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da833-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da833-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="da833-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="da833-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="da833-115">Application</span></span>                            | <span data-ttu-id="da833-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da833-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="da833-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da833-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/publications
POST /users/{id | userPrincipalName}/profile/publications
```

## <a name="request-headers"></a><span data-ttu-id="da833-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="da833-118">Request headers</span></span>
|<span data-ttu-id="da833-119">名称</span><span class="sxs-lookup"><span data-stu-id="da833-119">Name</span></span>|<span data-ttu-id="da833-120">说明</span><span class="sxs-lookup"><span data-stu-id="da833-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="da833-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="da833-121">Authorization</span></span>|<span data-ttu-id="da833-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="da833-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="da833-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da833-124">Content-Type</span></span>|<span data-ttu-id="da833-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="da833-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da833-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="da833-127">Request body</span></span>
<span data-ttu-id="da833-128">在请求正文中，提供 [itemPublication](../resources/itempublication.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da833-128">In the request body, supply a JSON representation of the [itemPublication](../resources/itempublication.md) object.</span></span>

<span data-ttu-id="da833-129">下表显示了在用户[配置文件](../resources/profile.md)中创建新的[itemPublication](../resources/itempublication.md)对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="da833-129">The following table shows the properties that are possible to set when creating a new [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="da833-130">属性</span><span class="sxs-lookup"><span data-stu-id="da833-130">Property</span></span>|<span data-ttu-id="da833-131">类型</span><span class="sxs-lookup"><span data-stu-id="da833-131">Type</span></span>|<span data-ttu-id="da833-132">说明</span><span class="sxs-lookup"><span data-stu-id="da833-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da833-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="da833-133">allowedAudiences</span></span>|<span data-ttu-id="da833-134">String</span><span class="sxs-lookup"><span data-stu-id="da833-134">String</span></span>|<span data-ttu-id="da833-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="da833-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="da833-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="da833-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="da833-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="da833-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="da833-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="da833-138">createdBy</span></span>|[<span data-ttu-id="da833-139">identitySet</span><span class="sxs-lookup"><span data-stu-id="da833-139">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="da833-140">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="da833-140">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="da833-141">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="da833-141">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="da833-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da833-142">createdDateTime</span></span>|<span data-ttu-id="da833-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da833-143">DateTimeOffset</span></span>|<span data-ttu-id="da833-144">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="da833-144">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="da833-145">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="da833-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="da833-146">说明</span><span class="sxs-lookup"><span data-stu-id="da833-146">description</span></span>    |<span data-ttu-id="da833-147">String</span><span class="sxs-lookup"><span data-stu-id="da833-147">String</span></span>      |<span data-ttu-id="da833-148">出版物的说明。</span><span class="sxs-lookup"><span data-stu-id="da833-148">Description of the publication.</span></span>                   |
|<span data-ttu-id="da833-149">displayName</span><span class="sxs-lookup"><span data-stu-id="da833-149">displayName</span></span>    |<span data-ttu-id="da833-150">String</span><span class="sxs-lookup"><span data-stu-id="da833-150">String</span></span>      |<span data-ttu-id="da833-151">出版物的标题。</span><span class="sxs-lookup"><span data-stu-id="da833-151">Title of the publication.</span></span>                         |
|<span data-ttu-id="da833-152">id</span><span class="sxs-lookup"><span data-stu-id="da833-152">id</span></span>|<span data-ttu-id="da833-153">String</span><span class="sxs-lookup"><span data-stu-id="da833-153">String</span></span>|<span data-ttu-id="da833-154">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="da833-154">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="da833-155">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="da833-155">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="da833-156">推导</span><span class="sxs-lookup"><span data-stu-id="da833-156">inference</span></span>|[<span data-ttu-id="da833-157">inferenceData</span><span class="sxs-lookup"><span data-stu-id="da833-157">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="da833-158">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="da833-158">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="da833-159">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="da833-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="da833-160">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="da833-160">lastModifiedBy</span></span>|[<span data-ttu-id="da833-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="da833-161">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="da833-162">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="da833-162">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="da833-163">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="da833-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="da833-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da833-164">lastModifiedDateTime</span></span>|<span data-ttu-id="da833-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da833-165">DateTimeOffset</span></span>|<span data-ttu-id="da833-166">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="da833-166">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="da833-167">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="da833-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="da833-168">publishedDate</span><span class="sxs-lookup"><span data-stu-id="da833-168">publishedDate</span></span>  |<span data-ttu-id="da833-169">日期</span><span class="sxs-lookup"><span data-stu-id="da833-169">Date</span></span>        |<span data-ttu-id="da833-170">发布出版物的日期。</span><span class="sxs-lookup"><span data-stu-id="da833-170">The date that the publication was published.</span></span>      |
|<span data-ttu-id="da833-171">发布者</span><span class="sxs-lookup"><span data-stu-id="da833-171">publisher</span></span>      |<span data-ttu-id="da833-172">String</span><span class="sxs-lookup"><span data-stu-id="da833-172">String</span></span>      |<span data-ttu-id="da833-173">出版物的出版物或发布者。</span><span class="sxs-lookup"><span data-stu-id="da833-173">Publication or Publisher for the publication.</span></span>     |
|<span data-ttu-id="da833-174">source</span><span class="sxs-lookup"><span data-stu-id="da833-174">source</span></span>|[<span data-ttu-id="da833-175">personDataSource</span><span class="sxs-lookup"><span data-stu-id="da833-175">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="da833-176">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="da833-176">Where the values originated if synced from another service.</span></span> <span data-ttu-id="da833-177">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="da833-177">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="da833-178">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="da833-178">thumbnailUrl</span></span>   |<span data-ttu-id="da833-179">String</span><span class="sxs-lookup"><span data-stu-id="da833-179">String</span></span>      |<span data-ttu-id="da833-180">URL 引用出版物的缩略图。</span><span class="sxs-lookup"><span data-stu-id="da833-180">URL referencing a thumbnail of the publication.</span></span>   |
|<span data-ttu-id="da833-181">webUrl</span><span class="sxs-lookup"><span data-stu-id="da833-181">webUrl</span></span>         |<span data-ttu-id="da833-182">String</span><span class="sxs-lookup"><span data-stu-id="da833-182">String</span></span>      |<span data-ttu-id="da833-183">引用发布的 URL。</span><span class="sxs-lookup"><span data-stu-id="da833-183">URL referencing the publication.</span></span>                  |

## <a name="response"></a><span data-ttu-id="da833-184">响应</span><span class="sxs-lookup"><span data-stu-id="da833-184">Response</span></span>

<span data-ttu-id="da833-185">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [itemPublication](../resources/itempublication.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da833-185">If successful, this method returns a `201 Created` response code and an [itemPublication](../resources/itempublication.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da833-186">示例</span><span class="sxs-lookup"><span data-stu-id="da833-186">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="da833-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="da833-187">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="da833-188">C#</span><span class="sxs-lookup"><span data-stu-id="da833-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-itempublication-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da833-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da833-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-itempublication-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da833-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da833-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-itempublication-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da833-191">Java</span><span class="sxs-lookup"><span data-stu-id="da833-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-itempublication-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="da833-192">响应</span><span class="sxs-lookup"><span data-stu-id="da833-192">Response</span></span>
<span data-ttu-id="da833-193">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="da833-193">**Note:** The response object shown here might be shortened for readability.</span></span>
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


