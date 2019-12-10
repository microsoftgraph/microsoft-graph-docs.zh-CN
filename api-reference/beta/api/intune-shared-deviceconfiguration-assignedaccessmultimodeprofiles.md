---
title: assignedAccessMultiModeProfiles 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9795d48fe744b78e301933d15aef48237e0e4343
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940080"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="6084c-103">assignedAccessMultiModeProfiles 操作</span><span class="sxs-lookup"><span data-stu-id="6084c-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="6084c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6084c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6084c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6084c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6084c-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6084c-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6084c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6084c-107">Prerequisites</span></span>
<span data-ttu-id="6084c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6084c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6084c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6084c-110">Permission type</span></span>|<span data-ttu-id="6084c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6084c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6084c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6084c-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6084c-113">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="6084c-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6084c-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6084c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6084c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6084c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6084c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6084c-116">Not supported.</span></span>|
|<span data-ttu-id="6084c-117">Application</span><span class="sxs-lookup"><span data-stu-id="6084c-117">Application</span></span>||
| <span data-ttu-id="6084c-118">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="6084c-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6084c-119">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6084c-119">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6084c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6084c-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="6084c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6084c-121">Request headers</span></span>
|<span data-ttu-id="6084c-122">标头</span><span class="sxs-lookup"><span data-stu-id="6084c-122">Header</span></span>|<span data-ttu-id="6084c-123">值</span><span class="sxs-lookup"><span data-stu-id="6084c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6084c-124">授权</span><span class="sxs-lookup"><span data-stu-id="6084c-124">Authorization</span></span>|<span data-ttu-id="6084c-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6084c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6084c-126">接受</span><span class="sxs-lookup"><span data-stu-id="6084c-126">Accept</span></span>|<span data-ttu-id="6084c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6084c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6084c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6084c-128">Request body</span></span>
<span data-ttu-id="6084c-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6084c-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6084c-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="6084c-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6084c-131">属性</span><span class="sxs-lookup"><span data-stu-id="6084c-131">Property</span></span>|<span data-ttu-id="6084c-132">类型</span><span class="sxs-lookup"><span data-stu-id="6084c-132">Type</span></span>|<span data-ttu-id="6084c-133">说明</span><span class="sxs-lookup"><span data-stu-id="6084c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6084c-134">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="6084c-134">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="6084c-135">windowsAssignedAccessProfile 集合</span><span class="sxs-lookup"><span data-stu-id="6084c-135">windowsAssignedAccessProfile collection</span></span>|<span data-ttu-id="6084c-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6084c-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6084c-137">响应</span><span class="sxs-lookup"><span data-stu-id="6084c-137">Response</span></span>
<span data-ttu-id="6084c-138">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6084c-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6084c-139">示例</span><span class="sxs-lookup"><span data-stu-id="6084c-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="6084c-140">请求</span><span class="sxs-lookup"><span data-stu-id="6084c-140">Request</span></span>
<span data-ttu-id="6084c-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6084c-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles

Content-type: application/json
Content-length: 528

{
  "assignedAccessMultiModeProfiles": [
    {
      "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
      "id": "cfa70299-0299-cfa7-9902-a7cf9902a7cf",
      "profileName": "Profile Name value",
      "showTaskBar": true,
      "appUserModelIds": [
        "App User Model Ids value"
      ],
      "desktopAppPaths": [
        "Desktop App Paths value"
      ],
      "userAccounts": [
        "User Accounts value"
      ],
      "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="6084c-142">响应</span><span class="sxs-lookup"><span data-stu-id="6084c-142">Response</span></span>
<span data-ttu-id="6084c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6084c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








