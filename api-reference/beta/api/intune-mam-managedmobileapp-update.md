---
title: 更新 managedMobileApp
description: 更新 managedMobileApp 对象的属性。
ms.openlocfilehash: c15e46562b43aa87f9dafe85be2b8dde93ff21f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042022"
---
# <a name="update-managedmobileapp"></a><span data-ttu-id="f8634-103">更新 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="f8634-103">Update managedMobileApp</span></span>

> <span data-ttu-id="f8634-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f8634-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8634-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f8634-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8634-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f8634-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8634-107">更新 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f8634-107">Update the properties of a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8634-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f8634-108">Prerequisites</span></span>
<span data-ttu-id="f8634-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f8634-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8634-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8634-111">Permission type</span></span>|<span data-ttu-id="f8634-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f8634-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8634-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8634-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8634-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8634-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f8634-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8634-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8634-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8634-116">Not supported.</span></span>|
|<span data-ttu-id="f8634-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8634-117">Application</span></span>|<span data-ttu-id="f8634-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8634-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8634-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8634-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f8634-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8634-120">Request headers</span></span>
|<span data-ttu-id="f8634-121">标头</span><span class="sxs-lookup"><span data-stu-id="f8634-121">Header</span></span>|<span data-ttu-id="f8634-122">值</span><span class="sxs-lookup"><span data-stu-id="f8634-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8634-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8634-123">Authorization</span></span>|<span data-ttu-id="f8634-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f8634-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8634-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8634-125">Accept</span></span>|<span data-ttu-id="f8634-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8634-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8634-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8634-127">Request body</span></span>
<span data-ttu-id="f8634-128">在请求正文中，提供 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8634-128">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

<span data-ttu-id="f8634-129">下表显示创建 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f8634-129">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune-mam-managedmobileapp.md).</span></span>

|<span data-ttu-id="f8634-130">属性</span><span class="sxs-lookup"><span data-stu-id="f8634-130">Property</span></span>|<span data-ttu-id="f8634-131">类型</span><span class="sxs-lookup"><span data-stu-id="f8634-131">Type</span></span>|<span data-ttu-id="f8634-132">说明</span><span class="sxs-lookup"><span data-stu-id="f8634-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8634-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f8634-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="f8634-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f8634-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="f8634-135">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="f8634-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="f8634-136">id</span><span class="sxs-lookup"><span data-stu-id="f8634-136">id</span></span>|<span data-ttu-id="f8634-137">String</span><span class="sxs-lookup"><span data-stu-id="f8634-137">String</span></span>|<span data-ttu-id="f8634-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f8634-138">Key of the entity.</span></span>|
|<span data-ttu-id="f8634-139">version</span><span class="sxs-lookup"><span data-stu-id="f8634-139">version</span></span>|<span data-ttu-id="f8634-140">String</span><span class="sxs-lookup"><span data-stu-id="f8634-140">String</span></span>|<span data-ttu-id="f8634-141">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="f8634-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="f8634-142">响应</span><span class="sxs-lookup"><span data-stu-id="f8634-142">Response</span></span>
<span data-ttu-id="f8634-143">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f8634-143">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8634-144">示例</span><span class="sxs-lookup"><span data-stu-id="f8634-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8634-145">请求</span><span class="sxs-lookup"><span data-stu-id="f8634-145">Request</span></span>
<span data-ttu-id="f8634-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8634-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 126

{
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="f8634-147">响应</span><span class="sxs-lookup"><span data-stu-id="f8634-147">Response</span></span>
<span data-ttu-id="f8634-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8634-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





