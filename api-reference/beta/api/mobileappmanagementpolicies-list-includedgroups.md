---
title: 列出 includedGroups
description: 获取包含在移动应用管理策略中的组列表。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d69156b2614b17037a6eba473d00e7d333868d6c
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351067"
---
# <a name="list-includedgroups"></a><span data-ttu-id="997e7-103">列出 includedGroups</span><span class="sxs-lookup"><span data-stu-id="997e7-103">List includedGroups</span></span>

<span data-ttu-id="997e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="997e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="997e7-105">获取包含在移动应用管理策略中的组列表。</span><span class="sxs-lookup"><span data-stu-id="997e7-105">Get the list of groups that are included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="997e7-106">权限</span><span class="sxs-lookup"><span data-stu-id="997e7-106">Permissions</span></span>

<span data-ttu-id="997e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="997e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="997e7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="997e7-109">Permission type</span></span>|<span data-ttu-id="997e7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="997e7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="997e7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="997e7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="997e7-112">Policy.Read.All、Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="997e7-112">Policy.Read.All, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="997e7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="997e7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="997e7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="997e7-114">Not supported.</span></span>|
|<span data-ttu-id="997e7-115">Application</span><span class="sxs-lookup"><span data-stu-id="997e7-115">Application</span></span> | <span data-ttu-id="997e7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="997e7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="997e7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="997e7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileAppManagementPolicies/{id}/includedGroups
```

## <a name="request-headers"></a><span data-ttu-id="997e7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="997e7-118">Request headers</span></span>

|<span data-ttu-id="997e7-119">名称</span><span class="sxs-lookup"><span data-stu-id="997e7-119">Name</span></span>|<span data-ttu-id="997e7-120">说明</span><span class="sxs-lookup"><span data-stu-id="997e7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="997e7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="997e7-121">Authorization</span></span>|<span data-ttu-id="997e7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="997e7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="997e7-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="997e7-124">Request body</span></span>

<span data-ttu-id="997e7-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="997e7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="997e7-126">响应</span><span class="sxs-lookup"><span data-stu-id="997e7-126">Response</span></span>

<span data-ttu-id="997e7-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="997e7-127">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="997e7-128">示例</span><span class="sxs-lookup"><span data-stu-id="997e7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="997e7-129">请求</span><span class="sxs-lookup"><span data-stu-id="997e7-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups
```

### <a name="response"></a><span data-ttu-id="997e7-130">响应</span><span class="sxs-lookup"><span data-stu-id="997e7-130">Response</span></span>

><span data-ttu-id="997e7-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="997e7-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "id": "800c583d-cc3d-4361-8e4a-3fbf668f27f4",
      "displayName": "Test Group"
    }
  ]
}
```
