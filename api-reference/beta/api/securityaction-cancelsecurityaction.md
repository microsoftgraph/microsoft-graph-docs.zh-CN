---
title: 'securityAction: cancelSecurityAction'
description: 取消安全操作。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 1b37563ffde274944dc877482602c36d2bf3a4bd
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366950"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="157af-103">securityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="157af-103">securityAction: cancelSecurityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="157af-104">取消安全操作。</span><span class="sxs-lookup"><span data-stu-id="157af-104">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="157af-105">权限</span><span class="sxs-lookup"><span data-stu-id="157af-105">Permissions</span></span>

<span data-ttu-id="157af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="157af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="157af-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="157af-108">Permission type</span></span>                        | <span data-ttu-id="157af-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="157af-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="157af-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="157af-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="157af-111">SecurityActions</span><span class="sxs-lookup"><span data-stu-id="157af-111">SecurityActions.ReadWrite.All</span></span> |
| <span data-ttu-id="157af-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="157af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="157af-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="157af-113">Not supported.</span></span> |
| <span data-ttu-id="157af-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="157af-114">Application</span></span>                            | <span data-ttu-id="157af-115">SecurityActions</span><span class="sxs-lookup"><span data-stu-id="157af-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="157af-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="157af-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="157af-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="157af-117">Request headers</span></span>

| <span data-ttu-id="157af-118">名称</span><span class="sxs-lookup"><span data-stu-id="157af-118">Name</span></span>          | <span data-ttu-id="157af-119">说明</span><span class="sxs-lookup"><span data-stu-id="157af-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="157af-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="157af-120">Authorization</span></span> | <span data-ttu-id="157af-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="157af-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="157af-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="157af-122">Request body</span></span>

<span data-ttu-id="157af-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="157af-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="157af-124">响应</span><span class="sxs-lookup"><span data-stu-id="157af-124">Response</span></span>

<span data-ttu-id="157af-p102">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="157af-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="157af-127">示例</span><span class="sxs-lookup"><span data-stu-id="157af-127">Examples</span></span>

<span data-ttu-id="157af-128">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="157af-128">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="157af-129">请求</span><span class="sxs-lookup"><span data-stu-id="157af-129">Request</span></span>

<span data-ttu-id="157af-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="157af-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```

### <a name="response"></a><span data-ttu-id="157af-131">响应</span><span class="sxs-lookup"><span data-stu-id="157af-131">Response</span></span>

<span data-ttu-id="157af-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="157af-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction: cancelSecurityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
