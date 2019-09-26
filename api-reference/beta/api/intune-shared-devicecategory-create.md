---
title: 创建 deviceCategory
description: 创建新的 deviceCategory 对象。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2715d1a16b1647f23d85002f52c9c789d5c47668
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194731"
---
# <a name="create-devicecategory"></a><span data-ttu-id="aeca7-103">创建 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="aeca7-103">Create deviceCategory</span></span>

> <span data-ttu-id="aeca7-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aeca7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aeca7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aeca7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aeca7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aeca7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aeca7-107">创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aeca7-107">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aeca7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="aeca7-108">Prerequisites</span></span>

<span data-ttu-id="aeca7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aeca7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aeca7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aeca7-111">Permission type</span></span>|<span data-ttu-id="aeca7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aeca7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aeca7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aeca7-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="aeca7-114">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="aeca7-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="aeca7-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aeca7-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="aeca7-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aeca7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aeca7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="aeca7-117">Not supported.</span></span>|
|<span data-ttu-id="aeca7-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="aeca7-118">Application</span></span>||
| <span data-ttu-id="aeca7-119">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="aeca7-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="aeca7-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aeca7-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aeca7-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aeca7-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="aeca7-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="aeca7-122">Request headers</span></span>

|<span data-ttu-id="aeca7-123">标头</span><span class="sxs-lookup"><span data-stu-id="aeca7-123">Header</span></span>|<span data-ttu-id="aeca7-124">值</span><span class="sxs-lookup"><span data-stu-id="aeca7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aeca7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aeca7-125">Authorization</span></span>|<span data-ttu-id="aeca7-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aeca7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aeca7-127">接受</span><span class="sxs-lookup"><span data-stu-id="aeca7-127">Accept</span></span>|<span data-ttu-id="aeca7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="aeca7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aeca7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="aeca7-129">Request body</span></span>

<span data-ttu-id="aeca7-130">在请求正文中，提供 deviceCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aeca7-130">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="aeca7-131">下表显示创建 deviceCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aeca7-131">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="aeca7-132">属性</span><span class="sxs-lookup"><span data-stu-id="aeca7-132">Property</span></span>|<span data-ttu-id="aeca7-133">类型</span><span class="sxs-lookup"><span data-stu-id="aeca7-133">Type</span></span>|<span data-ttu-id="aeca7-134">说明</span><span class="sxs-lookup"><span data-stu-id="aeca7-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aeca7-135">id</span><span class="sxs-lookup"><span data-stu-id="aeca7-135">id</span></span>|<span data-ttu-id="aeca7-136">字符串</span><span class="sxs-lookup"><span data-stu-id="aeca7-136">String</span></span>|<span data-ttu-id="aeca7-137">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aeca7-137">Unique identifier for the device category.</span></span> <span data-ttu-id="aeca7-138">只读。</span><span class="sxs-lookup"><span data-stu-id="aeca7-138">Read-only.</span></span>|
|<span data-ttu-id="aeca7-139">**Obboarding**</span><span class="sxs-lookup"><span data-stu-id="aeca7-139">**Obboarding**</span></span>|
|<span data-ttu-id="aeca7-140">说明</span><span class="sxs-lookup"><span data-stu-id="aeca7-140">description</span></span>|<span data-ttu-id="aeca7-141">String</span><span class="sxs-lookup"><span data-stu-id="aeca7-141">String</span></span>|<span data-ttu-id="aeca7-142">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="aeca7-142">Optional description for the device category.</span></span>|
|<span data-ttu-id="aeca7-143">displayName</span><span class="sxs-lookup"><span data-stu-id="aeca7-143">displayName</span></span>|<span data-ttu-id="aeca7-144">String</span><span class="sxs-lookup"><span data-stu-id="aeca7-144">String</span></span>|<span data-ttu-id="aeca7-145">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="aeca7-145">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="aeca7-146">响应</span><span class="sxs-lookup"><span data-stu-id="aeca7-146">Response</span></span>

<span data-ttu-id="aeca7-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aeca7-147">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aeca7-148">示例</span><span class="sxs-lookup"><span data-stu-id="aeca7-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="aeca7-149">请求</span><span class="sxs-lookup"><span data-stu-id="aeca7-149">Request</span></span>

<span data-ttu-id="aeca7-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aeca7-150">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="aeca7-151">响应</span><span class="sxs-lookup"><span data-stu-id="aeca7-151">Response</span></span>

<span data-ttu-id="aeca7-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aeca7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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







