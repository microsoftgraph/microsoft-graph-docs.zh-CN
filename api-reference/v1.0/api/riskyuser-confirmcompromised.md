---
title: riskyUser：confirmComprom一
description: 确认用户遭到入侵
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dbf80b5642616f9c48fbd3e3b80121ed77566a15
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719991"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="6f200-103">riskyUser：confirmComprom一</span><span class="sxs-lookup"><span data-stu-id="6f200-103">riskyUser: confirmCompromised</span></span>
<span data-ttu-id="6f200-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f200-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="6f200-105">**注意：** riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="6f200-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="6f200-106">确认一个或多个 [riskyUser](../resources/riskyuser.md) 对象受到威胁。</span><span class="sxs-lookup"><span data-stu-id="6f200-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="6f200-107">此操作将目标用户的风险级别设置得较高。</span><span class="sxs-lookup"><span data-stu-id="6f200-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f200-108">权限</span><span class="sxs-lookup"><span data-stu-id="6f200-108">Permissions</span></span>
<span data-ttu-id="6f200-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="6f200-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="6f200-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f200-111">Permission type</span></span>      | <span data-ttu-id="6f200-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6f200-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f200-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f200-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6f200-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f200-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="6f200-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f200-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f200-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f200-116">Not supported.</span></span>    |
|<span data-ttu-id="6f200-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f200-117">Application</span></span> | <span data-ttu-id="6f200-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f200-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f200-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f200-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyUsers/confirmCompromised
```

## <a name="request-headers"></a><span data-ttu-id="6f200-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f200-120">Request headers</span></span>
|<span data-ttu-id="6f200-121">名称</span><span class="sxs-lookup"><span data-stu-id="6f200-121">Name</span></span>|<span data-ttu-id="6f200-122">说明</span><span class="sxs-lookup"><span data-stu-id="6f200-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6f200-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f200-123">Authorization</span></span>|<span data-ttu-id="6f200-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6f200-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6f200-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6f200-126">Content-Type</span></span>|<span data-ttu-id="6f200-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6f200-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f200-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f200-129">Request body</span></span>
<span data-ttu-id="6f200-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f200-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6f200-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="6f200-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6f200-132">参数</span><span class="sxs-lookup"><span data-stu-id="6f200-132">Parameter</span></span>|<span data-ttu-id="6f200-133">类型</span><span class="sxs-lookup"><span data-stu-id="6f200-133">Type</span></span>|<span data-ttu-id="6f200-134">说明</span><span class="sxs-lookup"><span data-stu-id="6f200-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f200-135">userIds</span><span class="sxs-lookup"><span data-stu-id="6f200-135">userIds</span></span>|<span data-ttu-id="6f200-136">String 集合</span><span class="sxs-lookup"><span data-stu-id="6f200-136">String collection</span></span>|<span data-ttu-id="6f200-137">指定在请求正文中要消除的风险用户 ID。</span><span class="sxs-lookup"><span data-stu-id="6f200-137">Specify the risky user IDs to dismiss in the request body.</span></span>|



## <a name="response"></a><span data-ttu-id="6f200-138">响应</span><span class="sxs-lookup"><span data-stu-id="6f200-138">Response</span></span>

<span data-ttu-id="6f200-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6f200-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6f200-140">示例</span><span class="sxs-lookup"><span data-stu-id="6f200-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6f200-141">请求</span><span class="sxs-lookup"><span data-stu-id="6f200-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "riskyuser_confirmcompromised"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised
Content-Type: application/json
Content-length: 39

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```


### <a name="response"></a><span data-ttu-id="6f200-142">响应</span><span class="sxs-lookup"><span data-stu-id="6f200-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


