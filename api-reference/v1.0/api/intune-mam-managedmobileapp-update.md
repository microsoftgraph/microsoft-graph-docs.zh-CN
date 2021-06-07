---
title: 更新 managedMobileApp
description: 更新 managedMobileApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83d4478692c0e4de4205a4b33eb05306bad76563
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751522"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="b5c46-103">更新 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="b5c46-103">Update managedMobileApp</span></span>

<span data-ttu-id="b5c46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5c46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5c46-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5c46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5c46-106">更新 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b5c46-106">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5c46-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b5c46-107">Prerequisites</span></span>
<span data-ttu-id="b5c46-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5c46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5c46-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5c46-110">Permission type</span></span>|<span data-ttu-id="b5c46-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5c46-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5c46-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5c46-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b5c46-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5c46-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b5c46-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5c46-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5c46-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5c46-115">Not supported.</span></span>|
|<span data-ttu-id="b5c46-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5c46-116">Application</span></span>|<span data-ttu-id="b5c46-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5c46-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5c46-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5c46-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b5c46-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5c46-119">Request headers</span></span>
|<span data-ttu-id="b5c46-120">标头</span><span class="sxs-lookup"><span data-stu-id="b5c46-120">Header</span></span>|<span data-ttu-id="b5c46-121">值</span><span class="sxs-lookup"><span data-stu-id="b5c46-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5c46-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5c46-122">Authorization</span></span>|<span data-ttu-id="b5c46-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b5c46-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5c46-124">接受</span><span class="sxs-lookup"><span data-stu-id="b5c46-124">Accept</span></span>|<span data-ttu-id="b5c46-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5c46-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5c46-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5c46-126">Request body</span></span>
<span data-ttu-id="b5c46-127">在请求正文中，提供 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5c46-127">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="b5c46-128">下表显示创建 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b5c46-128">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="b5c46-129">属性</span><span class="sxs-lookup"><span data-stu-id="b5c46-129">Property</span></span>|<span data-ttu-id="b5c46-130">类型</span><span class="sxs-lookup"><span data-stu-id="b5c46-130">Type</span></span>|<span data-ttu-id="b5c46-131">Description</span><span class="sxs-lookup"><span data-stu-id="b5c46-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5c46-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b5c46-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="b5c46-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="b5c46-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="b5c46-134">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="b5c46-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="b5c46-135">id</span><span class="sxs-lookup"><span data-stu-id="b5c46-135">id</span></span>|<span data-ttu-id="b5c46-136">String</span><span class="sxs-lookup"><span data-stu-id="b5c46-136">String</span></span>|<span data-ttu-id="b5c46-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b5c46-137">Key of the entity.</span></span>|
|<span data-ttu-id="b5c46-138">version</span><span class="sxs-lookup"><span data-stu-id="b5c46-138">version</span></span>|<span data-ttu-id="b5c46-139">String</span><span class="sxs-lookup"><span data-stu-id="b5c46-139">String</span></span>|<span data-ttu-id="b5c46-140">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="b5c46-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b5c46-141">响应</span><span class="sxs-lookup"><span data-stu-id="b5c46-141">Response</span></span>
<span data-ttu-id="b5c46-142">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5c46-142">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5c46-143">示例</span><span class="sxs-lookup"><span data-stu-id="b5c46-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5c46-144">请求</span><span class="sxs-lookup"><span data-stu-id="b5c46-144">Request</span></span>
<span data-ttu-id="b5c46-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5c46-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 226

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="b5c46-146">响应</span><span class="sxs-lookup"><span data-stu-id="b5c46-146">Response</span></span>
<span data-ttu-id="b5c46-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5c46-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```




