---
title: 域：验证
description: 验证域的所有权。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c4289e6c67844238460be9e706b8ff2f51c55035
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519155"
---
# <a name="domain-verify"></a><span data-ttu-id="5661b-103">域：验证</span><span class="sxs-lookup"><span data-stu-id="5661b-103">domain: verify</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5661b-104">验证域的所有权。</span><span class="sxs-lookup"><span data-stu-id="5661b-104">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="5661b-p101">**重要说明：** 仅适用于未验证的域。对于未验证的域，[域](../resources/domain.md)的 isVerified 属性为 false。</span><span class="sxs-lookup"><span data-stu-id="5661b-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="5661b-107">权限</span><span class="sxs-lookup"><span data-stu-id="5661b-107">Permissions</span></span>

<span data-ttu-id="5661b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5661b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5661b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5661b-110">Permission type</span></span>      | <span data-ttu-id="5661b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5661b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5661b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5661b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5661b-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5661b-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="5661b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5661b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5661b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5661b-115">Not supported.</span></span>    |
|<span data-ttu-id="5661b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5661b-116">Application</span></span> | <span data-ttu-id="5661b-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5661b-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5661b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5661b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="5661b-119">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="5661b-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5661b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5661b-120">Request headers</span></span>

| <span data-ttu-id="5661b-121">名称</span><span class="sxs-lookup"><span data-stu-id="5661b-121">Name</span></span>       | <span data-ttu-id="5661b-122">说明</span><span class="sxs-lookup"><span data-stu-id="5661b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5661b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5661b-123">Authorization</span></span>  | <span data-ttu-id="5661b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5661b-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="5661b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5661b-126">Content-Type</span></span>  | <span data-ttu-id="5661b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5661b-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5661b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5661b-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5661b-129">响应</span><span class="sxs-lookup"><span data-stu-id="5661b-129">Response</span></span>

<span data-ttu-id="5661b-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [domain](../resources/domain.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5661b-130">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5661b-131">示例</span><span class="sxs-lookup"><span data-stu-id="5661b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5661b-132">请求</span><span class="sxs-lookup"><span data-stu-id="5661b-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/verify
```

##### <a name="response"></a><span data-ttu-id="5661b-133">响应</span><span class="sxs-lookup"><span data-stu-id="5661b-133">Response</span></span>
<span data-ttu-id="5661b-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5661b-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "name": "contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-verify.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
