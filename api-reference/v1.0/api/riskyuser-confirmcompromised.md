---
title: 'riskyUser: confirmCompromised'
description: 确认用户是否受到威胁
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f82194dff2e805fe73d11ad4301a0e2c74347335
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897587"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="e3ce8-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="e3ce8-103">riskyUser: confirmCompromised</span></span>
<span data-ttu-id="e3ce8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3ce8-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="e3ce8-105">**注意：** RiskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="e3ce8-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="e3ce8-106">确认一个或多个[riskyUser](../resources/riskyuser.md)对象已泄露。</span><span class="sxs-lookup"><span data-stu-id="e3ce8-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="e3ce8-107">此操作将目标用户的风险级别设置为 "高"。</span><span class="sxs-lookup"><span data-stu-id="e3ce8-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3ce8-108">权限</span><span class="sxs-lookup"><span data-stu-id="e3ce8-108">Permissions</span></span>
<span data-ttu-id="e3ce8-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e3ce8-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e3ce8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="e3ce8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="e3ce8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3ce8-111">Permission type</span></span>      | <span data-ttu-id="e3ce8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3ce8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3ce8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3ce8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e3ce8-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3ce8-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="e3ce8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3ce8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3ce8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3ce8-116">Not supported.</span></span>    |
|<span data-ttu-id="e3ce8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3ce8-117">Application</span></span> | <span data-ttu-id="e3ce8-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3ce8-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3ce8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3ce8-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyUsers/confirmCompromised
```

## <a name="request-headers"></a><span data-ttu-id="e3ce8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3ce8-120">Request headers</span></span>
|<span data-ttu-id="e3ce8-121">名称</span><span class="sxs-lookup"><span data-stu-id="e3ce8-121">Name</span></span>|<span data-ttu-id="e3ce8-122">说明</span><span class="sxs-lookup"><span data-stu-id="e3ce8-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e3ce8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3ce8-123">Authorization</span></span>|<span data-ttu-id="e3ce8-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="e3ce8-124">Bearer {token}.</span></span> <span data-ttu-id="e3ce8-125">Required.</span><span class="sxs-lookup"><span data-stu-id="e3ce8-125">Required.</span></span>|
|<span data-ttu-id="e3ce8-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3ce8-126">Content-Type</span></span>|<span data-ttu-id="e3ce8-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="e3ce8-127">application/json.</span></span> <span data-ttu-id="e3ce8-128">Required.</span><span class="sxs-lookup"><span data-stu-id="e3ce8-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3ce8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3ce8-129">Request body</span></span>
<span data-ttu-id="e3ce8-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3ce8-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e3ce8-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="e3ce8-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e3ce8-132">参数</span><span class="sxs-lookup"><span data-stu-id="e3ce8-132">Parameter</span></span>|<span data-ttu-id="e3ce8-133">类型</span><span class="sxs-lookup"><span data-stu-id="e3ce8-133">Type</span></span>|<span data-ttu-id="e3ce8-134">说明</span><span class="sxs-lookup"><span data-stu-id="e3ce8-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3ce8-135">userIds</span><span class="sxs-lookup"><span data-stu-id="e3ce8-135">userIds</span></span>|<span data-ttu-id="e3ce8-136">String collection</span><span class="sxs-lookup"><span data-stu-id="e3ce8-136">String collection</span></span>|<span data-ttu-id="e3ce8-137">指定要在请求正文中消除的有风险的用户 Id。</span><span class="sxs-lookup"><span data-stu-id="e3ce8-137">Specify the risky user IDs to dismiss in the request body.</span></span>|



## <a name="response"></a><span data-ttu-id="e3ce8-138">响应</span><span class="sxs-lookup"><span data-stu-id="e3ce8-138">Response</span></span>

<span data-ttu-id="e3ce8-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e3ce8-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e3ce8-140">示例</span><span class="sxs-lookup"><span data-stu-id="e3ce8-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e3ce8-141">请求</span><span class="sxs-lookup"><span data-stu-id="e3ce8-141">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="e3ce8-142">响应</span><span class="sxs-lookup"><span data-stu-id="e3ce8-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

