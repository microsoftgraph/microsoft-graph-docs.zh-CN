---
title: 创建 managedMobileApp
description: 创建新的 managedMobileApp 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6363932442346dbbcfb7350a7ba020de384df53
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42803468"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="8ba72-103">创建 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="8ba72-103">Create managedMobileApp</span></span>

> <span data-ttu-id="8ba72-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8ba72-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ba72-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ba72-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ba72-106">创建新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ba72-106">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ba72-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8ba72-107">Prerequisites</span></span>
<span data-ttu-id="8ba72-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ba72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ba72-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ba72-110">Permission type</span></span>|<span data-ttu-id="8ba72-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8ba72-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ba72-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ba72-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8ba72-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ba72-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8ba72-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ba72-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ba72-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ba72-115">Not supported.</span></span>|
|<span data-ttu-id="8ba72-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ba72-116">Application</span></span>|<span data-ttu-id="8ba72-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ba72-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ba72-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ba72-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
POST /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
POST /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="8ba72-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ba72-119">Request headers</span></span>
|<span data-ttu-id="8ba72-120">标头</span><span class="sxs-lookup"><span data-stu-id="8ba72-120">Header</span></span>|<span data-ttu-id="8ba72-121">值</span><span class="sxs-lookup"><span data-stu-id="8ba72-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ba72-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ba72-122">Authorization</span></span>|<span data-ttu-id="8ba72-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8ba72-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ba72-124">接受</span><span class="sxs-lookup"><span data-stu-id="8ba72-124">Accept</span></span>|<span data-ttu-id="8ba72-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8ba72-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ba72-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ba72-126">Request body</span></span>
<span data-ttu-id="8ba72-127">在请求正文中，提供 managedMobileApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ba72-127">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="8ba72-128">下表显示创建 managedMobileApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8ba72-128">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="8ba72-129">属性</span><span class="sxs-lookup"><span data-stu-id="8ba72-129">Property</span></span>|<span data-ttu-id="8ba72-130">类型</span><span class="sxs-lookup"><span data-stu-id="8ba72-130">Type</span></span>|<span data-ttu-id="8ba72-131">说明</span><span class="sxs-lookup"><span data-stu-id="8ba72-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ba72-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8ba72-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="8ba72-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8ba72-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="8ba72-134">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="8ba72-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="8ba72-135">id</span><span class="sxs-lookup"><span data-stu-id="8ba72-135">id</span></span>|<span data-ttu-id="8ba72-136">String</span><span class="sxs-lookup"><span data-stu-id="8ba72-136">String</span></span>|<span data-ttu-id="8ba72-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8ba72-137">Key of the entity.</span></span>|
|<span data-ttu-id="8ba72-138">version</span><span class="sxs-lookup"><span data-stu-id="8ba72-138">version</span></span>|<span data-ttu-id="8ba72-139">String</span><span class="sxs-lookup"><span data-stu-id="8ba72-139">String</span></span>|<span data-ttu-id="8ba72-140">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="8ba72-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="8ba72-141">响应</span><span class="sxs-lookup"><span data-stu-id="8ba72-141">Response</span></span>
<span data-ttu-id="8ba72-142">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ba72-142">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ba72-143">示例</span><span class="sxs-lookup"><span data-stu-id="8ba72-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ba72-144">请求</span><span class="sxs-lookup"><span data-stu-id="8ba72-144">Request</span></span>
<span data-ttu-id="8ba72-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ba72-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
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

### <a name="response"></a><span data-ttu-id="8ba72-146">响应</span><span class="sxs-lookup"><span data-stu-id="8ba72-146">Response</span></span>
<span data-ttu-id="8ba72-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ba72-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




