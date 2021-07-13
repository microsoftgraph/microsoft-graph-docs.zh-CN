---
title: 删除 mobileAppManagementPolicy
description: 删除移动应用管理策略。
author: michaelrm97
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4676980ef37e8cf60410726ce018bb30287a58e0
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401688"
---
# <a name="delete-mobileappmanagementpolicy"></a><span data-ttu-id="84578-103">删除 mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="84578-103">Delete mobileAppManagementPolicy</span></span>

<span data-ttu-id="84578-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84578-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84578-105">删除 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="84578-105">Delete a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="84578-106">只有在策略不再有效时，才支持此操作;即 **isValid** 属性为 false 时，指示与此策略的应用程序关联的服务主体已删除。</span><span class="sxs-lookup"><span data-stu-id="84578-106">This operation is only supported when the policy is no longer valid; that is, when the **isValid** property is false, which indicates that the service principal associated with the application for this policy has been deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="84578-107">权限</span><span class="sxs-lookup"><span data-stu-id="84578-107">Permissions</span></span>

<span data-ttu-id="84578-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84578-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84578-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="84578-110">Permission type</span></span>|<span data-ttu-id="84578-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="84578-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84578-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84578-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84578-113">Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="84578-113">Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="84578-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84578-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84578-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="84578-115">Not supported.</span></span>|
|<span data-ttu-id="84578-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="84578-116">Application</span></span> | <span data-ttu-id="84578-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="84578-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84578-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84578-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/mobileAppManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="84578-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="84578-119">Request headers</span></span>

|<span data-ttu-id="84578-120">名称</span><span class="sxs-lookup"><span data-stu-id="84578-120">Name</span></span>|<span data-ttu-id="84578-121">说明</span><span class="sxs-lookup"><span data-stu-id="84578-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="84578-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="84578-122">Authorization</span></span>|<span data-ttu-id="84578-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84578-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84578-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="84578-125">Request body</span></span>

<span data-ttu-id="84578-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="84578-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84578-127">响应</span><span class="sxs-lookup"><span data-stu-id="84578-127">Response</span></span>

<span data-ttu-id="84578-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="84578-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="84578-130">示例</span><span class="sxs-lookup"><span data-stu-id="84578-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="84578-131">请求</span><span class="sxs-lookup"><span data-stu-id="84578-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_mobilitymanagementpolicy"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
```

### <a name="response"></a><span data-ttu-id="84578-132">响应</span><span class="sxs-lookup"><span data-stu-id="84578-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
