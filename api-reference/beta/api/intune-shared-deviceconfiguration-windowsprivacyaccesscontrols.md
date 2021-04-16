---
title: windowsPrivacyAccessControls 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c11bfa219db514a2539cd7ae8608ba41889c5944
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864240"
---
# <a name="windowsprivacyaccesscontrols-action"></a><span data-ttu-id="e68f7-103">windowsPrivacyAccessControls 操作</span><span class="sxs-lookup"><span data-stu-id="e68f7-103">windowsPrivacyAccessControls action</span></span>

<span data-ttu-id="e68f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e68f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e68f7-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e68f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e68f7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e68f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e68f7-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e68f7-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e68f7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e68f7-108">Prerequisites</span></span>
<span data-ttu-id="e68f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e68f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e68f7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e68f7-111">Permission type</span></span>|<span data-ttu-id="e68f7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e68f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e68f7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e68f7-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e68f7-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="e68f7-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e68f7-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e68f7-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e68f7-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e68f7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e68f7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e68f7-117">Not supported.</span></span>|
|<span data-ttu-id="e68f7-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="e68f7-118">Application</span></span>||
| <span data-ttu-id="e68f7-119">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="e68f7-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e68f7-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e68f7-120">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e68f7-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e68f7-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/windowsPrivacyAccessControls
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="e68f7-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e68f7-122">Request headers</span></span>
|<span data-ttu-id="e68f7-123">标头</span><span class="sxs-lookup"><span data-stu-id="e68f7-123">Header</span></span>|<span data-ttu-id="e68f7-124">值</span><span class="sxs-lookup"><span data-stu-id="e68f7-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e68f7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e68f7-125">Authorization</span></span>|<span data-ttu-id="e68f7-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e68f7-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e68f7-127">接受</span><span class="sxs-lookup"><span data-stu-id="e68f7-127">Accept</span></span>|<span data-ttu-id="e68f7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e68f7-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e68f7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e68f7-129">Request body</span></span>
<span data-ttu-id="e68f7-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e68f7-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e68f7-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="e68f7-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e68f7-132">属性</span><span class="sxs-lookup"><span data-stu-id="e68f7-132">Property</span></span>|<span data-ttu-id="e68f7-133">类型</span><span class="sxs-lookup"><span data-stu-id="e68f7-133">Type</span></span>|<span data-ttu-id="e68f7-134">说明</span><span class="sxs-lookup"><span data-stu-id="e68f7-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e68f7-135">windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="e68f7-135">windowsPrivacyAccessControls</span></span>|<span data-ttu-id="e68f7-136">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e68f7-136">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="e68f7-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e68f7-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e68f7-138">响应</span><span class="sxs-lookup"><span data-stu-id="e68f7-138">Response</span></span>
<span data-ttu-id="e68f7-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e68f7-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e68f7-140">示例</span><span class="sxs-lookup"><span data-stu-id="e68f7-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e68f7-141">请求</span><span class="sxs-lookup"><span data-stu-id="e68f7-141">Request</span></span>
<span data-ttu-id="e68f7-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e68f7-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls

Content-type: application/json
Content-length: 379

{
  "windowsPrivacyAccessControls": [
    {
      "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
      "id": "03b15556-5556-03b1-5655-b1035655b103",
      "accessLevel": "forceAllow",
      "dataCategory": "accountInfo",
      "appPackageFamilyName": "App Package Family Name value",
      "appDisplayName": "App Display Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e68f7-143">响应</span><span class="sxs-lookup"><span data-stu-id="e68f7-143">Response</span></span>
<span data-ttu-id="e68f7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e68f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







