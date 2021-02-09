---
title: 创建 userExperienceAnalyticsDeviceWithoutCloudIdentity
description: 创建新的 userExperienceAnalyticsDeviceWithoutCloudIdentity 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a3022153d740837f0c05864decfb2caba8fc9a43
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162257"
---
# <a name="create-userexperienceanalyticsdevicewithoutcloudidentity"></a><span data-ttu-id="c4b62-103">创建 userExperienceAnalyticsDeviceWithoutCloudIdentity</span><span class="sxs-lookup"><span data-stu-id="c4b62-103">Create userExperienceAnalyticsDeviceWithoutCloudIdentity</span></span>

<span data-ttu-id="c4b62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4b62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4b62-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c4b62-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4b62-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c4b62-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4b62-107">创建新的 [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c4b62-107">Create a new [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4b62-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c4b62-108">Prerequisites</span></span>
<span data-ttu-id="c4b62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4b62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4b62-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4b62-111">Permission type</span></span>|<span data-ttu-id="c4b62-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c4b62-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4b62-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4b62-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4b62-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4b62-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c4b62-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4b62-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4b62-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4b62-116">Not supported.</span></span>|
|<span data-ttu-id="c4b62-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4b62-117">Application</span></span>|<span data-ttu-id="c4b62-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4b62-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4b62-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4b62-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDevicesWithoutCloudIdentity
```

## <a name="request-headers"></a><span data-ttu-id="c4b62-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4b62-120">Request headers</span></span>
|<span data-ttu-id="c4b62-121">标头</span><span class="sxs-lookup"><span data-stu-id="c4b62-121">Header</span></span>|<span data-ttu-id="c4b62-122">值</span><span class="sxs-lookup"><span data-stu-id="c4b62-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4b62-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4b62-123">Authorization</span></span>|<span data-ttu-id="c4b62-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c4b62-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4b62-125">接受</span><span class="sxs-lookup"><span data-stu-id="c4b62-125">Accept</span></span>|<span data-ttu-id="c4b62-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4b62-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4b62-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4b62-127">Request body</span></span>
<span data-ttu-id="c4b62-128">在请求正文中，提供 userExperienceAnalyticsDeviceWithoutCloudIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4b62-128">In the request body, supply a JSON representation for the userExperienceAnalyticsDeviceWithoutCloudIdentity object.</span></span>

<span data-ttu-id="c4b62-129">下表显示创建 userExperienceAnalyticsDeviceWithoutCloudIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c4b62-129">The following table shows the properties that are required when you create the userExperienceAnalyticsDeviceWithoutCloudIdentity.</span></span>

|<span data-ttu-id="c4b62-130">属性</span><span class="sxs-lookup"><span data-stu-id="c4b62-130">Property</span></span>|<span data-ttu-id="c4b62-131">类型</span><span class="sxs-lookup"><span data-stu-id="c4b62-131">Type</span></span>|<span data-ttu-id="c4b62-132">说明</span><span class="sxs-lookup"><span data-stu-id="c4b62-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4b62-133">id</span><span class="sxs-lookup"><span data-stu-id="c4b62-133">id</span></span>|<span data-ttu-id="c4b62-134">String</span><span class="sxs-lookup"><span data-stu-id="c4b62-134">String</span></span>|<span data-ttu-id="c4b62-135">用户体验分析租户附加设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c4b62-135">The unique identifier of the user experience analytics tenant attach device.</span></span>|
|<span data-ttu-id="c4b62-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="c4b62-136">deviceName</span></span>|<span data-ttu-id="c4b62-137">String</span><span class="sxs-lookup"><span data-stu-id="c4b62-137">String</span></span>|<span data-ttu-id="c4b62-138">租户附加设备的名称。</span><span class="sxs-lookup"><span data-stu-id="c4b62-138">The tenant attach device's name.</span></span>|
|<span data-ttu-id="c4b62-139">azureAdDeviceId</span><span class="sxs-lookup"><span data-stu-id="c4b62-139">azureAdDeviceId</span></span>|<span data-ttu-id="c4b62-140">String</span><span class="sxs-lookup"><span data-stu-id="c4b62-140">String</span></span>|<span data-ttu-id="c4b62-141">Azure Active Directory 设备 ID</span><span class="sxs-lookup"><span data-stu-id="c4b62-141">Azure Active Directory Device Id</span></span>|



## <a name="response"></a><span data-ttu-id="c4b62-142">响应</span><span class="sxs-lookup"><span data-stu-id="c4b62-142">Response</span></span>
<span data-ttu-id="c4b62-143">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c4b62-143">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4b62-144">示例</span><span class="sxs-lookup"><span data-stu-id="c4b62-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4b62-145">请求</span><span class="sxs-lookup"><span data-stu-id="c4b62-145">Request</span></span>
<span data-ttu-id="c4b62-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c4b62-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicesWithoutCloudIdentity
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceWithoutCloudIdentity",
  "deviceName": "Device Name value",
  "azureAdDeviceId": "Azure Ad Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="c4b62-147">响应</span><span class="sxs-lookup"><span data-stu-id="c4b62-147">Response</span></span>
<span data-ttu-id="c4b62-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c4b62-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceWithoutCloudIdentity",
  "id": "80537287-7287-8053-8772-538087725380",
  "deviceName": "Device Name value",
  "azureAdDeviceId": "Azure Ad Device Id value"
}
```




