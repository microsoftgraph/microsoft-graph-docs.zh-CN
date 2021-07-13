---
title: 添加 includedGroups
description: 添加要包含在移动应用管理策略中的组。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3ec6ddda47493892c698c210dd0408f0cd1dfb27
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401650"
---
# <a name="add-includedgroups"></a><span data-ttu-id="643b1-103">添加 includedGroups</span><span class="sxs-lookup"><span data-stu-id="643b1-103">Add includedGroups</span></span>

<span data-ttu-id="643b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="643b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="643b1-105">添加要包含在移动应用管理策略中的组。</span><span class="sxs-lookup"><span data-stu-id="643b1-105">Add groups to be included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="643b1-106">权限</span><span class="sxs-lookup"><span data-stu-id="643b1-106">Permissions</span></span>
<span data-ttu-id="643b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="643b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="643b1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="643b1-109">Permission type</span></span>|<span data-ttu-id="643b1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="643b1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="643b1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="643b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="643b1-112">Policy.Read.All、Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="643b1-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="643b1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="643b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="643b1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="643b1-114">Not supported.</span></span>|
|<span data-ttu-id="643b1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="643b1-115">Application</span></span> | <span data-ttu-id="643b1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="643b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="643b1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="643b1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /policies/mobileAppManagementPolicies/{id}/includedGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="643b1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="643b1-118">Request headers</span></span>
|<span data-ttu-id="643b1-119">名称</span><span class="sxs-lookup"><span data-stu-id="643b1-119">Name</span></span>|<span data-ttu-id="643b1-120">说明</span><span class="sxs-lookup"><span data-stu-id="643b1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="643b1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="643b1-121">Authorization</span></span>|<span data-ttu-id="643b1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="643b1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="643b1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="643b1-124">Content-Type</span></span>|<span data-ttu-id="643b1-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="643b1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="643b1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="643b1-127">Request body</span></span>
<span data-ttu-id="643b1-128">在请求正文中，提供 group 对象的 JSON [表示](../resources/group.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="643b1-128">In the request body, supply a JSON representation of the [group](../resources/group.md) object.</span></span>

<span data-ttu-id="643b1-129">下表显示添加组 时所需的 [属性](../resources/group.md)。</span><span class="sxs-lookup"><span data-stu-id="643b1-129">The following table shows the properties that are required when you add the [group](../resources/group.md).</span></span>

|<span data-ttu-id="643b1-130">属性</span><span class="sxs-lookup"><span data-stu-id="643b1-130">Property</span></span>|<span data-ttu-id="643b1-131">类型</span><span class="sxs-lookup"><span data-stu-id="643b1-131">Type</span></span>|<span data-ttu-id="643b1-132">说明</span><span class="sxs-lookup"><span data-stu-id="643b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="643b1-133">id</span><span class="sxs-lookup"><span data-stu-id="643b1-133">id</span></span>|<span data-ttu-id="643b1-134">String</span><span class="sxs-lookup"><span data-stu-id="643b1-134">String</span></span>|<span data-ttu-id="643b1-135">组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="643b1-135">The unique identifier for the group.</span></span>|

## <a name="response"></a><span data-ttu-id="643b1-136">响应</span><span class="sxs-lookup"><span data-stu-id="643b1-136">Response</span></span>

<span data-ttu-id="643b1-137">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [group](../resources/group.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="643b1-137">If successful, this method returns a `204 No Content` response code and a [group](../resources/group.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="643b1-138">示例</span><span class="sxs-lookup"><span data-stu-id="643b1-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="643b1-139">请求</span><span class="sxs-lookup"><span data-stu-id="643b1-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
}
-->

``` http
POST https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/$ref
Content-Type: application/json

{
  "@odata.id": "https://graph.microsoft.com/odata/groups('1a9db3ab-0acf-4808-99ae-e8ed581cb2e0')"
}
```

### <a name="response"></a><span data-ttu-id="643b1-140">响应</span><span class="sxs-lookup"><span data-stu-id="643b1-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
