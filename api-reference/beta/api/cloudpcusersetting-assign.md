---
title: cloudPcUserSetting：assign
description: 将云电脑用户设置分配给用户组。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 987ecf4ee31b2ade7baf08246542b13d14a3a6da
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993643"
---
# <a name="cloudpcusersetting-assign"></a><span data-ttu-id="c85c5-103">cloudPcUserSetting：assign</span><span class="sxs-lookup"><span data-stu-id="c85c5-103">cloudPcUserSetting: assign</span></span>

<span data-ttu-id="c85c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c85c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c85c5-105">将 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 分配给用户组。</span><span class="sxs-lookup"><span data-stu-id="c85c5-105">Assign a [cloudPcUserSetting](../resources/cloudpcusersetting.md) to user groups.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="c85c5-106">权限</span><span class="sxs-lookup"><span data-stu-id="c85c5-106">Permissions</span></span>

<span data-ttu-id="c85c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c85c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c85c5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c85c5-109">Permission type</span></span>|<span data-ttu-id="c85c5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c85c5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c85c5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c85c5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c85c5-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c85c5-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="c85c5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c85c5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c85c5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c85c5-114">Not supported.</span></span>|
|<span data-ttu-id="c85c5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c85c5-115">Application</span></span>|<span data-ttu-id="c85c5-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c85c5-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c85c5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c85c5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/userSettings/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="c85c5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c85c5-118">Request headers</span></span>

|<span data-ttu-id="c85c5-119">名称</span><span class="sxs-lookup"><span data-stu-id="c85c5-119">Name</span></span>|<span data-ttu-id="c85c5-120">说明</span><span class="sxs-lookup"><span data-stu-id="c85c5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c85c5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c85c5-121">Authorization</span></span>|<span data-ttu-id="c85c5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c85c5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c85c5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c85c5-124">Content-Type</span></span>|<span data-ttu-id="c85c5-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c85c5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c85c5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c85c5-127">Request body</span></span>

<span data-ttu-id="c85c5-128">在请求正文中，提供 [cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c85c5-128">In the request body, supply a JSON representation of the [cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) object.</span></span>

<span data-ttu-id="c85c5-129">下表显示创建 [cloudPcUserSettingAssignment 时所需的属性](../resources/cloudpcusersettingassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="c85c5-129">The following table shows the properties that are required when you create the [cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md).</span></span>

|<span data-ttu-id="c85c5-130">属性</span><span class="sxs-lookup"><span data-stu-id="c85c5-130">Property</span></span>|<span data-ttu-id="c85c5-131">类型</span><span class="sxs-lookup"><span data-stu-id="c85c5-131">Type</span></span>|<span data-ttu-id="c85c5-132">说明</span><span class="sxs-lookup"><span data-stu-id="c85c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c85c5-133">target</span><span class="sxs-lookup"><span data-stu-id="c85c5-133">target</span></span>|[<span data-ttu-id="c85c5-134">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c85c5-134">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="c85c5-135">预配策略的分配目标。</span><span class="sxs-lookup"><span data-stu-id="c85c5-135">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="c85c5-136">目前，唯一支持的目标为用户组。</span><span class="sxs-lookup"><span data-stu-id="c85c5-136">Currently, the only target supported is a user group.</span></span>|

## <a name="response"></a><span data-ttu-id="c85c5-137">响应</span><span class="sxs-lookup"><span data-stu-id="c85c5-137">Response</span></span>

<span data-ttu-id="c85c5-138">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c85c5-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c85c5-139">示例</span><span class="sxs-lookup"><span data-stu-id="c85c5-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c85c5-140">请求</span><span class="sxs-lookup"><span data-stu-id="c85c5-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "cloudpcusersetting_assign"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff/assign
Content-Type: application/json
Content-length: 254

{
  "assignments": [
    {
      "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
      "target":{
        "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
        "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
        }
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="c85c5-141">响应</span><span class="sxs-lookup"><span data-stu-id="c85c5-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
