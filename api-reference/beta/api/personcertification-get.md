---
title: 获取 personCertification
description: 读取 personCertification 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: af3bc004cec2fae525e655c3b10c8e553db961b1
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819666"
---
# <a name="get-personcertification"></a><span data-ttu-id="d98c9-103">获取 personCertification</span><span class="sxs-lookup"><span data-stu-id="d98c9-103">Get personCertification</span></span>
<span data-ttu-id="d98c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d98c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d98c9-105">读取用户配置文件中的 [personCertification](../resources/personcertification.md) 对象的属性和 [关系](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="d98c9-105">Read the properties and relationships of a [personCertification](../resources/personcertification.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d98c9-106">权限</span><span class="sxs-lookup"><span data-stu-id="d98c9-106">Permissions</span></span>

<span data-ttu-id="d98c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d98c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d98c9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d98c9-109">Permission type</span></span>                        | <span data-ttu-id="d98c9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d98c9-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="d98c9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d98c9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d98c9-112">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d98c9-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d98c9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d98c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d98c9-114">User.Read、User.ReadWrite、User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d98c9-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d98c9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d98c9-115">Application</span></span>                            | <span data-ttu-id="d98c9-116">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d98c9-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="d98c9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d98c9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/certifications/{id}
GET /users/{id | userPrincipalName}/profile/certifications/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d98c9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d98c9-118">Optional query parameters</span></span>

<span data-ttu-id="d98c9-119">此方法支持 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="d98c9-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="d98c9-120">指定要在响应中包含的属性列表，并用逗号将它们分开。</span><span class="sxs-lookup"><span data-stu-id="d98c9-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="d98c9-121">为了获得最佳性能，请仅选择需要的属性子集。</span><span class="sxs-lookup"><span data-stu-id="d98c9-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d98c9-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d98c9-122">Request headers</span></span>
|<span data-ttu-id="d98c9-123">名称</span><span class="sxs-lookup"><span data-stu-id="d98c9-123">Name</span></span>|<span data-ttu-id="d98c9-124">说明</span><span class="sxs-lookup"><span data-stu-id="d98c9-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d98c9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d98c9-125">Authorization</span></span>|<span data-ttu-id="d98c9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d98c9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d98c9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d98c9-128">Request body</span></span>
<span data-ttu-id="d98c9-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d98c9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d98c9-130">响应</span><span class="sxs-lookup"><span data-stu-id="d98c9-130">Response</span></span>

<span data-ttu-id="d98c9-131">如果成功，此方法将在响应 `200 OK` 正文中返回 [响应代码和 personCertification](../resources/personcertification.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d98c9-131">If successful, this method returns a `200 OK` response code and an [personCertification](../resources/personcertification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d98c9-132">示例</span><span class="sxs-lookup"><span data-stu-id="d98c9-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d98c9-133">请求</span><span class="sxs-lookup"><span data-stu-id="d98c9-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="d98c9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d98c9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_personCertification"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/certifications/{id}
```
# <a name="c"></a>[<span data-ttu-id="d98c9-135">C#</span><span class="sxs-lookup"><span data-stu-id="d98c9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personcertification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d98c9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d98c9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personcertification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d98c9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d98c9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personcertification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d98c9-138">响应</span><span class="sxs-lookup"><span data-stu-id="d98c9-138">Response</span></span>

<span data-ttu-id="d98c9-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d98c9-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
