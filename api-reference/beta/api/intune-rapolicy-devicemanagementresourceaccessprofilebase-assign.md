---
title: assign 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c108a7fd3ab1473d5312cfaa224a7f342c5c7248
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152038"
---
# <a name="assign-action"></a><span data-ttu-id="69727-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="69727-103">assign action</span></span>

<span data-ttu-id="69727-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69727-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69727-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69727-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69727-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69727-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69727-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="69727-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69727-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="69727-108">Prerequisites</span></span>
<span data-ttu-id="69727-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69727-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69727-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="69727-111">Permission type</span></span>|<span data-ttu-id="69727-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69727-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69727-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69727-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69727-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69727-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="69727-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69727-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69727-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="69727-116">Not supported.</span></span>|
|<span data-ttu-id="69727-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="69727-117">Application</span></span>|<span data-ttu-id="69727-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69727-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="69727-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69727-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="69727-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="69727-120">Request headers</span></span>
|<span data-ttu-id="69727-121">标头</span><span class="sxs-lookup"><span data-stu-id="69727-121">Header</span></span>|<span data-ttu-id="69727-122">值</span><span class="sxs-lookup"><span data-stu-id="69727-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69727-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69727-123">Authorization</span></span>|<span data-ttu-id="69727-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="69727-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69727-125">接受</span><span class="sxs-lookup"><span data-stu-id="69727-125">Accept</span></span>|<span data-ttu-id="69727-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69727-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69727-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="69727-127">Request body</span></span>
<span data-ttu-id="69727-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69727-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="69727-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="69727-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="69727-130">属性</span><span class="sxs-lookup"><span data-stu-id="69727-130">Property</span></span>|<span data-ttu-id="69727-131">类型</span><span class="sxs-lookup"><span data-stu-id="69727-131">Type</span></span>|<span data-ttu-id="69727-132">说明</span><span class="sxs-lookup"><span data-stu-id="69727-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69727-133">assignments</span><span class="sxs-lookup"><span data-stu-id="69727-133">assignments</span></span>|<span data-ttu-id="69727-134">[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="69727-134">[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) collection</span></span>|<span data-ttu-id="69727-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="69727-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="69727-136">响应</span><span class="sxs-lookup"><span data-stu-id="69727-136">Response</span></span>
<span data-ttu-id="69727-137">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="69727-137">If successful, this action returns a `200 OK` response code and a [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69727-138">示例</span><span class="sxs-lookup"><span data-stu-id="69727-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="69727-139">请求</span><span class="sxs-lookup"><span data-stu-id="69727-139">Request</span></span>
<span data-ttu-id="69727-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69727-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}/assign

Content-type: application/json
Content-length: 591

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
      "id": "4ebb8d4e-8d4e-4ebb-4e8d-bb4e4e8dbb4e",
      "intent": "remove",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      },
      "sourceId": "Source Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="69727-141">响应</span><span class="sxs-lookup"><span data-stu-id="69727-141">Response</span></span>
<span data-ttu-id="69727-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69727-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 585

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementResourceAccessProfileAssignment",
      "id": "4ebb8d4e-8d4e-4ebb-4e8d-bb4e4e8dbb4e",
      "intent": "remove",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      },
      "sourceId": "Source Id value"
    }
  ]
}
```




