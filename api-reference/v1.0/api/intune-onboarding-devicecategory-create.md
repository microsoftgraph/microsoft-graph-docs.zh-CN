---
title: 创建 deviceCategory
description: 创建新的 deviceCategory 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9b1bfb046b4a1949ddba846d5a30c34256198049
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759484"
---
# <a name="create-devicecategory"></a><span data-ttu-id="12396-103">创建 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="12396-103">Create deviceCategory</span></span>

<span data-ttu-id="12396-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12396-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12396-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12396-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12396-106">创建新的 [deviceCategory](../resources/intune-onboarding-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12396-106">Create a new [deviceCategory](../resources/intune-onboarding-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12396-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="12396-107">Prerequisites</span></span>
<span data-ttu-id="12396-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12396-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12396-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="12396-110">Permission type</span></span>|<span data-ttu-id="12396-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12396-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12396-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12396-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12396-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12396-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="12396-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12396-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12396-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="12396-115">Not supported.</span></span>|
|<span data-ttu-id="12396-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="12396-116">Application</span></span>|<span data-ttu-id="12396-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12396-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12396-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12396-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="12396-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="12396-119">Request headers</span></span>
|<span data-ttu-id="12396-120">标头</span><span class="sxs-lookup"><span data-stu-id="12396-120">Header</span></span>|<span data-ttu-id="12396-121">值</span><span class="sxs-lookup"><span data-stu-id="12396-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12396-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12396-122">Authorization</span></span>|<span data-ttu-id="12396-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12396-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12396-124">接受</span><span class="sxs-lookup"><span data-stu-id="12396-124">Accept</span></span>|<span data-ttu-id="12396-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12396-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12396-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="12396-126">Request body</span></span>
<span data-ttu-id="12396-127">在请求正文中，提供 deviceCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12396-127">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="12396-128">下表显示创建 deviceCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="12396-128">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="12396-129">属性</span><span class="sxs-lookup"><span data-stu-id="12396-129">Property</span></span>|<span data-ttu-id="12396-130">类型</span><span class="sxs-lookup"><span data-stu-id="12396-130">Type</span></span>|<span data-ttu-id="12396-131">说明</span><span class="sxs-lookup"><span data-stu-id="12396-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12396-132">id</span><span class="sxs-lookup"><span data-stu-id="12396-132">id</span></span>|<span data-ttu-id="12396-133">String</span><span class="sxs-lookup"><span data-stu-id="12396-133">String</span></span>|<span data-ttu-id="12396-134">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="12396-134">Unique identifier for the device category.</span></span> <span data-ttu-id="12396-135">只读。</span><span class="sxs-lookup"><span data-stu-id="12396-135">Read-only.</span></span>|
|<span data-ttu-id="12396-136">displayName</span><span class="sxs-lookup"><span data-stu-id="12396-136">displayName</span></span>|<span data-ttu-id="12396-137">String</span><span class="sxs-lookup"><span data-stu-id="12396-137">String</span></span>|<span data-ttu-id="12396-138">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="12396-138">Display name for the device category.</span></span>|
|<span data-ttu-id="12396-139">description</span><span class="sxs-lookup"><span data-stu-id="12396-139">description</span></span>|<span data-ttu-id="12396-140">String</span><span class="sxs-lookup"><span data-stu-id="12396-140">String</span></span>|<span data-ttu-id="12396-141">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="12396-141">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="12396-142">响应</span><span class="sxs-lookup"><span data-stu-id="12396-142">Response</span></span>
<span data-ttu-id="12396-143">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceCategory](../resources/intune-onboarding-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12396-143">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-onboarding-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12396-144">示例</span><span class="sxs-lookup"><span data-stu-id="12396-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="12396-145">请求</span><span class="sxs-lookup"><span data-stu-id="12396-145">Request</span></span>
<span data-ttu-id="12396-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12396-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="12396-147">响应</span><span class="sxs-lookup"><span data-stu-id="12396-147">Response</span></span>
<span data-ttu-id="12396-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12396-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```




