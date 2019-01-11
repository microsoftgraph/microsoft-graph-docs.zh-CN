---
title: 更新域
description: 更新域对象的属性。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 07e1e78a43902b846e070523802eeb128217f953
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861409"
---
# <a name="update-domain"></a><span data-ttu-id="646c4-103">更新域</span><span class="sxs-lookup"><span data-stu-id="646c4-103">Update domain</span></span>

<span data-ttu-id="646c4-104">更新域对象的属性。</span><span class="sxs-lookup"><span data-stu-id="646c4-104">Update the properties of domain object.</span></span>

> <span data-ttu-id="646c4-105">**重要说明：** 只有已验证的域可以进行更新。</span><span class="sxs-lookup"><span data-stu-id="646c4-105">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="646c4-106">权限</span><span class="sxs-lookup"><span data-stu-id="646c4-106">Permissions</span></span>

<span data-ttu-id="646c4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="646c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="646c4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="646c4-109">Permission type</span></span>      | <span data-ttu-id="646c4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="646c4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="646c4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="646c4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="646c4-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="646c4-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="646c4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="646c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="646c4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="646c4-114">Not supported.</span></span>    |
|<span data-ttu-id="646c4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="646c4-115">Application</span></span> | <span data-ttu-id="646c4-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="646c4-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="646c4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="646c4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="646c4-118">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="646c4-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="646c4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="646c4-119">Request headers</span></span>

| <span data-ttu-id="646c4-120">名称</span><span class="sxs-lookup"><span data-stu-id="646c4-120">Name</span></span>       | <span data-ttu-id="646c4-121">说明</span><span class="sxs-lookup"><span data-stu-id="646c4-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="646c4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="646c4-122">Authorization</span></span>  | <span data-ttu-id="646c4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="646c4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="646c4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="646c4-125">Content-Type</span></span>  | <span data-ttu-id="646c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="646c4-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="646c4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="646c4-127">Request body</span></span>

<span data-ttu-id="646c4-p103">在请求正文中，提供要更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，仅包含已更改的值。</span><span class="sxs-lookup"><span data-stu-id="646c4-p103">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="646c4-131">响应</span><span class="sxs-lookup"><span data-stu-id="646c4-131">Response</span></span>

<span data-ttu-id="646c4-132">如果成功，此方法返回 `204 No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="646c4-132">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="646c4-133">示例</span><span class="sxs-lookup"><span data-stu-id="646c4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="646c4-134">请求</span><span class="sxs-lookup"><span data-stu-id="646c4-134">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="646c4-135">响应</span><span class="sxs-lookup"><span data-stu-id="646c4-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
