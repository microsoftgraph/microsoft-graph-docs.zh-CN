---
title: 从 incompatibleAccessPackages 中删除 accessPackage
description: 删除指示访问包与指定访问包不兼容的链接。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7cb6ad4af6809c75edef5f5e2966eee72a357215
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401052"
---
# <a name="remove-accesspackage-from-incompatibleaccesspackages"></a><span data-ttu-id="6da09-103">从 incompatibleAccessPackages 中删除 accessPackage</span><span class="sxs-lookup"><span data-stu-id="6da09-103">Remove accessPackage from incompatibleAccessPackages</span></span>

<span data-ttu-id="6da09-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6da09-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6da09-105">从 [accessPackage](../resources/accesspackage.md) 上标记为不兼容的访问包列表中删除 [访问包](../resources/accesspackage.md)。</span><span class="sxs-lookup"><span data-stu-id="6da09-105">Remove an [access package](../resources/accesspackage.md) from the list of access packages that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="6da09-106">权限</span><span class="sxs-lookup"><span data-stu-id="6da09-106">Permissions</span></span>

<span data-ttu-id="6da09-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6da09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6da09-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6da09-109">Permission type</span></span>                        | <span data-ttu-id="6da09-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6da09-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6da09-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6da09-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6da09-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6da09-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="6da09-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6da09-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6da09-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6da09-114">Not supported.</span></span> |
| <span data-ttu-id="6da09-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6da09-115">Application</span></span>                            | <span data-ttu-id="6da09-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6da09-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6da09-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6da09-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6da09-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6da09-118">Request headers</span></span>

| <span data-ttu-id="6da09-119">名称</span><span class="sxs-lookup"><span data-stu-id="6da09-119">Name</span></span>          | <span data-ttu-id="6da09-120">说明</span><span class="sxs-lookup"><span data-stu-id="6da09-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6da09-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6da09-121">Authorization</span></span> | <span data-ttu-id="6da09-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6da09-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6da09-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6da09-124">Content-Type</span></span>  | <span data-ttu-id="6da09-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6da09-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6da09-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6da09-127">Request body</span></span>

<span data-ttu-id="6da09-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6da09-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6da09-129">响应</span><span class="sxs-lookup"><span data-stu-id="6da09-129">Response</span></span>

<span data-ttu-id="6da09-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6da09-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6da09-132">示例</span><span class="sxs-lookup"><span data-stu-id="6da09-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6da09-133">请求</span><span class="sxs-lookup"><span data-stu-id="6da09-133">Request</span></span>

<span data-ttu-id="6da09-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6da09-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_incompatibleaccesspackage_from_accesspackage"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/{id}/$ref
```


### <a name="response"></a><span data-ttu-id="6da09-135">响应</span><span class="sxs-lookup"><span data-stu-id="6da09-135">Response</span></span>

<span data-ttu-id="6da09-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6da09-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove incompatibleAccessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

