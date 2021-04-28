---
title: 删除部署
description: 删除部署对象。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 305e905c254fc2a5acf66747f147cc009b41ae6a
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067969"
---
# <a name="delete-deployment"></a><span data-ttu-id="8273f-103">删除部署</span><span class="sxs-lookup"><span data-stu-id="8273f-103">Delete deployment</span></span>
<span data-ttu-id="8273f-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="8273f-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8273f-105">删除 [部署](../resources/windowsupdates-deployment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8273f-105">Delete a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8273f-106">权限</span><span class="sxs-lookup"><span data-stu-id="8273f-106">Permissions</span></span>
<span data-ttu-id="8273f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8273f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8273f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8273f-109">Permission type</span></span>|<span data-ttu-id="8273f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8273f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8273f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8273f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8273f-112">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8273f-112">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="8273f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8273f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8273f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8273f-114">Not supported.</span></span>|
|<span data-ttu-id="8273f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8273f-115">Application</span></span>|<span data-ttu-id="8273f-116">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8273f-116">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8273f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8273f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /admin/windows/updates/deployments/{deploymentId}
```

## <a name="request-headers"></a><span data-ttu-id="8273f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8273f-118">Request headers</span></span>
|<span data-ttu-id="8273f-119">名称</span><span class="sxs-lookup"><span data-stu-id="8273f-119">Name</span></span>|<span data-ttu-id="8273f-120">说明</span><span class="sxs-lookup"><span data-stu-id="8273f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8273f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8273f-121">Authorization</span></span>|<span data-ttu-id="8273f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8273f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8273f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8273f-124">Request body</span></span>
<span data-ttu-id="8273f-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8273f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8273f-126">响应</span><span class="sxs-lookup"><span data-stu-id="8273f-126">Response</span></span>

<span data-ttu-id="8273f-p103">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8273f-p103">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8273f-129">示例</span><span class="sxs-lookup"><span data-stu-id="8273f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8273f-130">请求</span><span class="sxs-lookup"><span data-stu-id="8273f-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_deployment"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}
```


### <a name="response"></a><span data-ttu-id="8273f-131">响应</span><span class="sxs-lookup"><span data-stu-id="8273f-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

