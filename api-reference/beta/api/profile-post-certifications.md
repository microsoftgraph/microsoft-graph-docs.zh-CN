---
title: 创建证书
description: 创建新的认证对象。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9a97a1219a1d98b4fdd456ac24e4ac78a1b5920e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809616"
---
# <a name="create-personcertification"></a><span data-ttu-id="0d8bc-103">创建 personCertification</span><span class="sxs-lookup"><span data-stu-id="0d8bc-103">Create personCertification</span></span>
<span data-ttu-id="0d8bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d8bc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d8bc-105">在用户的[配置文件](../resources/profile.md)中创建新的[personCertification](../resources/personcertification.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-105">Create a new [personCertification](../resources/personcertification.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0d8bc-106">权限</span><span class="sxs-lookup"><span data-stu-id="0d8bc-106">Permissions</span></span>

<span data-ttu-id="0d8bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d8bc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d8bc-109">Permission type</span></span>                        | <span data-ttu-id="0d8bc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d8bc-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="0d8bc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d8bc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d8bc-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0d8bc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d8bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d8bc-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0d8bc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d8bc-115">Application</span></span>                            | <span data-ttu-id="0d8bc-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d8bc-116">User.ReadWrite.All</span></span>                            |
## <a name="http-request"></a><span data-ttu-id="0d8bc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d8bc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/certifications
POST /users/{id | userPrincipalName}/profile/certifications
```

## <a name="request-headers"></a><span data-ttu-id="0d8bc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d8bc-118">Request headers</span></span>
|<span data-ttu-id="0d8bc-119">名称</span><span class="sxs-lookup"><span data-stu-id="0d8bc-119">Name</span></span>|<span data-ttu-id="0d8bc-120">说明</span><span class="sxs-lookup"><span data-stu-id="0d8bc-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0d8bc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d8bc-121">Authorization</span></span>|<span data-ttu-id="0d8bc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0d8bc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d8bc-124">Content-Type</span></span>|<span data-ttu-id="0d8bc-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0d8bc-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d8bc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d8bc-127">Request body</span></span>
<span data-ttu-id="0d8bc-128">在请求正文中，提供 [personCertification](../resources/personcertification.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-128">In the request body, supply a JSON representation of the [personCertification](../resources/personcertification.md) object.</span></span>

<span data-ttu-id="0d8bc-129">下表显示了在用户[配置文件](../resources/profile.md)中创建新的[personCertification](../resources/personcertification.md)对象时可以设置的属性。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-129">The following table shows the properties that are possible to set when creating a new [personCertification](../resources/personcertification.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="0d8bc-130">属性</span><span class="sxs-lookup"><span data-stu-id="0d8bc-130">Property</span></span>|<span data-ttu-id="0d8bc-131">类型</span><span class="sxs-lookup"><span data-stu-id="0d8bc-131">Type</span></span>|<span data-ttu-id="0d8bc-132">说明</span><span class="sxs-lookup"><span data-stu-id="0d8bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d8bc-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="0d8bc-133">allowedAudiences</span></span>|<span data-ttu-id="0d8bc-134">String</span><span class="sxs-lookup"><span data-stu-id="0d8bc-134">String</span></span>|<span data-ttu-id="0d8bc-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="0d8bc-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="0d8bc-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0d8bc-138">certificationId</span><span class="sxs-lookup"><span data-stu-id="0d8bc-138">certificationId</span></span>  |<span data-ttu-id="0d8bc-139">String</span><span class="sxs-lookup"><span data-stu-id="0d8bc-139">String</span></span>      |<span data-ttu-id="0d8bc-140">证书的 referenceable 标识符。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-140">The referenceable identifier for the certification.</span></span> |
|<span data-ttu-id="0d8bc-141">description</span><span class="sxs-lookup"><span data-stu-id="0d8bc-141">description</span></span>      |<span data-ttu-id="0d8bc-142">String</span><span class="sxs-lookup"><span data-stu-id="0d8bc-142">String</span></span>      |<span data-ttu-id="0d8bc-143">证书的说明。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-143">Description of the certification.</span></span>                   |
|<span data-ttu-id="0d8bc-144">displayName</span><span class="sxs-lookup"><span data-stu-id="0d8bc-144">displayName</span></span>      |<span data-ttu-id="0d8bc-145">String</span><span class="sxs-lookup"><span data-stu-id="0d8bc-145">String</span></span>      |<span data-ttu-id="0d8bc-146">证书的标题。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-146">Title of the certification.</span></span>                         |
|<span data-ttu-id="0d8bc-147">endDate</span><span class="sxs-lookup"><span data-stu-id="0d8bc-147">endDate</span></span>          |<span data-ttu-id="0d8bc-148">日期</span><span class="sxs-lookup"><span data-stu-id="0d8bc-148">Date</span></span>        |<span data-ttu-id="0d8bc-149">证书到期的日期。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-149">The date that the certification expires.</span></span>            |
|<span data-ttu-id="0d8bc-150">推导</span><span class="sxs-lookup"><span data-stu-id="0d8bc-150">inference</span></span>|[<span data-ttu-id="0d8bc-151">inferenceData</span><span class="sxs-lookup"><span data-stu-id="0d8bc-151">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="0d8bc-152">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-152">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="0d8bc-153">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0d8bc-154">issuedDate</span><span class="sxs-lookup"><span data-stu-id="0d8bc-154">issuedDate</span></span>       |<span data-ttu-id="0d8bc-155">日期</span><span class="sxs-lookup"><span data-stu-id="0d8bc-155">Date</span></span>        |<span data-ttu-id="0d8bc-156">颁发证书的日期。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-156">The date that the certification was issued.</span></span>         |
|<span data-ttu-id="0d8bc-157">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="0d8bc-157">issuingAuthority</span></span> |<span data-ttu-id="0d8bc-158">String</span><span class="sxs-lookup"><span data-stu-id="0d8bc-158">String</span></span>      |<span data-ttu-id="0d8bc-159">授予证书颁发机构的权限。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-159">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="0d8bc-160">issuingCompany</span><span class="sxs-lookup"><span data-stu-id="0d8bc-160">issuingCompany</span></span>   |<span data-ttu-id="0d8bc-161">String</span><span class="sxs-lookup"><span data-stu-id="0d8bc-161">String</span></span>      |<span data-ttu-id="0d8bc-162">授予证书颁发机构的权限。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-162">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="0d8bc-163">source</span><span class="sxs-lookup"><span data-stu-id="0d8bc-163">source</span></span>|[<span data-ttu-id="0d8bc-164">personDataSource</span><span class="sxs-lookup"><span data-stu-id="0d8bc-164">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="0d8bc-165">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-165">Where the values originated if synced from another service.</span></span> <span data-ttu-id="0d8bc-166">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-166">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="0d8bc-167">startDate</span><span class="sxs-lookup"><span data-stu-id="0d8bc-167">startDate</span></span>        |<span data-ttu-id="0d8bc-168">日期</span><span class="sxs-lookup"><span data-stu-id="0d8bc-168">Date</span></span>        |<span data-ttu-id="0d8bc-169">证书生效的日期。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-169">The date that the certification became valid.</span></span>       |
|<span data-ttu-id="0d8bc-170">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="0d8bc-170">thumbnailUrl</span></span>     |<span data-ttu-id="0d8bc-171">String</span><span class="sxs-lookup"><span data-stu-id="0d8bc-171">String</span></span>      |<span data-ttu-id="0d8bc-172">URL 引用证书的缩略图。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-172">URL referencing a thumbnail of the certification.</span></span>   |
|<span data-ttu-id="0d8bc-173">webUrl</span><span class="sxs-lookup"><span data-stu-id="0d8bc-173">webUrl</span></span>           |<span data-ttu-id="0d8bc-174">String</span><span class="sxs-lookup"><span data-stu-id="0d8bc-174">String</span></span>      |<span data-ttu-id="0d8bc-175">引用证书的 URL。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-175">URL referencing the certification.</span></span>                  |

## <a name="response"></a><span data-ttu-id="0d8bc-176">响应</span><span class="sxs-lookup"><span data-stu-id="0d8bc-176">Response</span></span>

<span data-ttu-id="0d8bc-177">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [personCertification](../resources/personcertification.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-177">If successful, this method returns a `201 Created` response code and an [personCertification](../resources/personcertification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d8bc-178">示例</span><span class="sxs-lookup"><span data-stu-id="0d8bc-178">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="0d8bc-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d8bc-179">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0d8bc-180">C#</span><span class="sxs-lookup"><span data-stu-id="0d8bc-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d8bc-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d8bc-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d8bc-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d8bc-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0d8bc-183">响应</span><span class="sxs-lookup"><span data-stu-id="0d8bc-183">Response</span></span>
<span data-ttu-id="0d8bc-184">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0d8bc-184">**Note:** The response object shown here might be shortened for readability.</span></span>
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
