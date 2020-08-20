---
title: 创建奖励
description: 创建新的奖励对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b40795f5961bfe47388b01abaf1ce39725a8d113
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819561"
---
# <a name="create-personaward"></a><span data-ttu-id="8c2be-103">创建 personAward</span><span class="sxs-lookup"><span data-stu-id="8c2be-103">Create personAward</span></span>

<span data-ttu-id="8c2be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c2be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c2be-105">在 [用户的配置文件中创建新的 personAward](../resources/personaward.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="8c2be-105">Create a new [personAward](../resources/personaward.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c2be-106">权限</span><span class="sxs-lookup"><span data-stu-id="8c2be-106">Permissions</span></span>

<span data-ttu-id="8c2be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c2be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c2be-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c2be-109">Permission type</span></span>                        | <span data-ttu-id="8c2be-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c2be-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="8c2be-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c2be-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c2be-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c2be-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="8c2be-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c2be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c2be-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c2be-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="8c2be-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c2be-115">Application</span></span>                            | <span data-ttu-id="8c2be-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c2be-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="8c2be-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c2be-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/awards
POST /users/{id | userPrincipalName}/profile/awards
```

## <a name="request-headers"></a><span data-ttu-id="8c2be-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c2be-118">Request headers</span></span>
|<span data-ttu-id="8c2be-119">名称</span><span class="sxs-lookup"><span data-stu-id="8c2be-119">Name</span></span>|<span data-ttu-id="8c2be-120">说明</span><span class="sxs-lookup"><span data-stu-id="8c2be-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8c2be-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c2be-121">Authorization</span></span>|<span data-ttu-id="8c2be-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8c2be-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8c2be-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c2be-124">Content-Type</span></span>|<span data-ttu-id="8c2be-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8c2be-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c2be-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c2be-127">Request body</span></span>
<span data-ttu-id="8c2be-128">在请求正文中，提供 [personAward 对象的](../resources/personaward.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c2be-128">In the request body, supply a JSON representation of the [personAward](../resources/personaward.md) object.</span></span>

<span data-ttu-id="8c2be-129">下表显示了在用户的配置文件中创建新 [personAward](../resources/personaward.md) 对象时可能设置 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="8c2be-129">The following table shows the properties that are possible to set when creating a new [personAward](../resources/personaward.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="8c2be-130">属性</span><span class="sxs-lookup"><span data-stu-id="8c2be-130">Property</span></span>|<span data-ttu-id="8c2be-131">类型</span><span class="sxs-lookup"><span data-stu-id="8c2be-131">Type</span></span>|<span data-ttu-id="8c2be-132">说明</span><span class="sxs-lookup"><span data-stu-id="8c2be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c2be-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="8c2be-133">allowedAudiences</span></span>|<span data-ttu-id="8c2be-134">String</span><span class="sxs-lookup"><span data-stu-id="8c2be-134">String</span></span>|<span data-ttu-id="8c2be-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="8c2be-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="8c2be-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="8c2be-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="8c2be-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8c2be-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8c2be-138">description</span><span class="sxs-lookup"><span data-stu-id="8c2be-138">description</span></span>|<span data-ttu-id="8c2be-139">String</span><span class="sxs-lookup"><span data-stu-id="8c2be-139">String</span></span>|<span data-ttu-id="8c2be-140">奖励或移动者的说明。</span><span class="sxs-lookup"><span data-stu-id="8c2be-140">Descpription of the award or honor.</span></span> |
|<span data-ttu-id="8c2be-141">displayName</span><span class="sxs-lookup"><span data-stu-id="8c2be-141">displayName</span></span>|<span data-ttu-id="8c2be-142">String</span><span class="sxs-lookup"><span data-stu-id="8c2be-142">String</span></span>|<span data-ttu-id="8c2be-143">奖励或移的姓名。</span><span class="sxs-lookup"><span data-stu-id="8c2be-143">Name of the award or honor.</span></span> |
|<span data-ttu-id="8c2be-144">推据</span><span class="sxs-lookup"><span data-stu-id="8c2be-144">inference</span></span>|[<span data-ttu-id="8c2be-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="8c2be-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="8c2be-146">如果实体受到创建或修改的应用程序的推理，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="8c2be-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="8c2be-147">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="8c2be-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8c2be-148">issuedDate</span><span class="sxs-lookup"><span data-stu-id="8c2be-148">issuedDate</span></span>|<span data-ttu-id="8c2be-149">日期</span><span class="sxs-lookup"><span data-stu-id="8c2be-149">Date</span></span>|<span data-ttu-id="8c2be-150">获得的奖励或手的日期。</span><span class="sxs-lookup"><span data-stu-id="8c2be-150">The date that the award or honor was granted.</span></span> |
|<span data-ttu-id="8c2be-151">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="8c2be-151">issuingAuthority</span></span>|<span data-ttu-id="8c2be-152">String</span><span class="sxs-lookup"><span data-stu-id="8c2be-152">String</span></span>|<span data-ttu-id="8c2be-153">向其授予或移访问者的授权。</span><span class="sxs-lookup"><span data-stu-id="8c2be-153">Authority which granted the award or honor.</span></span>  |
|<span data-ttu-id="8c2be-154">source</span><span class="sxs-lookup"><span data-stu-id="8c2be-154">source</span></span>|[<span data-ttu-id="8c2be-155">personDataSource</span><span class="sxs-lookup"><span data-stu-id="8c2be-155">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="8c2be-156">同步到其他服务时从哪个位置发送值。</span><span class="sxs-lookup"><span data-stu-id="8c2be-156">Where the values originated if synced from another service.</span></span> <span data-ttu-id="8c2be-157">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="8c2be-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="8c2be-158">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="8c2be-158">thumbnailUrl</span></span>|<span data-ttu-id="8c2be-159">String</span><span class="sxs-lookup"><span data-stu-id="8c2be-159">String</span></span>|<span data-ttu-id="8c2be-160">URL，用于引用奖励或更深的缩略图。</span><span class="sxs-lookup"><span data-stu-id="8c2be-160">URL referencing a thumbnail of the award or honor.</span></span>  |
|<span data-ttu-id="8c2be-161">webUrl</span><span class="sxs-lookup"><span data-stu-id="8c2be-161">webUrl</span></span>|<span data-ttu-id="8c2be-162">String</span><span class="sxs-lookup"><span data-stu-id="8c2be-162">String</span></span>|<span data-ttu-id="8c2be-163">引用奖励或移入者的 URL。</span><span class="sxs-lookup"><span data-stu-id="8c2be-163">URL referencing the award or honor.</span></span> |

## <a name="response"></a><span data-ttu-id="8c2be-164">响应</span><span class="sxs-lookup"><span data-stu-id="8c2be-164">Response</span></span>

<span data-ttu-id="8c2be-165">如果成功，此方法在响应 `201 Created` 正文中返回响应代码 [和 personAward](../resources/personaward.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8c2be-165">If successful, this method returns a `201 Created` response code and an [personAward](../resources/personaward.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c2be-166">示例</span><span class="sxs-lookup"><span data-stu-id="8c2be-166">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="8c2be-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c2be-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personaward_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/awards
Content-Type: application/json
Content-length: 497

{
  "description": "Lifetime Achievement award from the International Association of Branding Managers",
  "displayName": "Lifetime Achievement Award For Excellence in Branding",
  "issuedDate": "Date",
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
# <a name="c"></a>[<span data-ttu-id="8c2be-168">C#</span><span class="sxs-lookup"><span data-stu-id="8c2be-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personaward-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c2be-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c2be-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personaward-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c2be-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c2be-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personaward-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8c2be-171">响应</span><span class="sxs-lookup"><span data-stu-id="8c2be-171">Response</span></span>
<span data-ttu-id="8c2be-172">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8c2be-172">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAward"
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
  "description": "Lifetime Achievement award from the International Association of Branding Managers",
  "displayName": "Lifetime Achievement Award For Excellence in Branding",
  "issuedDate": "Date",
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
