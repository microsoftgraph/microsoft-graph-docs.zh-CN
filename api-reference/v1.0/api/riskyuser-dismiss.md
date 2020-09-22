---
title: riskyUser：消除
description: 消除有风险的用户
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 996d64d4b370b1536d1c0af28d5479cc5cbb0e79
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051317"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="cb945-103">riskyUser：消除</span><span class="sxs-lookup"><span data-stu-id="cb945-103">riskyUser: dismiss</span></span>
<span data-ttu-id="cb945-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb945-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="cb945-105">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="cb945-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="cb945-106">消除一个或多个 [riskyUser](../resources/riskyuser.md) 对象的风险。</span><span class="sxs-lookup"><span data-stu-id="cb945-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="cb945-107">此操作将目标用户的风险级别设置为 "无"。</span><span class="sxs-lookup"><span data-stu-id="cb945-107">This action sets the targeted user's risk level to none.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb945-108">权限</span><span class="sxs-lookup"><span data-stu-id="cb945-108">Permissions</span></span>
<span data-ttu-id="cb945-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="cb945-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="cb945-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb945-111">Permission type</span></span>      | <span data-ttu-id="cb945-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb945-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb945-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb945-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cb945-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb945-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="cb945-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb945-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb945-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb945-116">Not supported.</span></span>    |
|<span data-ttu-id="cb945-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb945-117">Application</span></span> | <span data-ttu-id="cb945-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb945-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb945-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb945-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyUsers/dismiss
```

## <a name="request-headers"></a><span data-ttu-id="cb945-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb945-120">Request headers</span></span>
|<span data-ttu-id="cb945-121">名称</span><span class="sxs-lookup"><span data-stu-id="cb945-121">Name</span></span>|<span data-ttu-id="cb945-122">说明</span><span class="sxs-lookup"><span data-stu-id="cb945-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cb945-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb945-123">Authorization</span></span>|<span data-ttu-id="cb945-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cb945-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cb945-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb945-126">Content-Type</span></span>|<span data-ttu-id="cb945-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cb945-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb945-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb945-129">Request body</span></span>
<span data-ttu-id="cb945-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb945-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="cb945-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="cb945-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="cb945-132">参数</span><span class="sxs-lookup"><span data-stu-id="cb945-132">Parameter</span></span>|<span data-ttu-id="cb945-133">类型</span><span class="sxs-lookup"><span data-stu-id="cb945-133">Type</span></span>|<span data-ttu-id="cb945-134">说明</span><span class="sxs-lookup"><span data-stu-id="cb945-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb945-135">userIds</span><span class="sxs-lookup"><span data-stu-id="cb945-135">userIds</span></span>|<span data-ttu-id="cb945-136">String collection</span><span class="sxs-lookup"><span data-stu-id="cb945-136">String collection</span></span>|<span data-ttu-id="cb945-137">在请求正文中指定要消除的 userIds。</span><span class="sxs-lookup"><span data-stu-id="cb945-137">Specify the userIds to dismiss in the request body.</span></span>|



## <a name="response"></a><span data-ttu-id="cb945-138">响应</span><span class="sxs-lookup"><span data-stu-id="cb945-138">Response</span></span>

<span data-ttu-id="cb945-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cb945-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cb945-140">示例</span><span class="sxs-lookup"><span data-stu-id="cb945-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb945-141">请求</span><span class="sxs-lookup"><span data-stu-id="cb945-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "riskyuser_dismiss"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss

Content-Type: application/json
Content-length: 39

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```


### <a name="response"></a><span data-ttu-id="cb945-142">响应</span><span class="sxs-lookup"><span data-stu-id="cb945-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


