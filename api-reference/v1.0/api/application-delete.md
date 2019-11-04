---
title: 删除应用程序
description: 删除 application 对象。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ecaafbaaa8558d8e9d86d45a75f824272fb6a14
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939731"
---
# <a name="delete-application"></a><span data-ttu-id="2812b-103">删除应用程序</span><span class="sxs-lookup"><span data-stu-id="2812b-103">Delete application</span></span>

<span data-ttu-id="2812b-104">删除[application](../resources/application.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2812b-104">Delete an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2812b-105">权限</span><span class="sxs-lookup"><span data-stu-id="2812b-105">Permissions</span></span>
<span data-ttu-id="2812b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2812b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2812b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2812b-108">Permission type</span></span>      | <span data-ttu-id="2812b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2812b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2812b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2812b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2812b-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2812b-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2812b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2812b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2812b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2812b-113">Not supported.</span></span>    |
|<span data-ttu-id="2812b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2812b-114">Application</span></span> | <span data-ttu-id="2812b-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2812b-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2812b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2812b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2812b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2812b-117">Request headers</span></span>
| <span data-ttu-id="2812b-118">名称</span><span class="sxs-lookup"><span data-stu-id="2812b-118">Name</span></span>       | <span data-ttu-id="2812b-119">类型</span><span class="sxs-lookup"><span data-stu-id="2812b-119">Type</span></span> | <span data-ttu-id="2812b-120">说明</span><span class="sxs-lookup"><span data-stu-id="2812b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2812b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2812b-121">Authorization</span></span>  | <span data-ttu-id="2812b-122">string</span><span class="sxs-lookup"><span data-stu-id="2812b-122">string</span></span>  | <span data-ttu-id="2812b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2812b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2812b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2812b-125">Request body</span></span>
<span data-ttu-id="2812b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2812b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2812b-127">响应</span><span class="sxs-lookup"><span data-stu-id="2812b-127">Response</span></span>

<span data-ttu-id="2812b-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2812b-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2812b-130">示例</span><span class="sxs-lookup"><span data-stu-id="2812b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2812b-131">请求</span><span class="sxs-lookup"><span data-stu-id="2812b-131">Request</span></span>
<span data-ttu-id="2812b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2812b-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}
```

##### <a name="response"></a><span data-ttu-id="2812b-133">响应</span><span class="sxs-lookup"><span data-stu-id="2812b-133">Response</span></span>
<span data-ttu-id="2812b-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2812b-134">Here is an example of the response.</span></span> 
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
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
