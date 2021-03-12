---
title: 删除本地化的组织BrandingProperties
description: 删除 organizationalBrandingProperties 以用于特定本地化。
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d15d5e5ef20cc7d18fbd26097fcdc19f7802ca0f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722534"
---
# <a name="delete-localized-organizationalbrandingproperties"></a><span data-ttu-id="771ac-103">删除本地化的组织BrandingProperties</span><span class="sxs-lookup"><span data-stu-id="771ac-103">Delete Localized organizationalBrandingProperties</span></span>

<span data-ttu-id="771ac-104">删除 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="771ac-104">Delete an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="771ac-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="771ac-105">Permissions</span></span>

<span data-ttu-id="771ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="771ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="771ac-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="771ac-108">Permission type</span></span>                        | <span data-ttu-id="771ac-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="771ac-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="771ac-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="771ac-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="771ac-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="771ac-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="771ac-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="771ac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="771ac-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="771ac-113">Not supported.</span></span> |
| <span data-ttu-id="771ac-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="771ac-114">Application</span></span>                            | <span data-ttu-id="771ac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="771ac-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="771ac-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="771ac-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/branding/localizations/{locale}
```

## <a name="request-headers"></a><span data-ttu-id="771ac-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="771ac-117">Request headers</span></span>

| <span data-ttu-id="771ac-118">名称</span><span class="sxs-lookup"><span data-stu-id="771ac-118">Name</span></span>          | <span data-ttu-id="771ac-119">说明</span><span class="sxs-lookup"><span data-stu-id="771ac-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="771ac-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="771ac-120">Authorization</span></span> | <span data-ttu-id="771ac-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="771ac-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="771ac-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="771ac-123">Request body</span></span>

<span data-ttu-id="771ac-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="771ac-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="771ac-125">响应</span><span class="sxs-lookup"><span data-stu-id="771ac-125">Response</span></span>

<span data-ttu-id="771ac-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="771ac-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="771ac-128">示例</span><span class="sxs-lookup"><span data-stu-id="771ac-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="771ac-129">请求</span><span class="sxs-lookup"><span data-stu-id="771ac-129">Request</span></span>

<span data-ttu-id="771ac-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="771ac-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_organizationalbrandingproperties"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```

### <a name="response"></a><span data-ttu-id="771ac-131">响应</span><span class="sxs-lookup"><span data-stu-id="771ac-131">Response</span></span>

<span data-ttu-id="771ac-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="771ac-132">The following is an example of the response.</span></span>

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
  "description": "Delete organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
