---
title: 列出 includedGroups
description: 获取包含在移动设备管理策略中的组列表。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9f29a263601958820d69fe51f146d34eb5a079c6
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401461"
---
# <a name="list-includedgroups"></a><span data-ttu-id="11214-103">列出 includedGroups</span><span class="sxs-lookup"><span data-stu-id="11214-103">List includedGroups</span></span>

<span data-ttu-id="11214-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11214-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11214-105">获取包含在移动设备管理策略中的组列表。</span><span class="sxs-lookup"><span data-stu-id="11214-105">Get the list of groups that are included in a mobile device management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="11214-106">权限</span><span class="sxs-lookup"><span data-stu-id="11214-106">Permissions</span></span>

<span data-ttu-id="11214-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11214-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11214-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="11214-109">Permission type</span></span>|<span data-ttu-id="11214-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="11214-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11214-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11214-111">Delegated (work or school account)</span></span>|<span data-ttu-id="11214-112">Policy.Read.All、Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="11214-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="11214-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11214-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11214-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="11214-114">Not supported.</span></span>|
|<span data-ttu-id="11214-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="11214-115">Application</span></span> | <span data-ttu-id="11214-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="11214-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11214-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11214-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileDeviceManagementPolicies/{id}/includedGroups
```

## <a name="request-headers"></a><span data-ttu-id="11214-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="11214-118">Request headers</span></span>

|<span data-ttu-id="11214-119">名称</span><span class="sxs-lookup"><span data-stu-id="11214-119">Name</span></span>|<span data-ttu-id="11214-120">说明</span><span class="sxs-lookup"><span data-stu-id="11214-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="11214-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="11214-121">Authorization</span></span>|<span data-ttu-id="11214-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="11214-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11214-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="11214-124">Request body</span></span>

<span data-ttu-id="11214-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="11214-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11214-126">响应</span><span class="sxs-lookup"><span data-stu-id="11214-126">Response</span></span>

<span data-ttu-id="11214-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="11214-127">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11214-128">示例</span><span class="sxs-lookup"><span data-stu-id="11214-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11214-129">请求</span><span class="sxs-lookup"><span data-stu-id="11214-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups
```

### <a name="response"></a><span data-ttu-id="11214-130">响应</span><span class="sxs-lookup"><span data-stu-id="11214-130">Response</span></span>

><span data-ttu-id="11214-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="11214-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
