---
title: 更新 oAuth2PermissionGrant
description: 更新 oAuth2PermissionGrant 对象的属性。
localization_priority: Normal
ms.openlocfilehash: 3c01d62dfb7c0c6906ff860656ee87b5f6d40aed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822349"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="44b87-103">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="44b87-103">Update oAuth2PermissionGrant</span></span>

> <span data-ttu-id="44b87-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="44b87-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44b87-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="44b87-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44b87-106">更新 oAuth2PermissionGrant 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="44b87-106">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="44b87-107">权限</span><span class="sxs-lookup"><span data-stu-id="44b87-107">Permissions</span></span>

<span data-ttu-id="44b87-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44b87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="44b87-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="44b87-110">Permission type</span></span>      | <span data-ttu-id="44b87-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44b87-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44b87-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44b87-112">Delegated (work or school account)</span></span> | <span data-ttu-id="44b87-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="44b87-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="44b87-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44b87-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44b87-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="44b87-115">Not supported.</span></span>    |
|<span data-ttu-id="44b87-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="44b87-116">Application</span></span> | <span data-ttu-id="44b87-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44b87-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44b87-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44b87-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="44b87-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="44b87-119">Request headers</span></span>
| <span data-ttu-id="44b87-120">名称</span><span class="sxs-lookup"><span data-stu-id="44b87-120">Name</span></span>       | <span data-ttu-id="44b87-121">类型</span><span class="sxs-lookup"><span data-stu-id="44b87-121">Type</span></span> | <span data-ttu-id="44b87-122">说明</span><span class="sxs-lookup"><span data-stu-id="44b87-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="44b87-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44b87-123">Authorization</span></span>  | <span data-ttu-id="44b87-124">string</span><span class="sxs-lookup"><span data-stu-id="44b87-124">string</span></span>  | <span data-ttu-id="44b87-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="44b87-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44b87-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="44b87-127">Request body</span></span>
<span data-ttu-id="44b87-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="44b87-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="44b87-131">属性</span><span class="sxs-lookup"><span data-stu-id="44b87-131">Property</span></span>     | <span data-ttu-id="44b87-132">类型</span><span class="sxs-lookup"><span data-stu-id="44b87-132">Type</span></span>   |<span data-ttu-id="44b87-133">说明</span><span class="sxs-lookup"><span data-stu-id="44b87-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44b87-134">scope</span><span class="sxs-lookup"><span data-stu-id="44b87-134">scope</span></span>|<span data-ttu-id="44b87-135">字符串</span><span class="sxs-lookup"><span data-stu-id="44b87-135">String</span></span>| <span data-ttu-id="44b87-136">OAuth 2.0 访问令牌中指定资源应用程序应产生预期范围声明的值。</span><span class="sxs-lookup"><span data-stu-id="44b87-136">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="44b87-137">响应</span><span class="sxs-lookup"><span data-stu-id="44b87-137">Response</span></span>

<span data-ttu-id="44b87-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="44b87-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44b87-140">示例</span><span class="sxs-lookup"><span data-stu-id="44b87-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44b87-141">请求</span><span class="sxs-lookup"><span data-stu-id="44b87-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_oAuth2Permissiongrant"
}-->
```http
PATCH https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
Content-type: application/json
Content-length: 30

{
  "scope": "scope-value"
}
```
##### <a name="response"></a><span data-ttu-id="44b87-142">响应</span><span class="sxs-lookup"><span data-stu-id="44b87-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
