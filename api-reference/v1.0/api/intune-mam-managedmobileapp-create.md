---
title: 创建 managedMobileApp
description: 创建新的 managedMobileApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08ef8698f98876d9a8115b604d3127c1385eade8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758071"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="d6bf2-103">创建 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="d6bf2-103">Create managedMobileApp</span></span>

<span data-ttu-id="d6bf2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6bf2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6bf2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6bf2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6bf2-106">创建新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6bf2-106">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6bf2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d6bf2-107">Prerequisites</span></span>
<span data-ttu-id="d6bf2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6bf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6bf2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6bf2-110">Permission type</span></span>|<span data-ttu-id="d6bf2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6bf2-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6bf2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6bf2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6bf2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6bf2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d6bf2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6bf2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6bf2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6bf2-115">Not supported.</span></span>|
|<span data-ttu-id="d6bf2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6bf2-116">Application</span></span>|<span data-ttu-id="d6bf2-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6bf2-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6bf2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6bf2-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d6bf2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6bf2-119">Request headers</span></span>
|<span data-ttu-id="d6bf2-120">标头</span><span class="sxs-lookup"><span data-stu-id="d6bf2-120">Header</span></span>|<span data-ttu-id="d6bf2-121">值</span><span class="sxs-lookup"><span data-stu-id="d6bf2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6bf2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6bf2-122">Authorization</span></span>|<span data-ttu-id="d6bf2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d6bf2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6bf2-124">接受</span><span class="sxs-lookup"><span data-stu-id="d6bf2-124">Accept</span></span>|<span data-ttu-id="d6bf2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6bf2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6bf2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6bf2-126">Request body</span></span>
<span data-ttu-id="d6bf2-127">在请求正文中，提供 managedMobileApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6bf2-127">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="d6bf2-128">下表显示创建 managedMobileApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d6bf2-128">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="d6bf2-129">属性</span><span class="sxs-lookup"><span data-stu-id="d6bf2-129">Property</span></span>|<span data-ttu-id="d6bf2-130">类型</span><span class="sxs-lookup"><span data-stu-id="d6bf2-130">Type</span></span>|<span data-ttu-id="d6bf2-131">说明</span><span class="sxs-lookup"><span data-stu-id="d6bf2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6bf2-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d6bf2-132">mobileAppIdentifier</span></span>|[<span data-ttu-id="d6bf2-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d6bf2-133">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d6bf2-134">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="d6bf2-134">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="d6bf2-135">id</span><span class="sxs-lookup"><span data-stu-id="d6bf2-135">id</span></span>|<span data-ttu-id="d6bf2-136">String</span><span class="sxs-lookup"><span data-stu-id="d6bf2-136">String</span></span>|<span data-ttu-id="d6bf2-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d6bf2-137">Key of the entity.</span></span>|
|<span data-ttu-id="d6bf2-138">version</span><span class="sxs-lookup"><span data-stu-id="d6bf2-138">version</span></span>|<span data-ttu-id="d6bf2-139">String</span><span class="sxs-lookup"><span data-stu-id="d6bf2-139">String</span></span>|<span data-ttu-id="d6bf2-140">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="d6bf2-140">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="d6bf2-141">响应</span><span class="sxs-lookup"><span data-stu-id="d6bf2-141">Response</span></span>
<span data-ttu-id="d6bf2-142">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6bf2-142">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6bf2-143">示例</span><span class="sxs-lookup"><span data-stu-id="d6bf2-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6bf2-144">请求</span><span class="sxs-lookup"><span data-stu-id="d6bf2-144">Request</span></span>
<span data-ttu-id="d6bf2-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6bf2-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
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

### <a name="response"></a><span data-ttu-id="d6bf2-146">响应</span><span class="sxs-lookup"><span data-stu-id="d6bf2-146">Response</span></span>
<span data-ttu-id="d6bf2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d6bf2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




