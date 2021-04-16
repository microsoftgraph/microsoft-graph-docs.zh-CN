---
title: assignedAccessMultiModeProfiles 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 68a2f17e040c76ad51e244c8b385ae797f9aab23
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864275"
---
# <a name="assignedaccessmultimodeprofiles-action"></a><span data-ttu-id="aa718-103">assignedAccessMultiModeProfiles 操作</span><span class="sxs-lookup"><span data-stu-id="aa718-103">assignedAccessMultiModeProfiles action</span></span>

<span data-ttu-id="aa718-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa718-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa718-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aa718-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa718-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aa718-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa718-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="aa718-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa718-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="aa718-108">Prerequisites</span></span>
<span data-ttu-id="aa718-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa718-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa718-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa718-111">Permission type</span></span>|<span data-ttu-id="aa718-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aa718-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa718-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa718-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="aa718-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="aa718-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="aa718-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa718-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="aa718-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa718-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa718-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa718-117">Not supported.</span></span>|
|<span data-ttu-id="aa718-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa718-118">Application</span></span>||
| <span data-ttu-id="aa718-119">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="aa718-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="aa718-120">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="aa718-120">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa718-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa718-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assignedAccessMultiModeProfiles
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a><span data-ttu-id="aa718-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa718-122">Request headers</span></span>
|<span data-ttu-id="aa718-123">标头</span><span class="sxs-lookup"><span data-stu-id="aa718-123">Header</span></span>|<span data-ttu-id="aa718-124">值</span><span class="sxs-lookup"><span data-stu-id="aa718-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa718-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa718-125">Authorization</span></span>|<span data-ttu-id="aa718-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aa718-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa718-127">接受</span><span class="sxs-lookup"><span data-stu-id="aa718-127">Accept</span></span>|<span data-ttu-id="aa718-128">application/json</span><span class="sxs-lookup"><span data-stu-id="aa718-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa718-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa718-129">Request body</span></span>
<span data-ttu-id="aa718-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa718-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="aa718-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="aa718-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="aa718-132">属性</span><span class="sxs-lookup"><span data-stu-id="aa718-132">Property</span></span>|<span data-ttu-id="aa718-133">类型</span><span class="sxs-lookup"><span data-stu-id="aa718-133">Type</span></span>|<span data-ttu-id="aa718-134">说明</span><span class="sxs-lookup"><span data-stu-id="aa718-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa718-135">assignedAccessMultiModeProfiles</span><span class="sxs-lookup"><span data-stu-id="aa718-135">assignedAccessMultiModeProfiles</span></span>|<span data-ttu-id="aa718-136">windowsAssignedAccessProfile 集合</span><span class="sxs-lookup"><span data-stu-id="aa718-136">windowsAssignedAccessProfile collection</span></span>|<span data-ttu-id="aa718-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="aa718-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="aa718-138">响应</span><span class="sxs-lookup"><span data-stu-id="aa718-138">Response</span></span>
<span data-ttu-id="aa718-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="aa718-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aa718-140">示例</span><span class="sxs-lookup"><span data-stu-id="aa718-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa718-141">请求</span><span class="sxs-lookup"><span data-stu-id="aa718-141">Request</span></span>
<span data-ttu-id="aa718-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aa718-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aa718-143">响应</span><span class="sxs-lookup"><span data-stu-id="aa718-143">Response</span></span>
<span data-ttu-id="aa718-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aa718-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







