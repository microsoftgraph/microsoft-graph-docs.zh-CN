---
title: 创建 managedMobileApp
description: 创建新的 managedMobileApp 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 546110d3e25c7b5b683f9104997fdbc497e78f9c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404699"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="19602-103">创建 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="19602-103">Create managedMobileApp</span></span>

> <span data-ttu-id="19602-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="19602-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="19602-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="19602-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19602-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19602-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19602-107">创建新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19602-107">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19602-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="19602-108">Prerequisites</span></span>
<span data-ttu-id="19602-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="19602-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="19602-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="19602-111">Permission type</span></span>|<span data-ttu-id="19602-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="19602-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19602-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19602-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19602-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19602-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="19602-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19602-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19602-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="19602-116">Not supported.</span></span>|
|<span data-ttu-id="19602-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="19602-117">Application</span></span>|<span data-ttu-id="19602-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="19602-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19602-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19602-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="19602-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="19602-120">Request headers</span></span>
|<span data-ttu-id="19602-121">标头</span><span class="sxs-lookup"><span data-stu-id="19602-121">Header</span></span>|<span data-ttu-id="19602-122">值</span><span class="sxs-lookup"><span data-stu-id="19602-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19602-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="19602-123">Authorization</span></span>|<span data-ttu-id="19602-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="19602-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19602-125">Accept</span><span class="sxs-lookup"><span data-stu-id="19602-125">Accept</span></span>|<span data-ttu-id="19602-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19602-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19602-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="19602-127">Request body</span></span>
<span data-ttu-id="19602-128">在请求正文中，提供 managedMobileApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19602-128">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="19602-129">下表显示创建 managedMobileApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="19602-129">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="19602-130">属性</span><span class="sxs-lookup"><span data-stu-id="19602-130">Property</span></span>|<span data-ttu-id="19602-131">类型</span><span class="sxs-lookup"><span data-stu-id="19602-131">Type</span></span>|<span data-ttu-id="19602-132">说明</span><span class="sxs-lookup"><span data-stu-id="19602-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19602-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="19602-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="19602-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="19602-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="19602-135">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="19602-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="19602-136">id</span><span class="sxs-lookup"><span data-stu-id="19602-136">id</span></span>|<span data-ttu-id="19602-137">String</span><span class="sxs-lookup"><span data-stu-id="19602-137">String</span></span>|<span data-ttu-id="19602-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="19602-138">Key of the entity.</span></span>|
|<span data-ttu-id="19602-139">version</span><span class="sxs-lookup"><span data-stu-id="19602-139">version</span></span>|<span data-ttu-id="19602-140">String</span><span class="sxs-lookup"><span data-stu-id="19602-140">String</span></span>|<span data-ttu-id="19602-141">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="19602-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="19602-142">响应</span><span class="sxs-lookup"><span data-stu-id="19602-142">Response</span></span>
<span data-ttu-id="19602-143">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19602-143">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19602-144">示例</span><span class="sxs-lookup"><span data-stu-id="19602-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="19602-145">请求</span><span class="sxs-lookup"><span data-stu-id="19602-145">Request</span></span>
<span data-ttu-id="19602-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="19602-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="19602-147">响应</span><span class="sxs-lookup"><span data-stu-id="19602-147">Response</span></span>
<span data-ttu-id="19602-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19602-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




