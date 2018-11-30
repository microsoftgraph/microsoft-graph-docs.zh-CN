---
title: 删除目录设置
description: 删除目录设置。
ms.openlocfilehash: 442c4f0433dd1595708b478f527bf881a055713d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046460"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="cae12-103">删除目录设置</span><span class="sxs-lookup"><span data-stu-id="cae12-103">Delete a directory setting</span></span>

> <span data-ttu-id="cae12-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cae12-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cae12-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cae12-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cae12-106">删除目录设置。</span><span class="sxs-lookup"><span data-stu-id="cae12-106">Delete a directory setting.</span></span>

> <span data-ttu-id="cae12-107">**注意**： 此 API 的 /beta 版本才适用于组。</span><span class="sxs-lookup"><span data-stu-id="cae12-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="cae12-108">此 API 的 /v1.0 版本已被重命名为*删除 groupSettings*。</span><span class="sxs-lookup"><span data-stu-id="cae12-108">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="cae12-109">权限</span><span class="sxs-lookup"><span data-stu-id="cae12-109">Permissions</span></span>
<span data-ttu-id="cae12-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cae12-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cae12-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="cae12-112">Permission type</span></span>      | <span data-ttu-id="cae12-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cae12-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cae12-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cae12-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cae12-115">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cae12-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cae12-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cae12-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cae12-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cae12-117">Not supported.</span></span>    |
|<span data-ttu-id="cae12-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="cae12-118">Application</span></span> | <span data-ttu-id="cae12-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cae12-119">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cae12-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cae12-120">HTTP request</span></span>
<span data-ttu-id="cae12-121"><!-- { "blockType": "ignored" } -->删除特定的租户范围或组设置</span><span class="sxs-lookup"><span data-stu-id="cae12-121"><!-- { "blockType": "ignored" } --> Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="cae12-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="cae12-122">Request headers</span></span>
| <span data-ttu-id="cae12-123">名称</span><span class="sxs-lookup"><span data-stu-id="cae12-123">Name</span></span>       | <span data-ttu-id="cae12-124">说明</span><span class="sxs-lookup"><span data-stu-id="cae12-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cae12-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cae12-125">Authorization</span></span>  | <span data-ttu-id="cae12-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cae12-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cae12-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cae12-128">Request body</span></span>
<span data-ttu-id="cae12-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cae12-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cae12-130">响应</span><span class="sxs-lookup"><span data-stu-id="cae12-130">Response</span></span>

<span data-ttu-id="cae12-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cae12-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cae12-133">示例</span><span class="sxs-lookup"><span data-stu-id="cae12-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cae12-134">请求</span><span class="sxs-lookup"><span data-stu-id="cae12-134">Request</span></span>
<span data-ttu-id="cae12-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cae12-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="cae12-136">响应</span><span class="sxs-lookup"><span data-stu-id="cae12-136">Response</span></span>
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
  "description": "Delete directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->