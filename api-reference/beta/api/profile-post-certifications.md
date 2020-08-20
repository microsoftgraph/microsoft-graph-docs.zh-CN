---
title: 创建认证
description: 创建新的认证对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 662b25f18734ed47cd2fb89fce90d04957429830
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820201"
---
# <a name="create-personcertification"></a><span data-ttu-id="fe750-103">创建 personCertification</span><span class="sxs-lookup"><span data-stu-id="fe750-103">Create personCertification</span></span>
<span data-ttu-id="fe750-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe750-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe750-105">在用户配置文件 [中创建新的 personCertification](../resources/personcertification.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="fe750-105">Create a new [personCertification](../resources/personcertification.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe750-106">权限</span><span class="sxs-lookup"><span data-stu-id="fe750-106">Permissions</span></span>

<span data-ttu-id="fe750-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe750-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fe750-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe750-109">Permission type</span></span>                        | <span data-ttu-id="fe750-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe750-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="fe750-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe750-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe750-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe750-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="fe750-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe750-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe750-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe750-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="fe750-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe750-115">Application</span></span>                            | <span data-ttu-id="fe750-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe750-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="fe750-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe750-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/certifications
POST /users/{id | userPrincipalName}/profile/certifications
```

## <a name="request-headers"></a><span data-ttu-id="fe750-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe750-118">Request headers</span></span>
|<span data-ttu-id="fe750-119">名称</span><span class="sxs-lookup"><span data-stu-id="fe750-119">Name</span></span>|<span data-ttu-id="fe750-120">说明</span><span class="sxs-lookup"><span data-stu-id="fe750-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fe750-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe750-121">Authorization</span></span>|<span data-ttu-id="fe750-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe750-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fe750-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe750-124">Content-Type</span></span>|<span data-ttu-id="fe750-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="fe750-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe750-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe750-127">Request body</span></span>
<span data-ttu-id="fe750-128">在请求正文中，提供 [personCertification](../resources/personcertification.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe750-128">In the request body, supply a JSON representation of the [personCertification](../resources/personcertification.md) object.</span></span>

<span data-ttu-id="fe750-129">下表显示了在用户的配置文件中创建新 [personCertification](../resources/personcertification.md) 对象时可能设置 [的属性](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="fe750-129">The following table shows the properties that are possible to set when creating a new [personCertification](../resources/personcertification.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="fe750-130">属性</span><span class="sxs-lookup"><span data-stu-id="fe750-130">Property</span></span>|<span data-ttu-id="fe750-131">类型</span><span class="sxs-lookup"><span data-stu-id="fe750-131">Type</span></span>|<span data-ttu-id="fe750-132">说明</span><span class="sxs-lookup"><span data-stu-id="fe750-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe750-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="fe750-133">allowedAudiences</span></span>|<span data-ttu-id="fe750-134">String</span><span class="sxs-lookup"><span data-stu-id="fe750-134">String</span></span>|<span data-ttu-id="fe750-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="fe750-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="fe750-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="fe750-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="fe750-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="fe750-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="fe750-138">certificationId</span><span class="sxs-lookup"><span data-stu-id="fe750-138">certificationId</span></span>  |<span data-ttu-id="fe750-139">String</span><span class="sxs-lookup"><span data-stu-id="fe750-139">String</span></span>      |<span data-ttu-id="fe750-140">证书的可引用标识符。</span><span class="sxs-lookup"><span data-stu-id="fe750-140">The referenceable identifier for the certification.</span></span> |
|<span data-ttu-id="fe750-141">description</span><span class="sxs-lookup"><span data-stu-id="fe750-141">description</span></span>      |<span data-ttu-id="fe750-142">String</span><span class="sxs-lookup"><span data-stu-id="fe750-142">String</span></span>      |<span data-ttu-id="fe750-143">认证的说明。</span><span class="sxs-lookup"><span data-stu-id="fe750-143">Description of the certification.</span></span>                   |
|<span data-ttu-id="fe750-144">displayName</span><span class="sxs-lookup"><span data-stu-id="fe750-144">displayName</span></span>      |<span data-ttu-id="fe750-145">String</span><span class="sxs-lookup"><span data-stu-id="fe750-145">String</span></span>      |<span data-ttu-id="fe750-146">认证的标题。</span><span class="sxs-lookup"><span data-stu-id="fe750-146">Title of the certification.</span></span>                         |
|<span data-ttu-id="fe750-147">endDate</span><span class="sxs-lookup"><span data-stu-id="fe750-147">endDate</span></span>          |<span data-ttu-id="fe750-148">日期</span><span class="sxs-lookup"><span data-stu-id="fe750-148">Date</span></span>        |<span data-ttu-id="fe750-149">认证的到期日期。</span><span class="sxs-lookup"><span data-stu-id="fe750-149">The date that the certification expires.</span></span>            |
|<span data-ttu-id="fe750-150">推据</span><span class="sxs-lookup"><span data-stu-id="fe750-150">inference</span></span>|[<span data-ttu-id="fe750-151">inferenceData</span><span class="sxs-lookup"><span data-stu-id="fe750-151">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="fe750-152">如果实体受到创建或修改的应用程序的推理，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="fe750-152">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="fe750-153">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="fe750-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="fe750-154">issuedDate</span><span class="sxs-lookup"><span data-stu-id="fe750-154">issuedDate</span></span>       |<span data-ttu-id="fe750-155">日期</span><span class="sxs-lookup"><span data-stu-id="fe750-155">Date</span></span>        |<span data-ttu-id="fe750-156">认证的发布日期。</span><span class="sxs-lookup"><span data-stu-id="fe750-156">The date that the certification was issued.</span></span>         |
|<span data-ttu-id="fe750-157">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="fe750-157">issuingAuthority</span></span> |<span data-ttu-id="fe750-158">String</span><span class="sxs-lookup"><span data-stu-id="fe750-158">String</span></span>      |<span data-ttu-id="fe750-159">证书授权的颁发机构。</span><span class="sxs-lookup"><span data-stu-id="fe750-159">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="fe750-160">issuingCompany</span><span class="sxs-lookup"><span data-stu-id="fe750-160">issuingCompany</span></span>   |<span data-ttu-id="fe750-161">String</span><span class="sxs-lookup"><span data-stu-id="fe750-161">String</span></span>      |<span data-ttu-id="fe750-162">证书授权的颁发机构。</span><span class="sxs-lookup"><span data-stu-id="fe750-162">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="fe750-163">source</span><span class="sxs-lookup"><span data-stu-id="fe750-163">source</span></span>|[<span data-ttu-id="fe750-164">personDataSource</span><span class="sxs-lookup"><span data-stu-id="fe750-164">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="fe750-165">同步到其他服务时从哪个位置发送值。</span><span class="sxs-lookup"><span data-stu-id="fe750-165">Where the values originated if synced from another service.</span></span> <span data-ttu-id="fe750-166">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="fe750-166">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="fe750-167">startDate</span><span class="sxs-lookup"><span data-stu-id="fe750-167">startDate</span></span>        |<span data-ttu-id="fe750-168">日期</span><span class="sxs-lookup"><span data-stu-id="fe750-168">Date</span></span>        |<span data-ttu-id="fe750-169">认证的有效日期。</span><span class="sxs-lookup"><span data-stu-id="fe750-169">The date that the certification became valid.</span></span>       |
|<span data-ttu-id="fe750-170">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="fe750-170">thumbnailUrl</span></span>     |<span data-ttu-id="fe750-171">String</span><span class="sxs-lookup"><span data-stu-id="fe750-171">String</span></span>      |<span data-ttu-id="fe750-172">引用认证缩略图的 URL。</span><span class="sxs-lookup"><span data-stu-id="fe750-172">URL referencing a thumbnail of the certification.</span></span>   |
|<span data-ttu-id="fe750-173">webUrl</span><span class="sxs-lookup"><span data-stu-id="fe750-173">webUrl</span></span>           |<span data-ttu-id="fe750-174">String</span><span class="sxs-lookup"><span data-stu-id="fe750-174">String</span></span>      |<span data-ttu-id="fe750-175">引用认证的 URL。</span><span class="sxs-lookup"><span data-stu-id="fe750-175">URL referencing the certification.</span></span>                  |

## <a name="response"></a><span data-ttu-id="fe750-176">响应</span><span class="sxs-lookup"><span data-stu-id="fe750-176">Response</span></span>

<span data-ttu-id="fe750-177">如果成功，此方法将在响应 `201 Created` 正文中返回 [响应代码和 personCertification](../resources/personcertification.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fe750-177">If successful, this method returns a `201 Created` response code and an [personCertification](../resources/personcertification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fe750-178">示例</span><span class="sxs-lookup"><span data-stu-id="fe750-178">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="fe750-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe750-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personCertification_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/certifications
Content-Type: application/json
Content-length: 497

{
  "certificationId": "KB-1235466333663322",
  "description": "Blackbelt in Marketing - Brand Management",
  "displayName": "Marketing Blackbelt - Brand Management",
  "thumbnailUrl": "https://iame.io/dfhdfdfd334.jpg",
  "webUrl": "https://www.iame.io/blackbelt"
}
```
# <a name="c"></a>[<span data-ttu-id="fe750-180">C#</span><span class="sxs-lookup"><span data-stu-id="fe750-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personcertification-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe750-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe750-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personcertification-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe750-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe750-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personcertification-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="fe750-183">响应</span><span class="sxs-lookup"><span data-stu-id="fe750-183">Response</span></span>
<span data-ttu-id="fe750-184">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fe750-184">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personCertification"
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
  "certificationId": "KB-1235466333663322",
  "description": "Blackbelt in Marketing - Brand Management",
  "displayName": "Marketing Blackbelt - Brand Management",
  "endDate": "Date",
  "issuedDate": "Date",
  "issuingAuthority": null,
  "issuingCompany": null,
  "startDate": "Date",
  "thumbnailUrl": "https://iame.io/dfhdfdfd334.jpg",
  "webUrl": "https://www.iame.io/blackbelt"
}
```
