---
title: 删除 registeredowners
description: 将用户删除为设备的已注册所有者。
localization_priority: Normal
author: michaelrm97
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7f958a1af94d74b9eee3db8f925ed1d6d9246617
ms.sourcegitcommit: 9c1abb1c87177da20e1f5bbf1fae8131ab7e4f16
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146852"
---
# <a name="delete-registeredowner"></a><span data-ttu-id="ce1f8-103">删除 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="ce1f8-103">Delete registeredOwner</span></span>

<span data-ttu-id="ce1f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce1f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce1f8-105">将用户删除为设备的已注册所有者。</span><span class="sxs-lookup"><span data-stu-id="ce1f8-105">Remove a user as a registered owner of the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce1f8-106">权限</span><span class="sxs-lookup"><span data-stu-id="ce1f8-106">Permissions</span></span>

<span data-ttu-id="ce1f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce1f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce1f8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce1f8-109">Permission type</span></span>      | <span data-ttu-id="ce1f8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce1f8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce1f8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce1f8-111">Delegated (work or school account)</span></span> |<span data-ttu-id="ce1f8-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ce1f8-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ce1f8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce1f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce1f8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce1f8-114">Not supported.</span></span>    |
|<span data-ttu-id="ce1f8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce1f8-115">Application</span></span> | <span data-ttu-id="ce1f8-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce1f8-116">Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ce1f8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce1f8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}/registeredOwners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ce1f8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce1f8-118">Request headers</span></span>
| <span data-ttu-id="ce1f8-119">名称</span><span class="sxs-lookup"><span data-stu-id="ce1f8-119">Name</span></span>       | <span data-ttu-id="ce1f8-120">类型</span><span class="sxs-lookup"><span data-stu-id="ce1f8-120">Type</span></span> | <span data-ttu-id="ce1f8-121">说明</span><span class="sxs-lookup"><span data-stu-id="ce1f8-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ce1f8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce1f8-122">Authorization</span></span>  | <span data-ttu-id="ce1f8-123">string</span><span class="sxs-lookup"><span data-stu-id="ce1f8-123">string</span></span>  | <span data-ttu-id="ce1f8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ce1f8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce1f8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce1f8-126">Request body</span></span>
<span data-ttu-id="ce1f8-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ce1f8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce1f8-128">响应</span><span class="sxs-lookup"><span data-stu-id="ce1f8-128">Response</span></span>

<span data-ttu-id="ce1f8-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ce1f8-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ce1f8-130">示例</span><span class="sxs-lookup"><span data-stu-id="ce1f8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce1f8-131">请求</span><span class="sxs-lookup"><span data-stu-id="ce1f8-131">Request</span></span>
<span data-ttu-id="ce1f8-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce1f8-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce1f8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce1f8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_registeredowners"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/devices/{id}/registeredOwners/{id}/$ref
```

---

##### <a name="response"></a><span data-ttu-id="ce1f8-134">响应</span><span class="sxs-lookup"><span data-stu-id="ce1f8-134">Response</span></span>
<span data-ttu-id="ce1f8-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ce1f8-135">Here is an example of the response.</span></span>
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
  "description": "Delete registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
