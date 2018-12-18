---
title: 更新 managedDeviceMobileAppConfigurationAssignment
description: 更新 managedDeviceMobileAppConfigurationAssignment 对象的属性。
author: tfitzmac
ms.openlocfilehash: a9c1c7b1f0af2ec49080d6b6e225d3923b7f37b5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301433"
---
# <a name="update-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="1fd03-103">更新 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1fd03-103">Update managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="1fd03-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1fd03-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1fd03-105">更新 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1fd03-105">Update the properties of a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1fd03-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1fd03-106">Prerequisites</span></span>
<span data-ttu-id="1fd03-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1fd03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fd03-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1fd03-109">Permission type</span></span>|<span data-ttu-id="1fd03-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1fd03-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fd03-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1fd03-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1fd03-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fd03-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1fd03-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1fd03-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fd03-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fd03-114">Not supported.</span></span>|
|<span data-ttu-id="1fd03-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1fd03-115">Application</span></span>|<span data-ttu-id="1fd03-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fd03-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fd03-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1fd03-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1fd03-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1fd03-118">Request headers</span></span>
|<span data-ttu-id="1fd03-119">标头</span><span class="sxs-lookup"><span data-stu-id="1fd03-119">Header</span></span>|<span data-ttu-id="1fd03-120">值</span><span class="sxs-lookup"><span data-stu-id="1fd03-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fd03-121">授权</span><span class="sxs-lookup"><span data-stu-id="1fd03-121">Authorization</span></span>|<span data-ttu-id="1fd03-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1fd03-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fd03-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1fd03-123">Accept</span></span>|<span data-ttu-id="1fd03-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1fd03-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fd03-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1fd03-125">Request body</span></span>
<span data-ttu-id="1fd03-126">在请求正文中，提供 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fd03-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>

<span data-ttu-id="1fd03-127">下表显示创建 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1fd03-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).</span></span>

|<span data-ttu-id="1fd03-128">属性</span><span class="sxs-lookup"><span data-stu-id="1fd03-128">Property</span></span>|<span data-ttu-id="1fd03-129">类型</span><span class="sxs-lookup"><span data-stu-id="1fd03-129">Type</span></span>|<span data-ttu-id="1fd03-130">说明</span><span class="sxs-lookup"><span data-stu-id="1fd03-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fd03-131">id</span><span class="sxs-lookup"><span data-stu-id="1fd03-131">id</span></span>|<span data-ttu-id="1fd03-132">String</span><span class="sxs-lookup"><span data-stu-id="1fd03-132">String</span></span>|<span data-ttu-id="1fd03-133">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1fd03-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1fd03-134">target</span><span class="sxs-lookup"><span data-stu-id="1fd03-134">target</span></span>|[<span data-ttu-id="1fd03-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1fd03-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1fd03-136">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="1fd03-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="1fd03-137">响应</span><span class="sxs-lookup"><span data-stu-id="1fd03-137">Response</span></span>
<span data-ttu-id="1fd03-138">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1fd03-138">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fd03-139">示例</span><span class="sxs-lookup"><span data-stu-id="1fd03-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="1fd03-140">请求</span><span class="sxs-lookup"><span data-stu-id="1fd03-140">Request</span></span>
<span data-ttu-id="1fd03-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1fd03-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="1fd03-142">响应</span><span class="sxs-lookup"><span data-stu-id="1fd03-142">Response</span></span>
<span data-ttu-id="1fd03-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1fd03-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



