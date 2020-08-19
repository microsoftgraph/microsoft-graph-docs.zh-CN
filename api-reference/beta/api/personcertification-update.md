---
title: 更新 personCertification
description: 更新 personCertification 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 52327323d177e9414790583cee670d300c9095c4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809634"
---
# <a name="update-personcertification"></a><span data-ttu-id="83472-103">更新 personCertification</span><span class="sxs-lookup"><span data-stu-id="83472-103">Update personCertification</span></span>
<span data-ttu-id="83472-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83472-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="83472-105">从用户的[配置文件](../resources/profile.md)中更新[personCertification](../resources/personcertification.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="83472-105">Update the properties of a [personCertification](../resources/personcertification.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="83472-106">权限</span><span class="sxs-lookup"><span data-stu-id="83472-106">Permissions</span></span>

<span data-ttu-id="83472-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83472-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83472-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="83472-109">Permission type</span></span>                        | <span data-ttu-id="83472-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="83472-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="83472-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83472-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="83472-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="83472-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="83472-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83472-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83472-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="83472-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="83472-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="83472-115">Application</span></span>                            | <span data-ttu-id="83472-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83472-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="83472-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83472-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/certifications/{id}
PATCH /users/{id | userPrincipalName}/profile/certifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="83472-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="83472-118">Request headers</span></span>
|<span data-ttu-id="83472-119">名称</span><span class="sxs-lookup"><span data-stu-id="83472-119">Name</span></span>|<span data-ttu-id="83472-120">说明</span><span class="sxs-lookup"><span data-stu-id="83472-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="83472-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="83472-121">Authorization</span></span>|<span data-ttu-id="83472-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="83472-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="83472-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83472-124">Content-Type</span></span>|<span data-ttu-id="83472-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="83472-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="83472-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="83472-127">Request body</span></span>

<span data-ttu-id="83472-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="83472-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="83472-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="83472-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="83472-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="83472-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="83472-131">属性</span><span class="sxs-lookup"><span data-stu-id="83472-131">Property</span></span>|<span data-ttu-id="83472-132">类型</span><span class="sxs-lookup"><span data-stu-id="83472-132">Type</span></span>|<span data-ttu-id="83472-133">说明</span><span class="sxs-lookup"><span data-stu-id="83472-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83472-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="83472-134">allowedAudiences</span></span>|<span data-ttu-id="83472-135">String</span><span class="sxs-lookup"><span data-stu-id="83472-135">String</span></span>|<span data-ttu-id="83472-136">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="83472-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="83472-137">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="83472-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="83472-138">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="83472-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="83472-139">certificationId</span><span class="sxs-lookup"><span data-stu-id="83472-139">certificationId</span></span>  |<span data-ttu-id="83472-140">String</span><span class="sxs-lookup"><span data-stu-id="83472-140">String</span></span>      |<span data-ttu-id="83472-141">证书的 referenceable 标识符。</span><span class="sxs-lookup"><span data-stu-id="83472-141">The referenceable identifier for the certification.</span></span> |
|<span data-ttu-id="83472-142">description</span><span class="sxs-lookup"><span data-stu-id="83472-142">description</span></span>      |<span data-ttu-id="83472-143">String</span><span class="sxs-lookup"><span data-stu-id="83472-143">String</span></span>      |<span data-ttu-id="83472-144">证书的说明。</span><span class="sxs-lookup"><span data-stu-id="83472-144">Description of the certification.</span></span>                   |
|<span data-ttu-id="83472-145">displayName</span><span class="sxs-lookup"><span data-stu-id="83472-145">displayName</span></span>      |<span data-ttu-id="83472-146">String</span><span class="sxs-lookup"><span data-stu-id="83472-146">String</span></span>      |<span data-ttu-id="83472-147">证书的标题。</span><span class="sxs-lookup"><span data-stu-id="83472-147">Title of the certification.</span></span>                         |
|<span data-ttu-id="83472-148">endDate</span><span class="sxs-lookup"><span data-stu-id="83472-148">endDate</span></span>          |<span data-ttu-id="83472-149">日期</span><span class="sxs-lookup"><span data-stu-id="83472-149">Date</span></span>        |<span data-ttu-id="83472-150">证书到期的日期。</span><span class="sxs-lookup"><span data-stu-id="83472-150">The date that the certification expires.</span></span>            |
|<span data-ttu-id="83472-151">推导</span><span class="sxs-lookup"><span data-stu-id="83472-151">inference</span></span>|[<span data-ttu-id="83472-152">inferenceData</span><span class="sxs-lookup"><span data-stu-id="83472-152">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="83472-153">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="83472-153">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="83472-154">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="83472-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="83472-155">issuedDate</span><span class="sxs-lookup"><span data-stu-id="83472-155">issuedDate</span></span>       |<span data-ttu-id="83472-156">日期</span><span class="sxs-lookup"><span data-stu-id="83472-156">Date</span></span>        |<span data-ttu-id="83472-157">颁发证书的日期。</span><span class="sxs-lookup"><span data-stu-id="83472-157">The date that the certification was issued.</span></span>         |
|<span data-ttu-id="83472-158">issuingAuthority</span><span class="sxs-lookup"><span data-stu-id="83472-158">issuingAuthority</span></span> |<span data-ttu-id="83472-159">String</span><span class="sxs-lookup"><span data-stu-id="83472-159">String</span></span>      |<span data-ttu-id="83472-160">授予证书颁发机构的权限。</span><span class="sxs-lookup"><span data-stu-id="83472-160">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="83472-161">issuingCompany</span><span class="sxs-lookup"><span data-stu-id="83472-161">issuingCompany</span></span>   |<span data-ttu-id="83472-162">String</span><span class="sxs-lookup"><span data-stu-id="83472-162">String</span></span>      |<span data-ttu-id="83472-163">授予证书颁发机构的权限。</span><span class="sxs-lookup"><span data-stu-id="83472-163">Authority which granted the certification.</span></span>          |
|<span data-ttu-id="83472-164">startDate</span><span class="sxs-lookup"><span data-stu-id="83472-164">startDate</span></span>        |<span data-ttu-id="83472-165">日期</span><span class="sxs-lookup"><span data-stu-id="83472-165">Date</span></span>        |<span data-ttu-id="83472-166">证书生效的日期。</span><span class="sxs-lookup"><span data-stu-id="83472-166">The date that the certification became valid.</span></span>       |
|<span data-ttu-id="83472-167">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="83472-167">thumbnailUrl</span></span>     |<span data-ttu-id="83472-168">String</span><span class="sxs-lookup"><span data-stu-id="83472-168">String</span></span>      |<span data-ttu-id="83472-169">URL 引用证书的缩略图。</span><span class="sxs-lookup"><span data-stu-id="83472-169">URL referencing a thumbnail of the certification.</span></span>   |
|<span data-ttu-id="83472-170">webUrl</span><span class="sxs-lookup"><span data-stu-id="83472-170">webUrl</span></span>           |<span data-ttu-id="83472-171">String</span><span class="sxs-lookup"><span data-stu-id="83472-171">String</span></span>      |<span data-ttu-id="83472-172">引用证书的 URL。</span><span class="sxs-lookup"><span data-stu-id="83472-172">URL referencing the certification.</span></span>                  |

## <a name="response"></a><span data-ttu-id="83472-173">响应</span><span class="sxs-lookup"><span data-stu-id="83472-173">Response</span></span>

<span data-ttu-id="83472-174">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [personCertification](../resources/personcertification.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83472-174">If successful, this method returns a `200 OK` response code and an updated [personCertification](../resources/personcertification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83472-175">示例</span><span class="sxs-lookup"><span data-stu-id="83472-175">Examples</span></span>

### <a name="request"></a><span data-ttu-id="83472-176">请求</span><span class="sxs-lookup"><span data-stu-id="83472-176">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="83472-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="83472-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personcertification"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/user/{userId}/profile/certifications/{id}
Content-Type: application/json
Content-length: 497

{
  "issuingAuthority": "International Academy of Marketing Excellence",
  "issuingCompany": "International Academy of Marketing Excellence"
}
```
# <a name="c"></a>[<span data-ttu-id="83472-178">C#</span><span class="sxs-lookup"><span data-stu-id="83472-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83472-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83472-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83472-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83472-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="83472-181">响应</span><span class="sxs-lookup"><span data-stu-id="83472-181">Response</span></span>
<span data-ttu-id="83472-182">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="83472-182">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personCertification"
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
  "certificationId": "KB-1235466333663322",
  "description": "Blackbelt in Marketing - Brand Management",
  "displayName": "Marketing Blackbelt - Brand Management",
  "endDate": "Date",
  "issuedDate": "Date",
  "issuingAuthority": "International Academy of Marketing Excellence",
  "issuingCompany": "International Academy of Marketing Excellence",
  "startDate": "Date",
  "thumbnailUrl": "https://iame.io/dfhdfdfd334.jpg",
  "webUrl": "https://www.iame.io/blackbelt"
}
```
