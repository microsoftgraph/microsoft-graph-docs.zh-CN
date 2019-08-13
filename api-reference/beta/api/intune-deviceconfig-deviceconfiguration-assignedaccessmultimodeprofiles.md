---
title: assignedAccessMultiModeProfiles 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 094276c28cad82d60958e97d65134672f333c579
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346021"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="8a444-103">assignedAccessMultiModeProfiles 操作</span><span class="sxs-lookup"><span data-stu-id="8a444-103">assignedAccessMultiModeProfiles action</span></span>

> <span data-ttu-id="8a444-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8a444-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a444-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8a444-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a444-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8a444-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a444-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8a444-107">Prerequisites</span></span>
<span data-ttu-id="8a444-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a444-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a444-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a444-110">Permission type</span></span>|<span data-ttu-id="8a444-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8a444-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a444-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a444-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8a444-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a444-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8a444-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a444-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a444-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a444-115">Not supported.</span></span>|
|<span data-ttu-id="8a444-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a444-116">Application</span></span>|<span data-ttu-id="8a444-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a444-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a444-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a444-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="8a444-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a444-119">Request headers</span></span>
|<span data-ttu-id="8a444-120">标头</span><span class="sxs-lookup"><span data-stu-id="8a444-120">Header</span></span>|<span data-ttu-id="8a444-121">值</span><span class="sxs-lookup"><span data-stu-id="8a444-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a444-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a444-122">Authorization</span></span>|<span data-ttu-id="8a444-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8a444-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a444-124">接受</span><span class="sxs-lookup"><span data-stu-id="8a444-124">Accept</span></span>|<span data-ttu-id="8a444-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8a444-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a444-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a444-126">Request body</span></span>
<span data-ttu-id="8a444-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a444-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8a444-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="8a444-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8a444-129">属性</span><span class="sxs-lookup"><span data-stu-id="8a444-129">Property</span></span>|<span data-ttu-id="8a444-130">类型</span><span class="sxs-lookup"><span data-stu-id="8a444-130">Type</span></span>|<span data-ttu-id="8a444-131">说明</span><span class="sxs-lookup"><span data-stu-id="8a444-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a444-132">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="8a444-132">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="8a444-133">windowsAssignedAccessProfile 集合</span><span class="sxs-lookup"><span data-stu-id="8a444-133">windowsAssignedAccessProfile collection</span></span>|<span data-ttu-id="8a444-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8a444-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8a444-135">响应</span><span class="sxs-lookup"><span data-stu-id="8a444-135">Response</span></span>
<span data-ttu-id="8a444-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8a444-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8a444-137">示例</span><span class="sxs-lookup"><span data-stu-id="8a444-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a444-138">请求</span><span class="sxs-lookup"><span data-stu-id="8a444-138">Request</span></span>
<span data-ttu-id="8a444-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8a444-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8a444-140">响应</span><span class="sxs-lookup"><span data-stu-id="8a444-140">Response</span></span>
<span data-ttu-id="8a444-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8a444-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






