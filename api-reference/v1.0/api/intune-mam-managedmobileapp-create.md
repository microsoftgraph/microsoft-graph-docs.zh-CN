---
title: 创建 managedMobileApp
description: 创建新的 managedMobileApp 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ca5c8931a89982ec6cafe611bc6e9311187e8426
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37363463"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="31d10-103">创建 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="31d10-103">Create managedMobileApp</span></span>

> <span data-ttu-id="31d10-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="31d10-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31d10-105">创建新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31d10-105">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31d10-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="31d10-106">Prerequisites</span></span>
<span data-ttu-id="31d10-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31d10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31d10-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="31d10-109">Permission type</span></span>|<span data-ttu-id="31d10-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="31d10-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31d10-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31d10-111">Delegated (work or school account)</span></span>|<span data-ttu-id="31d10-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31d10-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="31d10-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31d10-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31d10-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="31d10-114">Not supported.</span></span>|
|<span data-ttu-id="31d10-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="31d10-115">Application</span></span>|<span data-ttu-id="31d10-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="31d10-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31d10-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31d10-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="31d10-118">请求头</span><span class="sxs-lookup"><span data-stu-id="31d10-118">Request headers</span></span>
|<span data-ttu-id="31d10-119">标头</span><span class="sxs-lookup"><span data-stu-id="31d10-119">Header</span></span>|<span data-ttu-id="31d10-120">值</span><span class="sxs-lookup"><span data-stu-id="31d10-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31d10-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="31d10-121">Authorization</span></span>|<span data-ttu-id="31d10-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="31d10-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31d10-123">接受</span><span class="sxs-lookup"><span data-stu-id="31d10-123">Accept</span></span>|<span data-ttu-id="31d10-124">application/json</span><span class="sxs-lookup"><span data-stu-id="31d10-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31d10-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="31d10-125">Request body</span></span>
<span data-ttu-id="31d10-126">在请求正文中，提供 managedMobileApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31d10-126">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="31d10-127">下表显示创建 managedMobileApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="31d10-127">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="31d10-128">属性</span><span class="sxs-lookup"><span data-stu-id="31d10-128">Property</span></span>|<span data-ttu-id="31d10-129">类型</span><span class="sxs-lookup"><span data-stu-id="31d10-129">Type</span></span>|<span data-ttu-id="31d10-130">说明</span><span class="sxs-lookup"><span data-stu-id="31d10-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31d10-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="31d10-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="31d10-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="31d10-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="31d10-133">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="31d10-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="31d10-134">id</span><span class="sxs-lookup"><span data-stu-id="31d10-134">id</span></span>|<span data-ttu-id="31d10-135">String</span><span class="sxs-lookup"><span data-stu-id="31d10-135">String</span></span>|<span data-ttu-id="31d10-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="31d10-136">Key of the entity.</span></span>|
|<span data-ttu-id="31d10-137">version</span><span class="sxs-lookup"><span data-stu-id="31d10-137">version</span></span>|<span data-ttu-id="31d10-138">String</span><span class="sxs-lookup"><span data-stu-id="31d10-138">String</span></span>|<span data-ttu-id="31d10-139">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="31d10-139">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="31d10-140">响应</span><span class="sxs-lookup"><span data-stu-id="31d10-140">Response</span></span>
<span data-ttu-id="31d10-141">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31d10-141">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31d10-142">示例</span><span class="sxs-lookup"><span data-stu-id="31d10-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="31d10-143">请求</span><span class="sxs-lookup"><span data-stu-id="31d10-143">Request</span></span>
<span data-ttu-id="31d10-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="31d10-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
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

### <a name="response"></a><span data-ttu-id="31d10-145">响应</span><span class="sxs-lookup"><span data-stu-id="31d10-145">Response</span></span>
<span data-ttu-id="31d10-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="31d10-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




