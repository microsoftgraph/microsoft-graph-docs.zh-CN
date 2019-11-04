---
title: 删除 accessPackageCatalog
description: 删除 accessPackageCatalog。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f6ab9df54690c93453e3fd030c37978d42db7da9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935284"
---
# <a name="delete-accesspackagecatalog"></a><span data-ttu-id="25ff0-103">删除 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="25ff0-103">Delete accessPackageCatalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25ff0-104">删除[accessPackageCatalog](../resources/accesspackagecatalog.md)。</span><span class="sxs-lookup"><span data-stu-id="25ff0-104">Delete an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="25ff0-105">权限</span><span class="sxs-lookup"><span data-stu-id="25ff0-105">Permissions</span></span>

<span data-ttu-id="25ff0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25ff0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="25ff0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="25ff0-108">Permission type</span></span>                        | <span data-ttu-id="25ff0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25ff0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="25ff0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25ff0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="25ff0-111">EntitlementManagement</span><span class="sxs-lookup"><span data-stu-id="25ff0-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="25ff0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25ff0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25ff0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="25ff0-113">Not supported.</span></span> |
| <span data-ttu-id="25ff0-114">Application</span><span class="sxs-lookup"><span data-stu-id="25ff0-114">Application</span></span>                            | <span data-ttu-id="25ff0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="25ff0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="25ff0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25ff0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="25ff0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="25ff0-117">Request headers</span></span>

| <span data-ttu-id="25ff0-118">名称</span><span class="sxs-lookup"><span data-stu-id="25ff0-118">Name</span></span>          | <span data-ttu-id="25ff0-119">说明</span><span class="sxs-lookup"><span data-stu-id="25ff0-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="25ff0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="25ff0-120">Authorization</span></span> | <span data-ttu-id="25ff0-121">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="25ff0-121">Bearer \{token\}.</span></span> <span data-ttu-id="25ff0-122">必填。</span><span class="sxs-lookup"><span data-stu-id="25ff0-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25ff0-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="25ff0-123">Request body</span></span>

<span data-ttu-id="25ff0-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="25ff0-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25ff0-125">响应</span><span class="sxs-lookup"><span data-stu-id="25ff0-125">Response</span></span>

<span data-ttu-id="25ff0-126">如果成功，此方法将返回一个200系列响应代码。</span><span class="sxs-lookup"><span data-stu-id="25ff0-126">If successful, this method returns a 200-series response code.</span></span> <span data-ttu-id="25ff0-127">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="25ff0-127">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="25ff0-128">示例</span><span class="sxs-lookup"><span data-stu-id="25ff0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="25ff0-129">请求</span><span class="sxs-lookup"><span data-stu-id="25ff0-129">Request</span></span>

<span data-ttu-id="25ff0-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="25ff0-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accesspackagecatalog"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

### <a name="response"></a><span data-ttu-id="25ff0-131">响应</span><span class="sxs-lookup"><span data-stu-id="25ff0-131">Response</span></span>

<span data-ttu-id="25ff0-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="25ff0-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
