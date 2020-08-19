---
title: 更新 itemPublication
description: 更新 itemPublication 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 236be40542e200613d496f071f178f520e0ad422
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812939"
---
# <a name="update-itempublication"></a><span data-ttu-id="2cb39-103">更新 itemPublication</span><span class="sxs-lookup"><span data-stu-id="2cb39-103">Update itemPublication</span></span>

<span data-ttu-id="2cb39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cb39-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2cb39-105">更新用户的[配置文件](../resources/profile.md)中的[itemPublication](../resources/itempublication.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2cb39-105">Update the properties of an [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2cb39-106">权限</span><span class="sxs-lookup"><span data-stu-id="2cb39-106">Permissions</span></span>

<span data-ttu-id="2cb39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2cb39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2cb39-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2cb39-109">Permission type</span></span>                        | <span data-ttu-id="2cb39-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2cb39-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="2cb39-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2cb39-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2cb39-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="2cb39-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="2cb39-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2cb39-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cb39-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="2cb39-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="2cb39-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2cb39-115">Application</span></span>                            | <span data-ttu-id="2cb39-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cb39-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="2cb39-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2cb39-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/publications/{id}
PATCH /users/{id | userPrincipalName}/profile/publications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2cb39-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2cb39-118">Request headers</span></span>
|<span data-ttu-id="2cb39-119">名称</span><span class="sxs-lookup"><span data-stu-id="2cb39-119">Name</span></span>|<span data-ttu-id="2cb39-120">说明</span><span class="sxs-lookup"><span data-stu-id="2cb39-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2cb39-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cb39-121">Authorization</span></span>|<span data-ttu-id="2cb39-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2cb39-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2cb39-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2cb39-124">Content-Type</span></span>|<span data-ttu-id="2cb39-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2cb39-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cb39-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2cb39-127">Request body</span></span>

<span data-ttu-id="2cb39-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="2cb39-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2cb39-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="2cb39-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2cb39-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="2cb39-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="2cb39-131">属性</span><span class="sxs-lookup"><span data-stu-id="2cb39-131">Property</span></span>|<span data-ttu-id="2cb39-132">类型</span><span class="sxs-lookup"><span data-stu-id="2cb39-132">Type</span></span>|<span data-ttu-id="2cb39-133">说明</span><span class="sxs-lookup"><span data-stu-id="2cb39-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cb39-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="2cb39-134">allowedAudiences</span></span>|<span data-ttu-id="2cb39-135">String</span><span class="sxs-lookup"><span data-stu-id="2cb39-135">String</span></span>|<span data-ttu-id="2cb39-136">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="2cb39-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="2cb39-137">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="2cb39-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="2cb39-138">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2cb39-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2cb39-139">description</span><span class="sxs-lookup"><span data-stu-id="2cb39-139">description</span></span>    |<span data-ttu-id="2cb39-140">String</span><span class="sxs-lookup"><span data-stu-id="2cb39-140">String</span></span>      |<span data-ttu-id="2cb39-141">出版物的说明。</span><span class="sxs-lookup"><span data-stu-id="2cb39-141">Description of the publication.</span></span>                   |
|<span data-ttu-id="2cb39-142">displayName</span><span class="sxs-lookup"><span data-stu-id="2cb39-142">displayName</span></span>    |<span data-ttu-id="2cb39-143">String</span><span class="sxs-lookup"><span data-stu-id="2cb39-143">String</span></span>      |<span data-ttu-id="2cb39-144">出版物的标题。</span><span class="sxs-lookup"><span data-stu-id="2cb39-144">Title of the publication.</span></span>                         |
|<span data-ttu-id="2cb39-145">推导</span><span class="sxs-lookup"><span data-stu-id="2cb39-145">inference</span></span>|[<span data-ttu-id="2cb39-146">inferenceData</span><span class="sxs-lookup"><span data-stu-id="2cb39-146">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="2cb39-147">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="2cb39-147">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="2cb39-148">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="2cb39-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="2cb39-149">publishedDate</span><span class="sxs-lookup"><span data-stu-id="2cb39-149">publishedDate</span></span>  |<span data-ttu-id="2cb39-150">日期</span><span class="sxs-lookup"><span data-stu-id="2cb39-150">Date</span></span>        |<span data-ttu-id="2cb39-151">发布出版物的日期。</span><span class="sxs-lookup"><span data-stu-id="2cb39-151">The date that the publication was published.</span></span>      |
|<span data-ttu-id="2cb39-152">发布者</span><span class="sxs-lookup"><span data-stu-id="2cb39-152">publisher</span></span>      |<span data-ttu-id="2cb39-153">String</span><span class="sxs-lookup"><span data-stu-id="2cb39-153">String</span></span>      |<span data-ttu-id="2cb39-154">出版物的出版物或发布者。</span><span class="sxs-lookup"><span data-stu-id="2cb39-154">Publication or Publisher for the publication.</span></span>     |
|<span data-ttu-id="2cb39-155">source</span><span class="sxs-lookup"><span data-stu-id="2cb39-155">source</span></span>|[<span data-ttu-id="2cb39-156">personDataSource</span><span class="sxs-lookup"><span data-stu-id="2cb39-156">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="2cb39-157">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="2cb39-157">Where the values originated if synced from another service.</span></span> <span data-ttu-id="2cb39-158">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="2cb39-158">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="2cb39-159">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="2cb39-159">thumbnailUrl</span></span>   |<span data-ttu-id="2cb39-160">String</span><span class="sxs-lookup"><span data-stu-id="2cb39-160">String</span></span>      |<span data-ttu-id="2cb39-161">URL 引用出版物的缩略图。</span><span class="sxs-lookup"><span data-stu-id="2cb39-161">URL referencing a thumbnail of the publication.</span></span>   |
|<span data-ttu-id="2cb39-162">webUrl</span><span class="sxs-lookup"><span data-stu-id="2cb39-162">webUrl</span></span>         |<span data-ttu-id="2cb39-163">String</span><span class="sxs-lookup"><span data-stu-id="2cb39-163">String</span></span>      |<span data-ttu-id="2cb39-164">引用发布的 URL。</span><span class="sxs-lookup"><span data-stu-id="2cb39-164">URL referencing the publication.</span></span>                  |

## <a name="response"></a><span data-ttu-id="2cb39-165">响应</span><span class="sxs-lookup"><span data-stu-id="2cb39-165">Response</span></span>

<span data-ttu-id="2cb39-166">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [itemPublication](../resources/itemPublication.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2cb39-166">If successful, this method returns a `200 OK` response code and an updated [itemPublication](../resources/itemPublication.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2cb39-167">示例</span><span class="sxs-lookup"><span data-stu-id="2cb39-167">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2cb39-168">请求</span><span class="sxs-lookup"><span data-stu-id="2cb39-168">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="2cb39-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="2cb39-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itemPublication"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/user/{userId}/profile/publications/{id}
Content-Type: application/json
Content-length: 497

{
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
}
```
# <a name="c"></a>[<span data-ttu-id="2cb39-170">C#</span><span class="sxs-lookup"><span data-stu-id="2cb39-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2cb39-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2cb39-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2cb39-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2cb39-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2cb39-173">响应</span><span class="sxs-lookup"><span data-stu-id="2cb39-173">Response</span></span>
<span data-ttu-id="2cb39-174">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2cb39-174">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPublication"
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
  "source": null,
  "description": "One persons journey to the top of the branding management field.",
  "displayName": "Got Brands? The story of Innocenty Popov and his journey to the top.",
  "publishedDate": "Date",
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
