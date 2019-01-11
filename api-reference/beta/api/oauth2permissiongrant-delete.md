---
title: 删除 oAuth2PermissionGrant
description: 删除 oAuth2PermissionGrant。
localization_priority: Normal
ms.openlocfilehash: 8eed0c8d2179af6fe199137cfeb7e386a97f733c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813816"
---
# <a name="delete-oauth2permissiongrant"></a><span data-ttu-id="0f5d4-103">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="0f5d4-103">Delete oAuth2PermissionGrant</span></span>

> <span data-ttu-id="0f5d4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0f5d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f5d4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0f5d4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0f5d4-106">删除 oAuth2PermissionGrant。</span><span class="sxs-lookup"><span data-stu-id="0f5d4-106">Delete an oAuth2PermissionGrant.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f5d4-107">权限</span><span class="sxs-lookup"><span data-stu-id="0f5d4-107">Permissions</span></span>
<span data-ttu-id="0f5d4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f5d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0f5d4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f5d4-110">Permission type</span></span>      | <span data-ttu-id="0f5d4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0f5d4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f5d4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f5d4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0f5d4-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0f5d4-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0f5d4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f5d4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f5d4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f5d4-115">Not supported.</span></span>    |
|<span data-ttu-id="0f5d4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f5d4-116">Application</span></span> | <span data-ttu-id="0f5d4-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f5d4-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f5d4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f5d4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /oAuth2Permissiongrants/{id}
DELETE /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
DELETE /drive/root/createdByUser/oAuth2Permissiongrants/{id}

```
## <a name="request-headers"></a><span data-ttu-id="0f5d4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f5d4-119">Request headers</span></span>
| <span data-ttu-id="0f5d4-120">名称</span><span class="sxs-lookup"><span data-stu-id="0f5d4-120">Name</span></span>       | <span data-ttu-id="0f5d4-121">类型</span><span class="sxs-lookup"><span data-stu-id="0f5d4-121">Type</span></span> | <span data-ttu-id="0f5d4-122">说明</span><span class="sxs-lookup"><span data-stu-id="0f5d4-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0f5d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f5d4-123">Authorization</span></span>  | <span data-ttu-id="0f5d4-124">string</span><span class="sxs-lookup"><span data-stu-id="0f5d4-124">string</span></span>  | <span data-ttu-id="0f5d4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0f5d4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f5d4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f5d4-127">Request body</span></span>
<span data-ttu-id="0f5d4-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0f5d4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f5d4-129">响应</span><span class="sxs-lookup"><span data-stu-id="0f5d4-129">Response</span></span>

<span data-ttu-id="0f5d4-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0f5d4-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f5d4-132">示例</span><span class="sxs-lookup"><span data-stu-id="0f5d4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f5d4-133">请求</span><span class="sxs-lookup"><span data-stu-id="0f5d4-133">Request</span></span>
<span data-ttu-id="0f5d4-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f5d4-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2Permissiongrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="0f5d4-135">响应</span><span class="sxs-lookup"><span data-stu-id="0f5d4-135">Response</span></span>
<span data-ttu-id="0f5d4-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0f5d4-136">Here is an example of the response.</span></span> 
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
  "description": "Delete oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
