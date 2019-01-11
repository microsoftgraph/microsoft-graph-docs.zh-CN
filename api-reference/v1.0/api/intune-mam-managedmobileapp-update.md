---
title: 更新 managedMobileApp
description: 更新 managedMobileApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6cc9c8df05db8bf9b7c0eb6e53f635c816e114ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807250"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="9fecd-103">更新 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="9fecd-103">Update managedMobileApp</span></span>

> <span data-ttu-id="9fecd-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9fecd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fecd-105">更新 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9fecd-105">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9fecd-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9fecd-106">Prerequisites</span></span>
<span data-ttu-id="9fecd-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="9fecd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fecd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fecd-109">Permission type</span></span>|<span data-ttu-id="9fecd-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9fecd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fecd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fecd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9fecd-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fecd-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9fecd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fecd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fecd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fecd-114">Not supported.</span></span>|
|<span data-ttu-id="9fecd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fecd-115">Application</span></span>|<span data-ttu-id="9fecd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fecd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fecd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9fecd-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9fecd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9fecd-118">Request headers</span></span>
|<span data-ttu-id="9fecd-119">标头</span><span class="sxs-lookup"><span data-stu-id="9fecd-119">Header</span></span>|<span data-ttu-id="9fecd-120">值</span><span class="sxs-lookup"><span data-stu-id="9fecd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fecd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fecd-121">Authorization</span></span>|<span data-ttu-id="9fecd-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9fecd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fecd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9fecd-123">Accept</span></span>|<span data-ttu-id="9fecd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9fecd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fecd-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9fecd-125">Request body</span></span>
<span data-ttu-id="9fecd-126">在请求正文中，提供 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fecd-126">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="9fecd-127">下表显示创建 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9fecd-127">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="9fecd-128">属性</span><span class="sxs-lookup"><span data-stu-id="9fecd-128">Property</span></span>|<span data-ttu-id="9fecd-129">类型</span><span class="sxs-lookup"><span data-stu-id="9fecd-129">Type</span></span>|<span data-ttu-id="9fecd-130">说明</span><span class="sxs-lookup"><span data-stu-id="9fecd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fecd-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9fecd-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="9fecd-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="9fecd-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="9fecd-133">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="9fecd-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="9fecd-134">id</span><span class="sxs-lookup"><span data-stu-id="9fecd-134">id</span></span>|<span data-ttu-id="9fecd-135">String</span><span class="sxs-lookup"><span data-stu-id="9fecd-135">String</span></span>|<span data-ttu-id="9fecd-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9fecd-136">Key of the entity.</span></span>|
|<span data-ttu-id="9fecd-137">version</span><span class="sxs-lookup"><span data-stu-id="9fecd-137">version</span></span>|<span data-ttu-id="9fecd-138">String</span><span class="sxs-lookup"><span data-stu-id="9fecd-138">String</span></span>|<span data-ttu-id="9fecd-139">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="9fecd-139">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="9fecd-140">响应</span><span class="sxs-lookup"><span data-stu-id="9fecd-140">Response</span></span>
<span data-ttu-id="9fecd-141">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9fecd-141">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fecd-142">示例</span><span class="sxs-lookup"><span data-stu-id="9fecd-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="9fecd-143">请求</span><span class="sxs-lookup"><span data-stu-id="9fecd-143">Request</span></span>
<span data-ttu-id="9fecd-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9fecd-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9fecd-145">响应</span><span class="sxs-lookup"><span data-stu-id="9fecd-145">Response</span></span>
<span data-ttu-id="9fecd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9fecd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



