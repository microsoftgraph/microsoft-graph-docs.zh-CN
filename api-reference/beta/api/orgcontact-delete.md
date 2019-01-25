---
title: 删除 orgContact
description: 删除 orgContact。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8afaebd679cbf935b13cffeece2d272ca3c7ae40
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515767"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="71abb-103">删除 orgContact</span><span class="sxs-lookup"><span data-stu-id="71abb-103">Delete orgContact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71abb-104">删除 orgContact。</span><span class="sxs-lookup"><span data-stu-id="71abb-104">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="71abb-105">权限</span><span class="sxs-lookup"><span data-stu-id="71abb-105">Permissions</span></span>
<span data-ttu-id="71abb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71abb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71abb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="71abb-108">Permission type</span></span>      | <span data-ttu-id="71abb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71abb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71abb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71abb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71abb-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="71abb-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="71abb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71abb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71abb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="71abb-113">Not supported.</span></span>    |
|<span data-ttu-id="71abb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="71abb-114">Application</span></span> | <span data-ttu-id="71abb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="71abb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71abb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71abb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="71abb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="71abb-117">Request headers</span></span>
| <span data-ttu-id="71abb-118">名称</span><span class="sxs-lookup"><span data-stu-id="71abb-118">Name</span></span>       | <span data-ttu-id="71abb-119">类型</span><span class="sxs-lookup"><span data-stu-id="71abb-119">Type</span></span> | <span data-ttu-id="71abb-120">说明</span><span class="sxs-lookup"><span data-stu-id="71abb-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="71abb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="71abb-121">Authorization</span></span>  | <span data-ttu-id="71abb-122">string</span><span class="sxs-lookup"><span data-stu-id="71abb-122">string</span></span>  | <span data-ttu-id="71abb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71abb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71abb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="71abb-125">Request body</span></span>
<span data-ttu-id="71abb-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="71abb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71abb-127">响应</span><span class="sxs-lookup"><span data-stu-id="71abb-127">Response</span></span>

<span data-ttu-id="71abb-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="71abb-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71abb-130">示例</span><span class="sxs-lookup"><span data-stu-id="71abb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71abb-131">请求</span><span class="sxs-lookup"><span data-stu-id="71abb-131">Request</span></span>
<span data-ttu-id="71abb-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71abb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="71abb-133">响应</span><span class="sxs-lookup"><span data-stu-id="71abb-133">Response</span></span>
<span data-ttu-id="71abb-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="71abb-134">Here is an example of the response.</span></span> 
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
  "description": "Delete orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
