---
title: 创建 managedMobileApp
description: 创建新的 managedMobileApp 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1594c06e87aa89f8b599c27426769a28740a0300
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463291"
---
# <a name="create-managedmobileapp"></a><span data-ttu-id="fadd3-103">创建 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="fadd3-103">Create managedMobileApp</span></span>

<span data-ttu-id="fadd3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="fadd3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fadd3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fadd3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fadd3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fadd3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fadd3-107">创建新的 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fadd3-107">Create a new [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fadd3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fadd3-108">Prerequisites</span></span>
<span data-ttu-id="fadd3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fadd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fadd3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fadd3-111">Permission type</span></span>|<span data-ttu-id="fadd3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fadd3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fadd3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fadd3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fadd3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fadd3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fadd3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fadd3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fadd3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fadd3-116">Not supported.</span></span>|
|<span data-ttu-id="fadd3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fadd3-117">Application</span></span>|<span data-ttu-id="fadd3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fadd3-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fadd3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fadd3-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="fadd3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fadd3-120">Request headers</span></span>
|<span data-ttu-id="fadd3-121">标头</span><span class="sxs-lookup"><span data-stu-id="fadd3-121">Header</span></span>|<span data-ttu-id="fadd3-122">值</span><span class="sxs-lookup"><span data-stu-id="fadd3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fadd3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fadd3-123">Authorization</span></span>|<span data-ttu-id="fadd3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fadd3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fadd3-125">接受</span><span class="sxs-lookup"><span data-stu-id="fadd3-125">Accept</span></span>|<span data-ttu-id="fadd3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fadd3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fadd3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fadd3-127">Request body</span></span>
<span data-ttu-id="fadd3-128">在请求正文中，提供 managedMobileApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fadd3-128">In the request body, supply a JSON representation for the managedMobileApp object.</span></span>

<span data-ttu-id="fadd3-129">下表显示创建 managedMobileApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fadd3-129">The following table shows the properties that are required when you create the managedMobileApp.</span></span>

|<span data-ttu-id="fadd3-130">属性</span><span class="sxs-lookup"><span data-stu-id="fadd3-130">Property</span></span>|<span data-ttu-id="fadd3-131">类型</span><span class="sxs-lookup"><span data-stu-id="fadd3-131">Type</span></span>|<span data-ttu-id="fadd3-132">说明</span><span class="sxs-lookup"><span data-stu-id="fadd3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fadd3-133">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fadd3-133">mobileAppIdentifier</span></span>|[<span data-ttu-id="fadd3-134">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fadd3-134">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="fadd3-135">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="fadd3-135">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="fadd3-136">id</span><span class="sxs-lookup"><span data-stu-id="fadd3-136">id</span></span>|<span data-ttu-id="fadd3-137">String</span><span class="sxs-lookup"><span data-stu-id="fadd3-137">String</span></span>|<span data-ttu-id="fadd3-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fadd3-138">Key of the entity.</span></span>|
|<span data-ttu-id="fadd3-139">version</span><span class="sxs-lookup"><span data-stu-id="fadd3-139">version</span></span>|<span data-ttu-id="fadd3-140">String</span><span class="sxs-lookup"><span data-stu-id="fadd3-140">String</span></span>|<span data-ttu-id="fadd3-141">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="fadd3-141">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="fadd3-142">响应</span><span class="sxs-lookup"><span data-stu-id="fadd3-142">Response</span></span>
<span data-ttu-id="fadd3-143">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedMobileApp](../resources/intune-mam-managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fadd3-143">If successful, this method returns a `201 Created` response code and a [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fadd3-144">示例</span><span class="sxs-lookup"><span data-stu-id="fadd3-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="fadd3-145">请求</span><span class="sxs-lookup"><span data-stu-id="fadd3-145">Request</span></span>
<span data-ttu-id="fadd3-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fadd3-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fadd3-147">响应</span><span class="sxs-lookup"><span data-stu-id="fadd3-147">Response</span></span>
<span data-ttu-id="fadd3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fadd3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





