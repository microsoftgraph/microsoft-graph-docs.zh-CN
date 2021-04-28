---
title: 更新 accessReviewPolicy
description: 更新 accessReviewPolicy 对象的属性。
author: kafen
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3a4ef900a4dfc88b28dfd3d11f96804655160823
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067343"
---
# <a name="update-accessreviewpolicy"></a><span data-ttu-id="58f71-103">更新 accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="58f71-103">Update accessReviewPolicy</span></span>
<span data-ttu-id="58f71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58f71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58f71-105">更新 [accessReviewPolicy 对象](../resources/accessreviewpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="58f71-105">Update the properties of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="58f71-106">权限</span><span class="sxs-lookup"><span data-stu-id="58f71-106">Permissions</span></span>
<span data-ttu-id="58f71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58f71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58f71-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="58f71-109">Permission type</span></span>|<span data-ttu-id="58f71-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="58f71-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58f71-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58f71-111">Delegated (work or school account)</span></span>|<span data-ttu-id="58f71-112">Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="58f71-112">Policy.ReadWrite.AccessReviews</span></span>|
|<span data-ttu-id="58f71-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58f71-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58f71-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="58f71-114">Not supported.</span></span>|
|<span data-ttu-id="58f71-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="58f71-115">Application</span></span>|<span data-ttu-id="58f71-116">Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="58f71-116">Policy.ReadWrite.AccessReviews</span></span>|

## <a name="http-request"></a><span data-ttu-id="58f71-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58f71-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/accessReviewPolicy
PATCH /identityGovernance/accessReviews/policy
```

## <a name="request-headers"></a><span data-ttu-id="58f71-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="58f71-118">Request headers</span></span>
|<span data-ttu-id="58f71-119">名称</span><span class="sxs-lookup"><span data-stu-id="58f71-119">Name</span></span>|<span data-ttu-id="58f71-120">说明</span><span class="sxs-lookup"><span data-stu-id="58f71-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="58f71-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="58f71-121">Authorization</span></span>|<span data-ttu-id="58f71-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="58f71-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="58f71-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="58f71-124">Content-Type</span></span>|<span data-ttu-id="58f71-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="58f71-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="58f71-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="58f71-127">Request body</span></span>
<span data-ttu-id="58f71-128">在请求正文中，提供 [accessReviewPolicy](../resources/accessreviewpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58f71-128">In the request body, supply a JSON representation of the [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

<span data-ttu-id="58f71-129">下表显示更新 [accessReviewPolicy 时所需的属性](../resources/accessreviewpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="58f71-129">The following table shows the properties that are required when you update the [accessReviewPolicy](../resources/accessreviewpolicy.md).</span></span>

|<span data-ttu-id="58f71-130">属性</span><span class="sxs-lookup"><span data-stu-id="58f71-130">Property</span></span>|<span data-ttu-id="58f71-131">类型</span><span class="sxs-lookup"><span data-stu-id="58f71-131">Type</span></span>|<span data-ttu-id="58f71-132">说明</span><span class="sxs-lookup"><span data-stu-id="58f71-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58f71-133">isGroupOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="58f71-133">isGroupOwnerManagementEnabled</span></span>|<span data-ttu-id="58f71-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="58f71-134">Boolean</span></span>|<span data-ttu-id="58f71-135">如果 `true` 为 ，组所有者可以在他们拥有的组上创建和管理访问评审。</span><span class="sxs-lookup"><span data-stu-id="58f71-135">If `true`, group owners can create and manage access reviews on groups they own.</span></span>|



## <a name="response"></a><span data-ttu-id="58f71-136">响应</span><span class="sxs-lookup"><span data-stu-id="58f71-136">Response</span></span>

<span data-ttu-id="58f71-137">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="58f71-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="58f71-138">示例</span><span class="sxs-lookup"><span data-stu-id="58f71-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="58f71-139">请求</span><span class="sxs-lookup"><span data-stu-id="58f71-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_accessreviewpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/accessReviewPolicy
Content-Type: application/json

{
  "isGroupOwnerManagementEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="58f71-140">响应</span><span class="sxs-lookup"><span data-stu-id="58f71-140">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="request"></a><span data-ttu-id="58f71-141">请求</span><span class="sxs-lookup"><span data-stu-id="58f71-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_accessreviewpolicy_2"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/accessReviews/policy
Content-Type: application/json

{
  "isGroupOwnerManagementEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="58f71-142">响应</span><span class="sxs-lookup"><span data-stu-id="58f71-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
