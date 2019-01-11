---
title: 域：验证
description: 验证域的所有权。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 4948f2dc833db80c2cbc3f3b8aa7c487b7bb97aa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864699"
---
# <a name="domain-verify"></a><span data-ttu-id="a4a79-103">域：验证</span><span class="sxs-lookup"><span data-stu-id="a4a79-103">domain: verify</span></span>

> <span data-ttu-id="a4a79-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a4a79-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4a79-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a4a79-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4a79-106">验证域的所有权。</span><span class="sxs-lookup"><span data-stu-id="a4a79-106">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="a4a79-p102">**重要说明：** 仅适用于未验证的域。对于未验证的域，[域](../resources/domain.md)的 isVerified 属性为 false。</span><span class="sxs-lookup"><span data-stu-id="a4a79-p102">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4a79-109">权限</span><span class="sxs-lookup"><span data-stu-id="a4a79-109">Permissions</span></span>

<span data-ttu-id="a4a79-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4a79-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a4a79-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4a79-112">Permission type</span></span>      | <span data-ttu-id="a4a79-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4a79-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4a79-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4a79-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a4a79-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4a79-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="a4a79-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4a79-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4a79-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4a79-117">Not supported.</span></span>    |
|<span data-ttu-id="a4a79-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4a79-118">Application</span></span> | <span data-ttu-id="a4a79-119">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4a79-119">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4a79-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4a79-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="a4a79-121">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="a4a79-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4a79-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4a79-122">Request headers</span></span>

| <span data-ttu-id="a4a79-123">名称</span><span class="sxs-lookup"><span data-stu-id="a4a79-123">Name</span></span>       | <span data-ttu-id="a4a79-124">说明</span><span class="sxs-lookup"><span data-stu-id="a4a79-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a4a79-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4a79-125">Authorization</span></span>  | <span data-ttu-id="a4a79-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4a79-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="a4a79-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4a79-128">Content-Type</span></span>  | <span data-ttu-id="a4a79-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a4a79-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4a79-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4a79-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a4a79-131">响应</span><span class="sxs-lookup"><span data-stu-id="a4a79-131">Response</span></span>

<span data-ttu-id="a4a79-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [domain](../resources/domain.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a4a79-132">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4a79-133">示例</span><span class="sxs-lookup"><span data-stu-id="a4a79-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4a79-134">请求</span><span class="sxs-lookup"><span data-stu-id="a4a79-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/verify
```

##### <a name="response"></a><span data-ttu-id="a4a79-135">响应</span><span class="sxs-lookup"><span data-stu-id="a4a79-135">Response</span></span>
<span data-ttu-id="a4a79-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4a79-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
