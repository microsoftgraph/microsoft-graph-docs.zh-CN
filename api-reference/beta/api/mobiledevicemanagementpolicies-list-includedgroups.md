---
title: 列出 includedGroups
description: 获取包含在移动设备管理策略中的组列表。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2b83a7c797d790600aa391712e1deb70b5639cf7
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547323"
---
# <a name="list-includedgroups"></a><span data-ttu-id="74e56-103">列出 includedGroups</span><span class="sxs-lookup"><span data-stu-id="74e56-103">List includedGroups</span></span>

<span data-ttu-id="74e56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74e56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74e56-105">获取包含在移动设备管理策略中的组列表。</span><span class="sxs-lookup"><span data-stu-id="74e56-105">Get the list of groups that are included in a mobile device management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="74e56-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="74e56-106">Permissions</span></span>

<span data-ttu-id="74e56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74e56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74e56-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="74e56-109">Permission type</span></span>|<span data-ttu-id="74e56-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74e56-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74e56-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74e56-111">Delegated (work or school account)</span></span>|<span data-ttu-id="74e56-112">Policy.Read.All、Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74e56-112">Policy.Read.All, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="74e56-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74e56-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74e56-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="74e56-114">Not supported.</span></span>|
|<span data-ttu-id="74e56-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="74e56-115">Application</span></span> | <span data-ttu-id="74e56-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="74e56-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74e56-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74e56-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileDeviceManagementPolicies/{id}/includedGroups
```

## <a name="request-headers"></a><span data-ttu-id="74e56-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="74e56-118">Request headers</span></span>

|<span data-ttu-id="74e56-119">名称</span><span class="sxs-lookup"><span data-stu-id="74e56-119">Name</span></span>|<span data-ttu-id="74e56-120">说明</span><span class="sxs-lookup"><span data-stu-id="74e56-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="74e56-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="74e56-121">Authorization</span></span>|<span data-ttu-id="74e56-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="74e56-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74e56-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="74e56-124">Request body</span></span>

<span data-ttu-id="74e56-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="74e56-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74e56-126">响应</span><span class="sxs-lookup"><span data-stu-id="74e56-126">Response</span></span>

<span data-ttu-id="74e56-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="74e56-127">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="74e56-128">示例</span><span class="sxs-lookup"><span data-stu-id="74e56-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="74e56-129">请求</span><span class="sxs-lookup"><span data-stu-id="74e56-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups
```

### <a name="response"></a><span data-ttu-id="74e56-130">响应</span><span class="sxs-lookup"><span data-stu-id="74e56-130">Response</span></span>

><span data-ttu-id="74e56-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="74e56-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.group)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef",
      "displayName": "Test MDM Group"
    }
  ]
}
```
