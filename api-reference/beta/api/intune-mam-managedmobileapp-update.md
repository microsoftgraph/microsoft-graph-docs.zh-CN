---
title: 更新 managedMobileApp
description: 更新 managedMobileApp 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 758696dd92361d1d362b520de2963f898405826d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392505"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="a905c-103">更新 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="a905c-103">Update managedMobileApp</span></span>

> <span data-ttu-id="a905c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a905c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a905c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a905c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a905c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a905c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a905c-107">更新 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a905c-107">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a905c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a905c-108">Prerequisites</span></span>
<span data-ttu-id="a905c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a905c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a905c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a905c-111">Permission type</span></span>|<span data-ttu-id="a905c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a905c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a905c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a905c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a905c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a905c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a905c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a905c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a905c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a905c-116">Not supported.</span></span>|
|<span data-ttu-id="a905c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a905c-117">Application</span></span>|<span data-ttu-id="a905c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a905c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a905c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a905c-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a905c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a905c-120">Request headers</span></span>
|<span data-ttu-id="a905c-121">标头</span><span class="sxs-lookup"><span data-stu-id="a905c-121">Header</span></span>|<span data-ttu-id="a905c-122">值</span><span class="sxs-lookup"><span data-stu-id="a905c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a905c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a905c-123">Authorization</span></span>|<span data-ttu-id="a905c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a905c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a905c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a905c-125">Accept</span></span>|<span data-ttu-id="a905c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a905c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a905c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a905c-127">Request body</span></span>
<span data-ttu-id="a905c-128">在请求正文中，提供 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a905c-128">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="a905c-129">下表显示创建 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a905c-129">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="a905c-130">属性</span><span class="sxs-lookup"><span data-stu-id="a905c-130">Property</span></span>|<span data-ttu-id="a905c-131">类型</span><span class="sxs-lookup"><span data-stu-id="a905c-131">Type</span></span>|<span data-ttu-id="a905c-132">说明</span><span class="sxs-lookup"><span data-stu-id="a905c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a905c-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a905c-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="a905c-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="a905c-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="a905c-135">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="a905c-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="a905c-136">id</span><span class="sxs-lookup"><span data-stu-id="a905c-136">id</span></span>|<span data-ttu-id="a905c-137">String</span><span class="sxs-lookup"><span data-stu-id="a905c-137">String</span></span>|<span data-ttu-id="a905c-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a905c-138">Key of the entity.</span></span>|
|<span data-ttu-id="a905c-139">version</span><span class="sxs-lookup"><span data-stu-id="a905c-139">version</span></span>|<span data-ttu-id="a905c-140">String</span><span class="sxs-lookup"><span data-stu-id="a905c-140">String</span></span>|<span data-ttu-id="a905c-141">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="a905c-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="a905c-142">响应</span><span class="sxs-lookup"><span data-stu-id="a905c-142">Response</span></span>
<span data-ttu-id="a905c-143">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a905c-143">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a905c-144">示例</span><span class="sxs-lookup"><span data-stu-id="a905c-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="a905c-145">请求</span><span class="sxs-lookup"><span data-stu-id="a905c-145">Request</span></span>
<span data-ttu-id="a905c-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a905c-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
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

### <a name="response"></a><span data-ttu-id="a905c-147">响应</span><span class="sxs-lookup"><span data-stu-id="a905c-147">Response</span></span>
<span data-ttu-id="a905c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a905c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




