---
title: riskyUser：消除
description: 消除有风险的用户
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 25bbea620a48b22d4baef4f2e6dd9d2a5681c730
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897580"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="c7fb6-103">riskyUser：消除</span><span class="sxs-lookup"><span data-stu-id="c7fb6-103">riskyUser: dismiss</span></span>
<span data-ttu-id="c7fb6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7fb6-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="c7fb6-105">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="c7fb6-105">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="c7fb6-106">消除一个或多个[riskyUser](../resources/riskyuser.md)对象的风险。</span><span class="sxs-lookup"><span data-stu-id="c7fb6-106">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="c7fb6-107">此操作将目标用户的风险级别设置为 "无"。</span><span class="sxs-lookup"><span data-stu-id="c7fb6-107">This action sets the targeted user's risk level to none.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7fb6-108">权限</span><span class="sxs-lookup"><span data-stu-id="c7fb6-108">Permissions</span></span>
<span data-ttu-id="c7fb6-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c7fb6-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c7fb6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="c7fb6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="c7fb6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7fb6-111">Permission type</span></span>      | <span data-ttu-id="c7fb6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7fb6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7fb6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7fb6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c7fb6-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7fb6-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7fb6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7fb6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7fb6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7fb6-116">Not supported.</span></span>    |
|<span data-ttu-id="c7fb6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7fb6-117">Application</span></span> | <span data-ttu-id="c7fb6-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7fb6-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7fb6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7fb6-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyUsers/dismiss
```

## <a name="request-headers"></a><span data-ttu-id="c7fb6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7fb6-120">Request headers</span></span>
|<span data-ttu-id="c7fb6-121">名称</span><span class="sxs-lookup"><span data-stu-id="c7fb6-121">Name</span></span>|<span data-ttu-id="c7fb6-122">说明</span><span class="sxs-lookup"><span data-stu-id="c7fb6-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c7fb6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7fb6-123">Authorization</span></span>|<span data-ttu-id="c7fb6-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="c7fb6-124">Bearer {token}.</span></span> <span data-ttu-id="c7fb6-125">Required.</span><span class="sxs-lookup"><span data-stu-id="c7fb6-125">Required.</span></span>|
|<span data-ttu-id="c7fb6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7fb6-126">Content-Type</span></span>|<span data-ttu-id="c7fb6-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="c7fb6-127">application/json.</span></span> <span data-ttu-id="c7fb6-128">Required.</span><span class="sxs-lookup"><span data-stu-id="c7fb6-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7fb6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7fb6-129">Request body</span></span>
<span data-ttu-id="c7fb6-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7fb6-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c7fb6-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c7fb6-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c7fb6-132">参数</span><span class="sxs-lookup"><span data-stu-id="c7fb6-132">Parameter</span></span>|<span data-ttu-id="c7fb6-133">类型</span><span class="sxs-lookup"><span data-stu-id="c7fb6-133">Type</span></span>|<span data-ttu-id="c7fb6-134">说明</span><span class="sxs-lookup"><span data-stu-id="c7fb6-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7fb6-135">userIds</span><span class="sxs-lookup"><span data-stu-id="c7fb6-135">userIds</span></span>|<span data-ttu-id="c7fb6-136">String collection</span><span class="sxs-lookup"><span data-stu-id="c7fb6-136">String collection</span></span>|<span data-ttu-id="c7fb6-137">在请求正文中指定要消除的 userIds。</span><span class="sxs-lookup"><span data-stu-id="c7fb6-137">Specify the userIds to dismiss in the request body.</span></span>|



## <a name="response"></a><span data-ttu-id="c7fb6-138">响应</span><span class="sxs-lookup"><span data-stu-id="c7fb6-138">Response</span></span>

<span data-ttu-id="c7fb6-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c7fb6-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c7fb6-140">示例</span><span class="sxs-lookup"><span data-stu-id="c7fb6-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7fb6-141">请求</span><span class="sxs-lookup"><span data-stu-id="c7fb6-141">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="c7fb6-142">响应</span><span class="sxs-lookup"><span data-stu-id="c7fb6-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

