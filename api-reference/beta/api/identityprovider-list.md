---
title: 列表 identityProviders
description: 检索所有 identityProviders 目录中。
localization_priority: Normal
ms.openlocfilehash: 4226e6f091527d2df8bfb544327ec2e49f2b890c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529731"
---
# <a name="list-identityproviders"></a><span data-ttu-id="73f09-103">列表 identityProviders</span><span class="sxs-lookup"><span data-stu-id="73f09-103">List identityProviders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73f09-104">检索所有[identityProviders](../resources/identityprovider.md)目录中。</span><span class="sxs-lookup"><span data-stu-id="73f09-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="73f09-105">权限</span><span class="sxs-lookup"><span data-stu-id="73f09-105">Permissions</span></span>

<span data-ttu-id="73f09-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73f09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73f09-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="73f09-108">Permission type</span></span>      | <span data-ttu-id="73f09-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73f09-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73f09-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73f09-110">Delegated (work or school account)</span></span>|<span data-ttu-id="73f09-111">IdentityProvider.Read.All IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73f09-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="73f09-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73f09-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="73f09-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="73f09-113">Not supported.</span></span>|
|<span data-ttu-id="73f09-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="73f09-114">Application</span></span>|<span data-ttu-id="73f09-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="73f09-115">Not supported.</span></span>|

<span data-ttu-id="73f09-116">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="73f09-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="73f09-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73f09-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="73f09-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="73f09-118">Request headers</span></span>

|<span data-ttu-id="73f09-119">名称</span><span class="sxs-lookup"><span data-stu-id="73f09-119">Name</span></span>|<span data-ttu-id="73f09-120">说明</span><span class="sxs-lookup"><span data-stu-id="73f09-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="73f09-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="73f09-121">Authorization</span></span>|<span data-ttu-id="73f09-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73f09-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73f09-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="73f09-124">Request body</span></span>

<span data-ttu-id="73f09-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73f09-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73f09-126">响应</span><span class="sxs-lookup"><span data-stu-id="73f09-126">Response</span></span>

<span data-ttu-id="73f09-127">如果成功，此方法返回`200 OK`响应代码和[identityProviders](../resources/identityprovider.md)中响应正文中的 JSON 表示形式的集合。</span><span class="sxs-lookup"><span data-stu-id="73f09-127">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73f09-128">示例</span><span class="sxs-lookup"><span data-stu-id="73f09-128">Example</span></span>

<span data-ttu-id="73f09-129">以下示例检索所有**identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="73f09-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="73f09-130">请求</span><span class="sxs-lookup"><span data-stu-id="73f09-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```

##### <a name="response"></a><span data-ttu-id="73f09-131">响应</span><span class="sxs-lookup"><span data-stu-id="73f09-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "Amazon-OAUTH",
        "name": "Login with Amazon",
        "type": "Amazon",
        "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
        "clientSecret": "*****"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityprovider-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
