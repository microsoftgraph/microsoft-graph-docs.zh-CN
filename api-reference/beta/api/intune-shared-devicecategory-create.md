---
title: 创建 deviceCategory
description: 创建新的 deviceCategory 对象。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5b7da53c95a73329b1e694e49956bfa0d66247a1
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866424"
---
# <a name="create-devicecategory"></a><span data-ttu-id="d272f-103">创建 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="d272f-103">Create deviceCategory</span></span>

<span data-ttu-id="d272f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d272f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d272f-105">**重要提示：** Microsoft Graph 中的 /beta 版本下的 API 可能会更改。</span><span class="sxs-lookup"><span data-stu-id="d272f-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d272f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d272f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d272f-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d272f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d272f-108">创建新的 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d272f-108">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d272f-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="d272f-109">Prerequisites</span></span>

<span data-ttu-id="d272f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d272f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d272f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d272f-112">Permission type</span></span>|<span data-ttu-id="d272f-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d272f-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d272f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d272f-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d272f-115">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="d272f-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d272f-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d272f-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d272f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d272f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d272f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d272f-118">Not supported.</span></span>|
|<span data-ttu-id="d272f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="d272f-119">Application</span></span>||
| <span data-ttu-id="d272f-120">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="d272f-120">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d272f-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d272f-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d272f-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d272f-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="d272f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d272f-123">Request headers</span></span>

|<span data-ttu-id="d272f-124">标头</span><span class="sxs-lookup"><span data-stu-id="d272f-124">Header</span></span>|<span data-ttu-id="d272f-125">值</span><span class="sxs-lookup"><span data-stu-id="d272f-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d272f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d272f-126">Authorization</span></span>|<span data-ttu-id="d272f-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d272f-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d272f-128">接受</span><span class="sxs-lookup"><span data-stu-id="d272f-128">Accept</span></span>|<span data-ttu-id="d272f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d272f-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d272f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d272f-130">Request body</span></span>

<span data-ttu-id="d272f-131">在请求正文中，提供 deviceCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d272f-131">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="d272f-132">下表显示创建 deviceCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d272f-132">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="d272f-133">属性</span><span class="sxs-lookup"><span data-stu-id="d272f-133">Property</span></span>|<span data-ttu-id="d272f-134">类型</span><span class="sxs-lookup"><span data-stu-id="d272f-134">Type</span></span>|<span data-ttu-id="d272f-135">说明</span><span class="sxs-lookup"><span data-stu-id="d272f-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d272f-136">id</span><span class="sxs-lookup"><span data-stu-id="d272f-136">id</span></span>|<span data-ttu-id="d272f-137">String</span><span class="sxs-lookup"><span data-stu-id="d272f-137">String</span></span>|<span data-ttu-id="d272f-138">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d272f-138">Unique identifier for the device category.</span></span> <span data-ttu-id="d272f-139">只读。</span><span class="sxs-lookup"><span data-stu-id="d272f-139">Read-only.</span></span>|
|<span data-ttu-id="d272f-140">**板载**</span><span class="sxs-lookup"><span data-stu-id="d272f-140">**Obboarding**</span></span>|
|<span data-ttu-id="d272f-141">说明</span><span class="sxs-lookup"><span data-stu-id="d272f-141">description</span></span>|<span data-ttu-id="d272f-142">String</span><span class="sxs-lookup"><span data-stu-id="d272f-142">String</span></span>|<span data-ttu-id="d272f-143">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="d272f-143">Optional description for the device category.</span></span>|
|<span data-ttu-id="d272f-144">displayName</span><span class="sxs-lookup"><span data-stu-id="d272f-144">displayName</span></span>|<span data-ttu-id="d272f-145">String</span><span class="sxs-lookup"><span data-stu-id="d272f-145">String</span></span>|<span data-ttu-id="d272f-146">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d272f-146">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="d272f-147">响应</span><span class="sxs-lookup"><span data-stu-id="d272f-147">Response</span></span>

<span data-ttu-id="d272f-148">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceCategory](../resources/intune-shared-devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d272f-148">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d272f-149">示例</span><span class="sxs-lookup"><span data-stu-id="d272f-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="d272f-150">请求</span><span class="sxs-lookup"><span data-stu-id="d272f-150">Request</span></span>

<span data-ttu-id="d272f-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d272f-151">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="d272f-152">响应</span><span class="sxs-lookup"><span data-stu-id="d272f-152">Response</span></span>

<span data-ttu-id="d272f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d272f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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










