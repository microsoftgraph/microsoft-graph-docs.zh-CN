---
title: 更新 managedMobileApp
description: 更新 managedMobileApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 30c93628a161cc3523d04561b93b625711ea4bd6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149070"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="9c3ea-103">更新 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="9c3ea-103">Update managedMobileApp</span></span>

<span data-ttu-id="9c3ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c3ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c3ea-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c3ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c3ea-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c3ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c3ea-107">更新 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9c3ea-107">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c3ea-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9c3ea-108">Prerequisites</span></span>
<span data-ttu-id="9c3ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c3ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c3ea-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c3ea-111">Permission type</span></span>|<span data-ttu-id="9c3ea-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c3ea-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c3ea-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c3ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c3ea-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c3ea-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9c3ea-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c3ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c3ea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c3ea-116">Not supported.</span></span>|
|<span data-ttu-id="9c3ea-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c3ea-117">Application</span></span>|<span data-ttu-id="9c3ea-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c3ea-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c3ea-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c3ea-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9c3ea-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c3ea-120">Request headers</span></span>
|<span data-ttu-id="9c3ea-121">标头</span><span class="sxs-lookup"><span data-stu-id="9c3ea-121">Header</span></span>|<span data-ttu-id="9c3ea-122">值</span><span class="sxs-lookup"><span data-stu-id="9c3ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c3ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c3ea-123">Authorization</span></span>|<span data-ttu-id="9c3ea-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9c3ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c3ea-125">接受</span><span class="sxs-lookup"><span data-stu-id="9c3ea-125">Accept</span></span>|<span data-ttu-id="9c3ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c3ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c3ea-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c3ea-127">Request body</span></span>
<span data-ttu-id="9c3ea-128">在请求正文中，提供 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c3ea-128">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="9c3ea-129">下表显示创建 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9c3ea-129">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="9c3ea-130">属性</span><span class="sxs-lookup"><span data-stu-id="9c3ea-130">Property</span></span>|<span data-ttu-id="9c3ea-131">类型</span><span class="sxs-lookup"><span data-stu-id="9c3ea-131">Type</span></span>|<span data-ttu-id="9c3ea-132">说明</span><span class="sxs-lookup"><span data-stu-id="9c3ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c3ea-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9c3ea-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="9c3ea-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9c3ea-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="9c3ea-135">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="9c3ea-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="9c3ea-136">id</span><span class="sxs-lookup"><span data-stu-id="9c3ea-136">id</span></span>|<span data-ttu-id="9c3ea-137">String</span><span class="sxs-lookup"><span data-stu-id="9c3ea-137">String</span></span>|<span data-ttu-id="9c3ea-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9c3ea-138">Key of the entity.</span></span>|
|<span data-ttu-id="9c3ea-139">version</span><span class="sxs-lookup"><span data-stu-id="9c3ea-139">version</span></span>|<span data-ttu-id="9c3ea-140">String</span><span class="sxs-lookup"><span data-stu-id="9c3ea-140">String</span></span>|<span data-ttu-id="9c3ea-141">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="9c3ea-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="9c3ea-142">响应</span><span class="sxs-lookup"><span data-stu-id="9c3ea-142">Response</span></span>
<span data-ttu-id="9c3ea-143">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9c3ea-143">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c3ea-144">示例</span><span class="sxs-lookup"><span data-stu-id="9c3ea-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c3ea-145">请求</span><span class="sxs-lookup"><span data-stu-id="9c3ea-145">Request</span></span>
<span data-ttu-id="9c3ea-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c3ea-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 227

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.windowsAppIdentifier",
    "windowsAppId": "Windows App Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="9c3ea-147">响应</span><span class="sxs-lookup"><span data-stu-id="9c3ea-147">Response</span></span>
<span data-ttu-id="9c3ea-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c3ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 276

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.windowsAppIdentifier",
    "windowsAppId": "Windows App Id value"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```




