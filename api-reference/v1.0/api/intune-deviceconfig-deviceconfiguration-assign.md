---
title: assign 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 161e76abb31c4ee569cebfa5b8e33966abcc6e25
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760634"
---
# <a name="assign-action"></a><span data-ttu-id="a18d5-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="a18d5-103">assign action</span></span>

<span data-ttu-id="a18d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a18d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a18d5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a18d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a18d5-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a18d5-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a18d5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a18d5-107">Prerequisites</span></span>
<span data-ttu-id="a18d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a18d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a18d5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a18d5-110">Permission type</span></span>|<span data-ttu-id="a18d5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a18d5-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a18d5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a18d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a18d5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a18d5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a18d5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a18d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a18d5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a18d5-115">Not supported.</span></span>|
|<span data-ttu-id="a18d5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a18d5-116">Application</span></span>|<span data-ttu-id="a18d5-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a18d5-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a18d5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a18d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="a18d5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a18d5-119">Request headers</span></span>
|<span data-ttu-id="a18d5-120">标头</span><span class="sxs-lookup"><span data-stu-id="a18d5-120">Header</span></span>|<span data-ttu-id="a18d5-121">值</span><span class="sxs-lookup"><span data-stu-id="a18d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a18d5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a18d5-122">Authorization</span></span>|<span data-ttu-id="a18d5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a18d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a18d5-124">接受</span><span class="sxs-lookup"><span data-stu-id="a18d5-124">Accept</span></span>|<span data-ttu-id="a18d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a18d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a18d5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a18d5-126">Request body</span></span>
<span data-ttu-id="a18d5-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a18d5-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a18d5-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="a18d5-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a18d5-129">属性</span><span class="sxs-lookup"><span data-stu-id="a18d5-129">Property</span></span>|<span data-ttu-id="a18d5-130">类型</span><span class="sxs-lookup"><span data-stu-id="a18d5-130">Type</span></span>|<span data-ttu-id="a18d5-131">说明</span><span class="sxs-lookup"><span data-stu-id="a18d5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a18d5-132">assignments</span><span class="sxs-lookup"><span data-stu-id="a18d5-132">assignments</span></span>|<span data-ttu-id="a18d5-133">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a18d5-133">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a18d5-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a18d5-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a18d5-135">响应</span><span class="sxs-lookup"><span data-stu-id="a18d5-135">Response</span></span>
<span data-ttu-id="a18d5-136">如果成功，此操作在响应正文中返回 `200 OK` 响应代码和 [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="a18d5-136">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a18d5-137">示例</span><span class="sxs-lookup"><span data-stu-id="a18d5-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="a18d5-138">请求</span><span class="sxs-lookup"><span data-stu-id="a18d5-138">Request</span></span>
<span data-ttu-id="a18d5-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a18d5-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 333

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a18d5-140">响应</span><span class="sxs-lookup"><span data-stu-id="a18d5-140">Response</span></span>
<span data-ttu-id="a18d5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a18d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 327

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```




