---
title: 创建 managedDeviceMobileAppConfigurationAssignment
description: 创建新的 managedDeviceMobileAppConfigurationAssignment 对象。
author: tfitzmac
ms.openlocfilehash: 8418b853c4d82f0a56d592a90542505f0355df0b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342775"
---
# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="0e1be-103">创建 managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0e1be-103">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="0e1be-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0e1be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e1be-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0e1be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e1be-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0e1be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e1be-107">创建新的 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e1be-107">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e1be-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0e1be-108">Prerequisites</span></span>
<span data-ttu-id="0e1be-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0e1be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e1be-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e1be-111">Permission type</span></span>|<span data-ttu-id="0e1be-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0e1be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e1be-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e1be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e1be-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e1be-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0e1be-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e1be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e1be-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e1be-116">Not supported.</span></span>|
|<span data-ttu-id="0e1be-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e1be-117">Application</span></span>|<span data-ttu-id="0e1be-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e1be-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e1be-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e1be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0e1be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e1be-120">Request headers</span></span>
|<span data-ttu-id="0e1be-121">标头</span><span class="sxs-lookup"><span data-stu-id="0e1be-121">Header</span></span>|<span data-ttu-id="0e1be-122">值</span><span class="sxs-lookup"><span data-stu-id="0e1be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e1be-123">授权</span><span class="sxs-lookup"><span data-stu-id="0e1be-123">Authorization</span></span>|<span data-ttu-id="0e1be-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0e1be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e1be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0e1be-125">Accept</span></span>|<span data-ttu-id="0e1be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e1be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e1be-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e1be-127">Request body</span></span>
<span data-ttu-id="0e1be-128">在请求正文中，提供 managedDeviceMobileAppConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e1be-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="0e1be-129">下表显示创建 managedDeviceMobileAppConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0e1be-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="0e1be-130">属性</span><span class="sxs-lookup"><span data-stu-id="0e1be-130">Property</span></span>|<span data-ttu-id="0e1be-131">类型</span><span class="sxs-lookup"><span data-stu-id="0e1be-131">Type</span></span>|<span data-ttu-id="0e1be-132">说明</span><span class="sxs-lookup"><span data-stu-id="0e1be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e1be-133">id</span><span class="sxs-lookup"><span data-stu-id="0e1be-133">id</span></span>|<span data-ttu-id="0e1be-134">String</span><span class="sxs-lookup"><span data-stu-id="0e1be-134">String</span></span>|<span data-ttu-id="0e1be-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0e1be-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="0e1be-136">target</span><span class="sxs-lookup"><span data-stu-id="0e1be-136">target</span></span>|[<span data-ttu-id="0e1be-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0e1be-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0e1be-138">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="0e1be-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="0e1be-139">响应</span><span class="sxs-lookup"><span data-stu-id="0e1be-139">Response</span></span>
<span data-ttu-id="0e1be-140">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e1be-140">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e1be-141">示例</span><span class="sxs-lookup"><span data-stu-id="0e1be-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="0e1be-142">请求</span><span class="sxs-lookup"><span data-stu-id="0e1be-142">Request</span></span>
<span data-ttu-id="0e1be-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e1be-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="0e1be-144">响应</span><span class="sxs-lookup"><span data-stu-id="0e1be-144">Response</span></span>
<span data-ttu-id="0e1be-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e1be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





