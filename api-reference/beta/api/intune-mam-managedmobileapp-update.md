---
title: 更新 managedMobileApp
description: 更新 managedMobileApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 268e0984dc062ecb73a412501865e1483255739e
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178183"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="24500-103">更新 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="24500-103">Update managedMobileApp</span></span>

<span data-ttu-id="24500-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24500-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24500-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="24500-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24500-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24500-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24500-107">更新 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="24500-107">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24500-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="24500-108">Prerequisites</span></span>
<span data-ttu-id="24500-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24500-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="24500-111">Permission type</span></span>|<span data-ttu-id="24500-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="24500-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24500-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24500-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24500-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24500-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="24500-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24500-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24500-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="24500-116">Not supported.</span></span>|
|<span data-ttu-id="24500-117">Application</span><span class="sxs-lookup"><span data-stu-id="24500-117">Application</span></span>|<span data-ttu-id="24500-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24500-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24500-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24500-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="24500-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="24500-120">Request headers</span></span>
|<span data-ttu-id="24500-121">标头</span><span class="sxs-lookup"><span data-stu-id="24500-121">Header</span></span>|<span data-ttu-id="24500-122">值</span><span class="sxs-lookup"><span data-stu-id="24500-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24500-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="24500-123">Authorization</span></span>|<span data-ttu-id="24500-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="24500-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24500-125">接受</span><span class="sxs-lookup"><span data-stu-id="24500-125">Accept</span></span>|<span data-ttu-id="24500-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24500-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24500-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="24500-127">Request body</span></span>
<span data-ttu-id="24500-128">在请求正文中，提供 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24500-128">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="24500-129">下表显示创建 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="24500-129">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="24500-130">属性</span><span class="sxs-lookup"><span data-stu-id="24500-130">Property</span></span>|<span data-ttu-id="24500-131">类型</span><span class="sxs-lookup"><span data-stu-id="24500-131">Type</span></span>|<span data-ttu-id="24500-132">说明</span><span class="sxs-lookup"><span data-stu-id="24500-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24500-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="24500-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="24500-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="24500-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="24500-135">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="24500-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="24500-136">id</span><span class="sxs-lookup"><span data-stu-id="24500-136">id</span></span>|<span data-ttu-id="24500-137">字符串</span><span class="sxs-lookup"><span data-stu-id="24500-137">String</span></span>|<span data-ttu-id="24500-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="24500-138">Key of the entity.</span></span>|
|<span data-ttu-id="24500-139">version</span><span class="sxs-lookup"><span data-stu-id="24500-139">version</span></span>|<span data-ttu-id="24500-140">String</span><span class="sxs-lookup"><span data-stu-id="24500-140">String</span></span>|<span data-ttu-id="24500-141">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="24500-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="24500-142">响应</span><span class="sxs-lookup"><span data-stu-id="24500-142">Response</span></span>
<span data-ttu-id="24500-143">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="24500-143">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24500-144">示例</span><span class="sxs-lookup"><span data-stu-id="24500-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="24500-145">请求</span><span class="sxs-lookup"><span data-stu-id="24500-145">Request</span></span>
<span data-ttu-id="24500-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24500-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
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

### <a name="response"></a><span data-ttu-id="24500-147">响应</span><span class="sxs-lookup"><span data-stu-id="24500-147">Response</span></span>
<span data-ttu-id="24500-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24500-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



