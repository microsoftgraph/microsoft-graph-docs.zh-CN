---
title: 删除目录设置
description: 删除目录设置。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c66335ec863460c9b2167e25a7e78850846e105c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454860"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="9697c-103">删除目录设置</span><span class="sxs-lookup"><span data-stu-id="9697c-103">Delete a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9697c-104">删除目录设置。</span><span class="sxs-lookup"><span data-stu-id="9697c-104">Delete a directory setting.</span></span>

> <span data-ttu-id="9697c-105">**注意**: 此 API 的/beta 版本仅适用于组。</span><span class="sxs-lookup"><span data-stu-id="9697c-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="9697c-106">此 API 的/v1.0 版本已重命名为*删除 groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="9697c-106">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="9697c-107">权限</span><span class="sxs-lookup"><span data-stu-id="9697c-107">Permissions</span></span>
<span data-ttu-id="9697c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9697c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9697c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9697c-110">Permission type</span></span>      | <span data-ttu-id="9697c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9697c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9697c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9697c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9697c-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9697c-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9697c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9697c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9697c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9697c-115">Not supported.</span></span>    |
|<span data-ttu-id="9697c-116">Application</span><span class="sxs-lookup"><span data-stu-id="9697c-116">Application</span></span> | <span data-ttu-id="9697c-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9697c-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9697c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9697c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="9697c-119">删除特定的租户范围或组设置</span><span class="sxs-lookup"><span data-stu-id="9697c-119">Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9697c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9697c-120">Request headers</span></span>
| <span data-ttu-id="9697c-121">名称</span><span class="sxs-lookup"><span data-stu-id="9697c-121">Name</span></span>       | <span data-ttu-id="9697c-122">说明</span><span class="sxs-lookup"><span data-stu-id="9697c-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9697c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9697c-123">Authorization</span></span>  | <span data-ttu-id="9697c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9697c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9697c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9697c-126">Request body</span></span>
<span data-ttu-id="9697c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9697c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9697c-128">响应</span><span class="sxs-lookup"><span data-stu-id="9697c-128">Response</span></span>

<span data-ttu-id="9697c-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9697c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9697c-131">示例</span><span class="sxs-lookup"><span data-stu-id="9697c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9697c-132">请求</span><span class="sxs-lookup"><span data-stu-id="9697c-132">Request</span></span>
<span data-ttu-id="9697c-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9697c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="9697c-134">响应</span><span class="sxs-lookup"><span data-stu-id="9697c-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
