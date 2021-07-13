---
title: 删除 includeGroup
description: 从移动设备管理策略中包含的组列表中删除组。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5fb051f94ec95d5fea05b19a9273a3ec6cf0d349
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401605"
---
# <a name="delete-includedgroup"></a><span data-ttu-id="ba14b-103">删除 includedGroup</span><span class="sxs-lookup"><span data-stu-id="ba14b-103">Delete includedGroup</span></span>

<span data-ttu-id="ba14b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba14b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba14b-105">从移动设备管理策略中包含的组列表中删除组。</span><span class="sxs-lookup"><span data-stu-id="ba14b-105">Delete a group from the list of groups included in a mobile device management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba14b-106">权限</span><span class="sxs-lookup"><span data-stu-id="ba14b-106">Permissions</span></span>

<span data-ttu-id="ba14b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba14b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba14b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba14b-109">Permission type</span></span>|<span data-ttu-id="ba14b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba14b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba14b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba14b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ba14b-112">Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="ba14b-112">Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="ba14b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba14b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba14b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba14b-114">Not supported.</span></span>|
|<span data-ttu-id="ba14b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba14b-115">Application</span></span> | <span data-ttu-id="ba14b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba14b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba14b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba14b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/mobileDeviceManagementPolicies/{id}/includedGroups/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ba14b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba14b-118">Request headers</span></span>

|<span data-ttu-id="ba14b-119">名称</span><span class="sxs-lookup"><span data-stu-id="ba14b-119">Name</span></span>|<span data-ttu-id="ba14b-120">说明</span><span class="sxs-lookup"><span data-stu-id="ba14b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ba14b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba14b-121">Authorization</span></span>|<span data-ttu-id="ba14b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ba14b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba14b-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba14b-124">Request body</span></span>

<span data-ttu-id="ba14b-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba14b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba14b-126">响应</span><span class="sxs-lookup"><span data-stu-id="ba14b-126">Response</span></span>

<span data-ttu-id="ba14b-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ba14b-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba14b-129">示例</span><span class="sxs-lookup"><span data-stu-id="ba14b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba14b-130">请求</span><span class="sxs-lookup"><span data-stu-id="ba14b-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ba14b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba14b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef/$ref
```
# <a name="c"></a>[<span data-ttu-id="ba14b-132">C#</span><span class="sxs-lookup"><span data-stu-id="ba14b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba14b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba14b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba14b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba14b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba14b-135">Java</span><span class="sxs-lookup"><span data-stu-id="ba14b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ba14b-136">响应</span><span class="sxs-lookup"><span data-stu-id="ba14b-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
