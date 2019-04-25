---
title: 删除组设置
description: 删除组设置。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 32bdd6b2856a96377859d523767f198779d23497
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525647"
---
# <a name="delete-a-group-setting"></a><span data-ttu-id="cb9ef-103">删除组设置</span><span class="sxs-lookup"><span data-stu-id="cb9ef-103">Delete a group setting</span></span>

<span data-ttu-id="cb9ef-104">删除组设置。</span><span class="sxs-lookup"><span data-stu-id="cb9ef-104">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb9ef-105">权限</span><span class="sxs-lookup"><span data-stu-id="cb9ef-105">Permissions</span></span>

<span data-ttu-id="cb9ef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb9ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cb9ef-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb9ef-108">Permission type</span></span>      | <span data-ttu-id="cb9ef-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb9ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb9ef-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb9ef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cb9ef-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cb9ef-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cb9ef-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb9ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb9ef-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb9ef-113">Not supported.</span></span>    |
|<span data-ttu-id="cb9ef-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb9ef-114">Application</span></span> | <span data-ttu-id="cb9ef-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb9ef-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb9ef-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb9ef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="cb9ef-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb9ef-117">Request headers</span></span>

| <span data-ttu-id="cb9ef-118">名称</span><span class="sxs-lookup"><span data-stu-id="cb9ef-118">Name</span></span> | <span data-ttu-id="cb9ef-119">说明</span><span class="sxs-lookup"><span data-stu-id="cb9ef-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="cb9ef-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb9ef-120">Authorization</span></span>  | <span data-ttu-id="cb9ef-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cb9ef-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cb9ef-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb9ef-123">Content-Type</span></span>  | <span data-ttu-id="cb9ef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cb9ef-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb9ef-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb9ef-125">Request body</span></span>
<span data-ttu-id="cb9ef-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cb9ef-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb9ef-127">响应</span><span class="sxs-lookup"><span data-stu-id="cb9ef-127">Response</span></span>

<span data-ttu-id="cb9ef-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cb9ef-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb9ef-130">示例</span><span class="sxs-lookup"><span data-stu-id="cb9ef-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb9ef-131">请求</span><span class="sxs-lookup"><span data-stu-id="cb9ef-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="cb9ef-132">响应</span><span class="sxs-lookup"><span data-stu-id="cb9ef-132">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
