---
title: 创建 mobileAppProvisioningConfigGroupAssignment
description: 创建新的 mobileAppProvisioningConfigGroupAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 173f8704ffb44750e3ef382160363dc6e1ce2e48
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139683"
---
# <a name="create-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="700a8-103">创建 mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="700a8-103">Create mobileAppProvisioningConfigGroupAssignment</span></span>

<span data-ttu-id="700a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="700a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="700a8-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="700a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="700a8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="700a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="700a8-107">创建新的 [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="700a8-107">Create a new [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="700a8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="700a8-108">Prerequisites</span></span>
<span data-ttu-id="700a8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="700a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="700a8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="700a8-111">Permission type</span></span>|<span data-ttu-id="700a8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="700a8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="700a8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="700a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="700a8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="700a8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="700a8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="700a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="700a8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="700a8-116">Not supported.</span></span>|
|<span data-ttu-id="700a8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="700a8-117">Application</span></span>|<span data-ttu-id="700a8-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="700a8-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="700a8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="700a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="700a8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="700a8-120">Request headers</span></span>
|<span data-ttu-id="700a8-121">标头</span><span class="sxs-lookup"><span data-stu-id="700a8-121">Header</span></span>|<span data-ttu-id="700a8-122">值</span><span class="sxs-lookup"><span data-stu-id="700a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="700a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="700a8-123">Authorization</span></span>|<span data-ttu-id="700a8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="700a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="700a8-125">接受</span><span class="sxs-lookup"><span data-stu-id="700a8-125">Accept</span></span>|<span data-ttu-id="700a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="700a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="700a8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="700a8-127">Request body</span></span>
<span data-ttu-id="700a8-128">在请求正文中，提供 mobileAppProvisioningConfigGroupAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="700a8-128">In the request body, supply a JSON representation for the mobileAppProvisioningConfigGroupAssignment object.</span></span>

<span data-ttu-id="700a8-129">下表显示创建 mobileAppProvisioningConfigGroupAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="700a8-129">The following table shows the properties that are required when you create the mobileAppProvisioningConfigGroupAssignment.</span></span>

|<span data-ttu-id="700a8-130">属性</span><span class="sxs-lookup"><span data-stu-id="700a8-130">Property</span></span>|<span data-ttu-id="700a8-131">类型</span><span class="sxs-lookup"><span data-stu-id="700a8-131">Type</span></span>|<span data-ttu-id="700a8-132">说明</span><span class="sxs-lookup"><span data-stu-id="700a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="700a8-133">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="700a8-133">targetGroupId</span></span>|<span data-ttu-id="700a8-134">String</span><span class="sxs-lookup"><span data-stu-id="700a8-134">String</span></span>|<span data-ttu-id="700a8-135">要定向应用预配配置的 AAD 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="700a8-135">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="700a8-136">id</span><span class="sxs-lookup"><span data-stu-id="700a8-136">id</span></span>|<span data-ttu-id="700a8-137">String</span><span class="sxs-lookup"><span data-stu-id="700a8-137">String</span></span>|<span data-ttu-id="700a8-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="700a8-138">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="700a8-139">响应</span><span class="sxs-lookup"><span data-stu-id="700a8-139">Response</span></span>
<span data-ttu-id="700a8-140">如果成功，此方法在响应 `201 Created` 正文中返回 响应 [代码和 mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="700a8-140">If successful, this method returns a `201 Created` response code and a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="700a8-141">示例</span><span class="sxs-lookup"><span data-stu-id="700a8-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="700a8-142">请求</span><span class="sxs-lookup"><span data-stu-id="700a8-142">Request</span></span>
<span data-ttu-id="700a8-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="700a8-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="700a8-144">响应</span><span class="sxs-lookup"><span data-stu-id="700a8-144">Response</span></span>
<span data-ttu-id="700a8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="700a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```




