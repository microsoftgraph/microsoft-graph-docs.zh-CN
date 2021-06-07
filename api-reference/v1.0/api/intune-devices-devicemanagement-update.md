---
title: 更新 deviceManagement
description: 更新 deviceManagement 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c13988e02ed5edcefb9bc830304359dce469d8c3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754325"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="b7d53-103">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="b7d53-103">Update deviceManagement</span></span>

<span data-ttu-id="b7d53-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7d53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7d53-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7d53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7d53-106">更新 [deviceManagement](../resources/intune-devices-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b7d53-106">Update the properties of a [deviceManagement](../resources/intune-devices-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7d53-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b7d53-107">Prerequisites</span></span>
<span data-ttu-id="b7d53-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7d53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7d53-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7d53-110">Permission type</span></span>|<span data-ttu-id="b7d53-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7d53-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7d53-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7d53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7d53-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7d53-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b7d53-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7d53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7d53-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7d53-115">Not supported.</span></span>|
|<span data-ttu-id="b7d53-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7d53-116">Application</span></span>|<span data-ttu-id="b7d53-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7d53-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7d53-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7d53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="b7d53-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7d53-119">Request headers</span></span>
|<span data-ttu-id="b7d53-120">标头</span><span class="sxs-lookup"><span data-stu-id="b7d53-120">Header</span></span>|<span data-ttu-id="b7d53-121">值</span><span class="sxs-lookup"><span data-stu-id="b7d53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7d53-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7d53-122">Authorization</span></span>|<span data-ttu-id="b7d53-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b7d53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7d53-124">接受</span><span class="sxs-lookup"><span data-stu-id="b7d53-124">Accept</span></span>|<span data-ttu-id="b7d53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7d53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7d53-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7d53-126">Request body</span></span>
<span data-ttu-id="b7d53-127">在请求正文中，提供 [deviceManagement](../resources/intune-devices-devicemanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7d53-127">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-devices-devicemanagement.md) object.</span></span>

<span data-ttu-id="b7d53-128">下表显示创建 [deviceManagement](../resources/intune-devices-devicemanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b7d53-128">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-devices-devicemanagement.md).</span></span>

|<span data-ttu-id="b7d53-129">属性</span><span class="sxs-lookup"><span data-stu-id="b7d53-129">Property</span></span>|<span data-ttu-id="b7d53-130">类型</span><span class="sxs-lookup"><span data-stu-id="b7d53-130">Type</span></span>|<span data-ttu-id="b7d53-131">说明</span><span class="sxs-lookup"><span data-stu-id="b7d53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7d53-132">id</span><span class="sxs-lookup"><span data-stu-id="b7d53-132">id</span></span>|<span data-ttu-id="b7d53-133">String</span><span class="sxs-lookup"><span data-stu-id="b7d53-133">String</span></span>|<span data-ttu-id="b7d53-134">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="b7d53-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="b7d53-135">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="b7d53-135">subscriptionState</span></span>|[<span data-ttu-id="b7d53-136">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="b7d53-136">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="b7d53-137">租户移动设备管理订阅状态。</span><span class="sxs-lookup"><span data-stu-id="b7d53-137">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="b7d53-138">可取值为：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="b7d53-138">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="b7d53-139">响应</span><span class="sxs-lookup"><span data-stu-id="b7d53-139">Response</span></span>
<span data-ttu-id="b7d53-140">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagement](../resources/intune-devices-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b7d53-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-devices-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7d53-141">示例</span><span class="sxs-lookup"><span data-stu-id="b7d53-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7d53-142">请求</span><span class="sxs-lookup"><span data-stu-id="b7d53-142">Request</span></span>
<span data-ttu-id="b7d53-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b7d53-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "subscriptionState": "active"
}
```

### <a name="response"></a><span data-ttu-id="b7d53-144">响应</span><span class="sxs-lookup"><span data-stu-id="b7d53-144">Response</span></span>
<span data-ttu-id="b7d53-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b7d53-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 141

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "subscriptionState": "active"
}
```




