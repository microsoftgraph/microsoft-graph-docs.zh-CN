---
title: 获取 personCertification
description: 读取 personCertification 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: dcff70295646bb5b668dc4a14e5547b7c58daa07
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812947"
---
# <a name="get-personcertification"></a><span data-ttu-id="7cefb-103">获取 personCertification</span><span class="sxs-lookup"><span data-stu-id="7cefb-103">Get personCertification</span></span>
<span data-ttu-id="7cefb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cefb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7cefb-105">读取用户的[配置文件](../resources/profile.md)中的[personCertification](../resources/personcertification.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7cefb-105">Read the properties and relationships of a [personCertification](../resources/personcertification.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7cefb-106">权限</span><span class="sxs-lookup"><span data-stu-id="7cefb-106">Permissions</span></span>

<span data-ttu-id="7cefb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7cefb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7cefb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7cefb-109">Permission type</span></span>                        | <span data-ttu-id="7cefb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7cefb-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="7cefb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7cefb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7cefb-112">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="7cefb-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="7cefb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7cefb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cefb-114">User. Read、User.readbasic.all、user. all、All、user. all。 All</span><span class="sxs-lookup"><span data-stu-id="7cefb-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="7cefb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7cefb-115">Application</span></span>                            | <span data-ttu-id="7cefb-116">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="7cefb-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="7cefb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7cefb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/certifications/{id}
GET /users/{id | userPrincipalName}/profile/certifications/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7cefb-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7cefb-118">Optional query parameters</span></span>

<span data-ttu-id="7cefb-119">此方法支持 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="7cefb-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="7cefb-120">指定要包含在响应中的属性的列表，并以逗号分隔。</span><span class="sxs-lookup"><span data-stu-id="7cefb-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="7cefb-121">为获得最佳性能，请仅选择所需的属性子集。</span><span class="sxs-lookup"><span data-stu-id="7cefb-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7cefb-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7cefb-122">Request headers</span></span>
|<span data-ttu-id="7cefb-123">名称</span><span class="sxs-lookup"><span data-stu-id="7cefb-123">Name</span></span>|<span data-ttu-id="7cefb-124">说明</span><span class="sxs-lookup"><span data-stu-id="7cefb-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7cefb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cefb-125">Authorization</span></span>|<span data-ttu-id="7cefb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7cefb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cefb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7cefb-128">Request body</span></span>
<span data-ttu-id="7cefb-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7cefb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cefb-130">响应</span><span class="sxs-lookup"><span data-stu-id="7cefb-130">Response</span></span>

<span data-ttu-id="7cefb-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [personCertification](../resources/personcertification.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7cefb-131">If successful, this method returns a `200 OK` response code and an [personCertification](../resources/personcertification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7cefb-132">示例</span><span class="sxs-lookup"><span data-stu-id="7cefb-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7cefb-133">请求</span><span class="sxs-lookup"><span data-stu-id="7cefb-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="7cefb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cefb-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_personCertification"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/certifications/{id}
```
# <a name="c"></a>[<span data-ttu-id="7cefb-135">C#</span><span class="sxs-lookup"><span data-stu-id="7cefb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationalactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7cefb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cefb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationalactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7cefb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7cefb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationalactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="7cefb-138">响应</span><span class="sxs-lookup"><span data-stu-id="7cefb-138">Response</span></span>

<span data-ttu-id="7cefb-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7cefb-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
