---
title: 更新域
description: 更新域对象的属性。
ms.openlocfilehash: 38a4baca42b22465ba2ea98081b7619d5f8af0e1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044217"
---
# <a name="update-domain"></a><span data-ttu-id="7e560-103">更新域</span><span class="sxs-lookup"><span data-stu-id="7e560-103">Update domain</span></span>

> <span data-ttu-id="7e560-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7e560-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e560-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7e560-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7e560-106">更新域对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7e560-106">Update the properties of domain object.</span></span>

> <span data-ttu-id="7e560-107">**重要说明：** 只有已验证的域可以进行更新。</span><span class="sxs-lookup"><span data-stu-id="7e560-107">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e560-108">权限</span><span class="sxs-lookup"><span data-stu-id="7e560-108">Permissions</span></span>

<span data-ttu-id="7e560-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e560-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7e560-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e560-111">Permission type</span></span>      | <span data-ttu-id="7e560-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e560-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e560-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e560-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7e560-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7e560-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7e560-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e560-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e560-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e560-116">Not supported.</span></span>    |
|<span data-ttu-id="7e560-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e560-117">Application</span></span> | <span data-ttu-id="7e560-118">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e560-118">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e560-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e560-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="7e560-120">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="7e560-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e560-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e560-121">Request headers</span></span>

| <span data-ttu-id="7e560-122">名称</span><span class="sxs-lookup"><span data-stu-id="7e560-122">Name</span></span>       | <span data-ttu-id="7e560-123">说明</span><span class="sxs-lookup"><span data-stu-id="7e560-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7e560-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e560-124">Authorization</span></span>  | <span data-ttu-id="7e560-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e560-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e560-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e560-127">Content-Type</span></span>  | <span data-ttu-id="7e560-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7e560-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e560-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e560-129">Request body</span></span>

<span data-ttu-id="7e560-p104">在请求正文中，提供要更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，仅包含已更改的值。</span><span class="sxs-lookup"><span data-stu-id="7e560-p104">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="7e560-133">响应</span><span class="sxs-lookup"><span data-stu-id="7e560-133">Response</span></span>

<span data-ttu-id="7e560-134">如果成功，此方法返回 `204 No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="7e560-134">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e560-135">示例</span><span class="sxs-lookup"><span data-stu-id="7e560-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e560-136">请求</span><span class="sxs-lookup"><span data-stu-id="7e560-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/beta/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="7e560-137">响应</span><span class="sxs-lookup"><span data-stu-id="7e560-137">Response</span></span>

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