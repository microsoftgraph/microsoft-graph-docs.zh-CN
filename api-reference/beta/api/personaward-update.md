---
title: 更新 personAward
description: 更新 personAward 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a33959dda6b8316f855ea03878756aa6b9bd5ce4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812961"
---
# <a name="update-personaward"></a><span data-ttu-id="c4045-103">更新 personAward</span><span class="sxs-lookup"><span data-stu-id="c4045-103">Update personAward</span></span>

<span data-ttu-id="c4045-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4045-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4045-105">从用户的[配置文件](../resources/profile.md)中更新[personAward](../resources/personAward.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c4045-105">Update the properties of a [personAward](../resources/personAward.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4045-106">权限</span><span class="sxs-lookup"><span data-stu-id="c4045-106">Permissions</span></span>

<span data-ttu-id="c4045-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4045-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4045-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4045-109">Permission type</span></span>                        | <span data-ttu-id="c4045-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4045-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="c4045-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4045-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4045-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="c4045-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="c4045-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4045-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4045-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="c4045-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="c4045-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4045-115">Application</span></span>                            | <span data-ttu-id="c4045-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4045-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="c4045-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4045-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/awards/{id}
PATCH /users/{id | userPrincipalName}/profile/awards/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c4045-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4045-118">Request headers</span></span>
|<span data-ttu-id="c4045-119">名称</span><span class="sxs-lookup"><span data-stu-id="c4045-119">Name</span></span>|<span data-ttu-id="c4045-120">说明</span><span class="sxs-lookup"><span data-stu-id="c4045-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c4045-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4045-121">Authorization</span></span>|<span data-ttu-id="c4045-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4045-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c4045-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4045-124">Content-Type</span></span>|<span data-ttu-id="c4045-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c4045-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4045-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4045-127">Request body</span></span>

<span data-ttu-id="c4045-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="c4045-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c4045-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="c4045-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c4045-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c4045-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="c4045-131">属性</span><span class="sxs-lookup"><span data-stu-id="c4045-131">Property</span></span>|<span data-ttu-id="c4045-132">类型</span><span class="sxs-lookup"><span data-stu-id="c4045-132">Type</span></span>|<span data-ttu-id="c4045-133">说明</span><span class="sxs-lookup"><span data-stu-id="c4045-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4045-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="c4045-134">allowedAudiences</span></span>|<span data-ttu-id="c4045-135">String</span><span class="sxs-lookup"><span data-stu-id="c4045-135">String</span></span>|<span data-ttu-id="c4045-136">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="c4045-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="c4045-137">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c4045-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="c4045-138">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c4045-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c4045-139">description</span><span class="sxs-lookup"><span data-stu-id="c4045-139">description</span></span>|<span data-ttu-id="c4045-140">String</span><span class="sxs-lookup"><span data-stu-id="c4045-140">String</span></span>|<span data-ttu-id="c4045-141">奖励或荣誉的 Descpription。</span><span class="sxs-lookup"><span data-stu-id="c4045-141">Descpription of the award or honor.</span></span> |
|<span data-ttu-id="c4045-142">displayName</span><span class="sxs-lookup"><span data-stu-id="c4045-142">displayName</span></span>|<span data-ttu-id="c4045-143">String</span><span class="sxs-lookup"><span data-stu-id="c4045-143">String</span></span>|<span data-ttu-id="c4045-144">获奖或荣誉的名称。</span><span class="sxs-lookup"><span data-stu-id="c4045-144">Name of the award or honor.</span></span> |
|<span data-ttu-id="c4045-145">推导</span><span class="sxs-lookup"><span data-stu-id="c4045-145">inference</span></span>|[<span data-ttu-id="c4045-146">inferenceData</span><span class="sxs-lookup"><span data-stu-id="c4045-146">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="c4045-147">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="c4045-147">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="c4045-148">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c4045-148">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="c4045-149">issuedDate</span><span class="sxs-lookup"><span data-stu-id="c4045-149">issuedDate</span></span>|<span data-ttu-id="c4045-150">日期</span><span class="sxs-lookup"><span data-stu-id="c4045-150">Date</span></span>|<span data-ttu-id="c4045-151">授予获奖或荣誉的日期。</span><span class="sxs-lookup"><span data-stu-id="c4045-151">The date that the award or honor was granted.</span></span> |
|<span data-ttu-id="c4045-152">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="c4045-152">issuingAuthority</span></span>|<span data-ttu-id="c4045-153">String</span><span class="sxs-lookup"><span data-stu-id="c4045-153">String</span></span>|<span data-ttu-id="c4045-154">授予奖项的证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="c4045-154">Authority which granted the award or honor.</span></span>  |
|<span data-ttu-id="c4045-155">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="c4045-155">thumbnailUrl</span></span>|<span data-ttu-id="c4045-156">String</span><span class="sxs-lookup"><span data-stu-id="c4045-156">String</span></span>|<span data-ttu-id="c4045-157">URL 引用获奖或荣誉的缩略图。</span><span class="sxs-lookup"><span data-stu-id="c4045-157">URL referencing a thumbnail of the award or honor.</span></span>  |
|<span data-ttu-id="c4045-158">webUrl</span><span class="sxs-lookup"><span data-stu-id="c4045-158">webUrl</span></span>|<span data-ttu-id="c4045-159">String</span><span class="sxs-lookup"><span data-stu-id="c4045-159">String</span></span>|<span data-ttu-id="c4045-160">引用奖项或荣誉的 URL。</span><span class="sxs-lookup"><span data-stu-id="c4045-160">URL referencing the award or honor.</span></span> |

## <a name="response"></a><span data-ttu-id="c4045-161">响应</span><span class="sxs-lookup"><span data-stu-id="c4045-161">Response</span></span>

<span data-ttu-id="c4045-162">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [personAward](../resources/personaward.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c4045-162">If successful, this method returns a `200 OK` response code and an updated [personAward](../resources/personaward.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4045-163">示例</span><span class="sxs-lookup"><span data-stu-id="c4045-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4045-164">请求</span><span class="sxs-lookup"><span data-stu-id="c4045-164">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="c4045-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4045-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personaward"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/user/{userId}/profile/awards/{personAwardId}
Content-Type: application/json
Content-length: 497

{
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg"
}
```
# <a name="c"></a>[<span data-ttu-id="c4045-166">C#</span><span class="sxs-lookup"><span data-stu-id="c4045-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4045-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4045-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4045-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4045-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c4045-169">响应</span><span class="sxs-lookup"><span data-stu-id="c4045-169">Response</span></span>
<span data-ttu-id="c4045-170">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c4045-170">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAward"
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
  "description": "Lifetime Achievement award from the International Association of Branding Managers",
  "displayName": "Lifetime Achievement Award For Excellence in Branding",
  "issuedDate": "Date",
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
