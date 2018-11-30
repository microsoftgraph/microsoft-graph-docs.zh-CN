---
title: 创建 managedMobileApp
description: 创建新的 managedMobileApp 对象。
ms.openlocfilehash: 56eabc98d51e2717406b2aa4993e21b26aecd47d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008952"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="d51e2-103">创建 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="d51e2-103">Create managedMobileApp</span></span>

> <span data-ttu-id="d51e2-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d51e2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d51e2-105">创建新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d51e2-105">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d51e2-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d51e2-106">Prerequisites</span></span>
<span data-ttu-id="d51e2-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d51e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d51e2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d51e2-109">Permission type</span></span>|<span data-ttu-id="d51e2-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d51e2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d51e2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d51e2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d51e2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d51e2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d51e2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d51e2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d51e2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d51e2-114">Not supported.</span></span>|
|<span data-ttu-id="d51e2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d51e2-115">Application</span></span>|<span data-ttu-id="d51e2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d51e2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d51e2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d51e2-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="d51e2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d51e2-118">Request headers</span></span>
|<span data-ttu-id="d51e2-119">标头</span><span class="sxs-lookup"><span data-stu-id="d51e2-119">Header</span></span>|<span data-ttu-id="d51e2-120">值</span><span class="sxs-lookup"><span data-stu-id="d51e2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d51e2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d51e2-121">Authorization</span></span>|<span data-ttu-id="d51e2-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d51e2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d51e2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d51e2-123">Accept</span></span>|<span data-ttu-id="d51e2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d51e2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d51e2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d51e2-125">Request body</span></span>
<span data-ttu-id="d51e2-126">在请求正文中，提供 managedMobileApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d51e2-126">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="d51e2-127">下表显示创建 managedMobileApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d51e2-127">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="d51e2-128">属性</span><span class="sxs-lookup"><span data-stu-id="d51e2-128">Property</span></span>|<span data-ttu-id="d51e2-129">类型</span><span class="sxs-lookup"><span data-stu-id="d51e2-129">Type</span></span>|<span data-ttu-id="d51e2-130">说明</span><span class="sxs-lookup"><span data-stu-id="d51e2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d51e2-131">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d51e2-131">mobileAppIdentifier</span></span>|[<span data-ttu-id="d51e2-132">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d51e2-132">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d51e2-133">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="d51e2-133">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="d51e2-134">id</span><span class="sxs-lookup"><span data-stu-id="d51e2-134">id</span></span>|<span data-ttu-id="d51e2-135">String</span><span class="sxs-lookup"><span data-stu-id="d51e2-135">String</span></span>|<span data-ttu-id="d51e2-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d51e2-136">Key of the entity.</span></span>|
|<span data-ttu-id="d51e2-137">version</span><span class="sxs-lookup"><span data-stu-id="d51e2-137">version</span></span>|<span data-ttu-id="d51e2-138">String</span><span class="sxs-lookup"><span data-stu-id="d51e2-138">String</span></span>|<span data-ttu-id="d51e2-139">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="d51e2-139">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="d51e2-140">响应</span><span class="sxs-lookup"><span data-stu-id="d51e2-140">Response</span></span>
<span data-ttu-id="d51e2-141">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d51e2-141">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d51e2-142">示例</span><span class="sxs-lookup"><span data-stu-id="d51e2-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="d51e2-143">请求</span><span class="sxs-lookup"><span data-stu-id="d51e2-143">Request</span></span>
<span data-ttu-id="d51e2-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d51e2-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d51e2-145">响应</span><span class="sxs-lookup"><span data-stu-id="d51e2-145">Response</span></span>
<span data-ttu-id="d51e2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d51e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



