---
title: 列出 deviceManagementConfigurationPolicyTemplates
description: 列出 deviceManagementConfigurationPolicyTemplate 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: abc6d85ecf76c4235d0277ceaf50f3f0655e4822
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665690"
---
# <a name="list-devicemanagementconfigurationpolicytemplates"></a><span data-ttu-id="77934-103">列出 deviceManagementConfigurationPolicyTemplates</span><span class="sxs-lookup"><span data-stu-id="77934-103">List deviceManagementConfigurationPolicyTemplates</span></span>

<span data-ttu-id="77934-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77934-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77934-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="77934-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77934-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77934-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77934-107">列出 [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77934-107">List properties and relationships of the [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77934-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="77934-108">Prerequisites</span></span>
<span data-ttu-id="77934-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77934-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77934-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="77934-111">Permission type</span></span>|<span data-ttu-id="77934-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77934-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77934-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77934-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77934-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77934-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77934-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77934-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77934-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="77934-116">Not supported.</span></span>|
|<span data-ttu-id="77934-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="77934-117">Application</span></span>|<span data-ttu-id="77934-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77934-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77934-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77934-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationPolicyTemplates
```

## <a name="request-headers"></a><span data-ttu-id="77934-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="77934-120">Request headers</span></span>
|<span data-ttu-id="77934-121">标头</span><span class="sxs-lookup"><span data-stu-id="77934-121">Header</span></span>|<span data-ttu-id="77934-122">值</span><span class="sxs-lookup"><span data-stu-id="77934-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77934-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77934-123">Authorization</span></span>|<span data-ttu-id="77934-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="77934-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77934-125">接受</span><span class="sxs-lookup"><span data-stu-id="77934-125">Accept</span></span>|<span data-ttu-id="77934-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77934-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77934-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="77934-127">Request body</span></span>
<span data-ttu-id="77934-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77934-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77934-129">响应</span><span class="sxs-lookup"><span data-stu-id="77934-129">Response</span></span>
<span data-ttu-id="77934-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="77934-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77934-131">示例</span><span class="sxs-lookup"><span data-stu-id="77934-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="77934-132">请求</span><span class="sxs-lookup"><span data-stu-id="77934-132">Request</span></span>
<span data-ttu-id="77934-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="77934-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationPolicyTemplates
```

### <a name="response"></a><span data-ttu-id="77934-134">响应</span><span class="sxs-lookup"><span data-stu-id="77934-134">Response</span></span>
<span data-ttu-id="77934-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77934-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 587

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
      "id": "424ddb9a-db9a-424d-9adb-4d429adb4d42",
      "baseId": "Base Id value",
      "version": 7,
      "displayName": "Display Name value",
      "description": "Description value",
      "displayVersion": "Display Version value",
      "lifecycleState": "draft",
      "platforms": "macOS",
      "technologies": "mdm",
      "templateFamily": "endpointSecurityAntivirus",
      "allowUnmanagedSettings": true,
      "settingTemplateCount": 4
    }
  ]
}
```




