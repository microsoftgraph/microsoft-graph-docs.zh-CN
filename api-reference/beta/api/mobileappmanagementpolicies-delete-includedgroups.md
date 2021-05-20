---
title: 删除 includedGroup
description: 从移动应用管理策略中包含的组列表中删除组。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7fb2c501ca1d052a6a97361faee79b06ddcb9671
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547407"
---
# <a name="delete-includedgroup"></a><span data-ttu-id="09dea-103">删除 includedGroup</span><span class="sxs-lookup"><span data-stu-id="09dea-103">Delete includedGroup</span></span>

<span data-ttu-id="09dea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09dea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09dea-105">从移动应用管理策略中包含的组列表中删除组。</span><span class="sxs-lookup"><span data-stu-id="09dea-105">Delete a group from the list of groups included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="09dea-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="09dea-106">Permissions</span></span>

<span data-ttu-id="09dea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09dea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09dea-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="09dea-109">Permission type</span></span>|<span data-ttu-id="09dea-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="09dea-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09dea-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09dea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="09dea-112">Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09dea-112">Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="09dea-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09dea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09dea-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="09dea-114">Not supported.</span></span>|
|<span data-ttu-id="09dea-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="09dea-115">Application</span></span> | <span data-ttu-id="09dea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="09dea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09dea-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09dea-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/mobileAppManagementPolicies/{id}/includedGroups/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="09dea-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="09dea-118">Request headers</span></span>

|<span data-ttu-id="09dea-119">名称</span><span class="sxs-lookup"><span data-stu-id="09dea-119">Name</span></span>|<span data-ttu-id="09dea-120">说明</span><span class="sxs-lookup"><span data-stu-id="09dea-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="09dea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="09dea-121">Authorization</span></span>|<span data-ttu-id="09dea-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="09dea-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="09dea-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="09dea-124">Request body</span></span>

<span data-ttu-id="09dea-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="09dea-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09dea-126">响应</span><span class="sxs-lookup"><span data-stu-id="09dea-126">Response</span></span>

<span data-ttu-id="09dea-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="09dea-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="09dea-129">示例</span><span class="sxs-lookup"><span data-stu-id="09dea-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="09dea-130">请求</span><span class="sxs-lookup"><span data-stu-id="09dea-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_group"
}
-->

```http
DELETE https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/1a9db3ab-0acf-4808-99ae-e8ed581cb2e0/$ref
```

### <a name="response"></a><span data-ttu-id="09dea-131">响应</span><span class="sxs-lookup"><span data-stu-id="09dea-131">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
