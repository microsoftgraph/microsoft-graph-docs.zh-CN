---
title: 更新 iosLobAppProvisioningConfigurationAssignment
description: 更新 iosLobAppProvisioningConfigurationAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcc683aa78c0f4de1c1d8d579482971411726876
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960872"
---
# <a name="update-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="de2bb-103">更新 iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="de2bb-103">Update iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="de2bb-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="de2bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de2bb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="de2bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de2bb-106">更新[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="de2bb-106">Update the properties of a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de2bb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="de2bb-107">Prerequisites</span></span>
<span data-ttu-id="de2bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de2bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de2bb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="de2bb-110">Permission type</span></span>|<span data-ttu-id="de2bb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="de2bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de2bb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de2bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de2bb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de2bb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="de2bb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de2bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de2bb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="de2bb-115">Not supported.</span></span>|
|<span data-ttu-id="de2bb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="de2bb-116">Application</span></span>|<span data-ttu-id="de2bb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="de2bb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de2bb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de2bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="de2bb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="de2bb-119">Request headers</span></span>
|<span data-ttu-id="de2bb-120">标头</span><span class="sxs-lookup"><span data-stu-id="de2bb-120">Header</span></span>|<span data-ttu-id="de2bb-121">值</span><span class="sxs-lookup"><span data-stu-id="de2bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de2bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="de2bb-122">Authorization</span></span>|<span data-ttu-id="de2bb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="de2bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de2bb-124">接受</span><span class="sxs-lookup"><span data-stu-id="de2bb-124">Accept</span></span>|<span data-ttu-id="de2bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de2bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de2bb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="de2bb-126">Request body</span></span>
<span data-ttu-id="de2bb-127">在请求正文中, 提供[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de2bb-127">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

<span data-ttu-id="de2bb-128">下表显示创建[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="de2bb-128">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

|<span data-ttu-id="de2bb-129">属性</span><span class="sxs-lookup"><span data-stu-id="de2bb-129">Property</span></span>|<span data-ttu-id="de2bb-130">类型</span><span class="sxs-lookup"><span data-stu-id="de2bb-130">Type</span></span>|<span data-ttu-id="de2bb-131">说明</span><span class="sxs-lookup"><span data-stu-id="de2bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de2bb-132">id</span><span class="sxs-lookup"><span data-stu-id="de2bb-132">id</span></span>|<span data-ttu-id="de2bb-133">String</span><span class="sxs-lookup"><span data-stu-id="de2bb-133">String</span></span>|<span data-ttu-id="de2bb-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="de2bb-134">Key of the entity.</span></span>|
|<span data-ttu-id="de2bb-135">target</span><span class="sxs-lookup"><span data-stu-id="de2bb-135">target</span></span>|[<span data-ttu-id="de2bb-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="de2bb-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="de2bb-137">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="de2bb-137">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="de2bb-138">响应</span><span class="sxs-lookup"><span data-stu-id="de2bb-138">Response</span></span>
<span data-ttu-id="de2bb-139">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="de2bb-139">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de2bb-140">示例</span><span class="sxs-lookup"><span data-stu-id="de2bb-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="de2bb-141">请求</span><span class="sxs-lookup"><span data-stu-id="de2bb-141">Request</span></span>
<span data-ttu-id="de2bb-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de2bb-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="de2bb-143">响应</span><span class="sxs-lookup"><span data-stu-id="de2bb-143">Response</span></span>
<span data-ttu-id="de2bb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="de2bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




