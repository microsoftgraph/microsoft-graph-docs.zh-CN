---
title: 更新 managedMobileApp
description: 更新 managedMobileApp 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2f3fd398dd9721096d6a52e914e516dfae1e16b8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513026"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="8242d-103">更新 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="8242d-103">Update managedMobileApp</span></span>

<span data-ttu-id="8242d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8242d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8242d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8242d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8242d-106">更新 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8242d-106">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8242d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8242d-107">Prerequisites</span></span>
<span data-ttu-id="8242d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8242d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8242d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8242d-110">Permission type</span></span>|<span data-ttu-id="8242d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8242d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8242d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8242d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8242d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8242d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8242d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8242d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8242d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8242d-115">Not supported.</span></span>|
|<span data-ttu-id="8242d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8242d-116">Application</span></span>|<span data-ttu-id="8242d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8242d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8242d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8242d-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="8242d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8242d-119">Request headers</span></span>
|<span data-ttu-id="8242d-120">标头</span><span class="sxs-lookup"><span data-stu-id="8242d-120">Header</span></span>|<span data-ttu-id="8242d-121">值</span><span class="sxs-lookup"><span data-stu-id="8242d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8242d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8242d-122">Authorization</span></span>|<span data-ttu-id="8242d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8242d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8242d-124">接受</span><span class="sxs-lookup"><span data-stu-id="8242d-124">Accept</span></span>|<span data-ttu-id="8242d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8242d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8242d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8242d-126">Request body</span></span>
<span data-ttu-id="8242d-127">在请求正文中，提供 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8242d-127">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="8242d-128">下表显示创建 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8242d-128">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="8242d-129">属性</span><span class="sxs-lookup"><span data-stu-id="8242d-129">Property</span></span>|<span data-ttu-id="8242d-130">类型</span><span class="sxs-lookup"><span data-stu-id="8242d-130">Type</span></span>|<span data-ttu-id="8242d-131">说明</span><span class="sxs-lookup"><span data-stu-id="8242d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8242d-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8242d-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="8242d-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8242d-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="8242d-134">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="8242d-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="8242d-135">id</span><span class="sxs-lookup"><span data-stu-id="8242d-135">id</span></span>|<span data-ttu-id="8242d-136">字符串</span><span class="sxs-lookup"><span data-stu-id="8242d-136">String</span></span>|<span data-ttu-id="8242d-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8242d-137">Key of the entity.</span></span>|
|<span data-ttu-id="8242d-138">version</span><span class="sxs-lookup"><span data-stu-id="8242d-138">version</span></span>|<span data-ttu-id="8242d-139">String</span><span class="sxs-lookup"><span data-stu-id="8242d-139">String</span></span>|<span data-ttu-id="8242d-140">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="8242d-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="8242d-141">响应</span><span class="sxs-lookup"><span data-stu-id="8242d-141">Response</span></span>
<span data-ttu-id="8242d-142">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8242d-142">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8242d-143">示例</span><span class="sxs-lookup"><span data-stu-id="8242d-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="8242d-144">请求</span><span class="sxs-lookup"><span data-stu-id="8242d-144">Request</span></span>
<span data-ttu-id="8242d-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8242d-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="8242d-146">响应</span><span class="sxs-lookup"><span data-stu-id="8242d-146">Response</span></span>
<span data-ttu-id="8242d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8242d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 230

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```




