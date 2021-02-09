---
title: 列出 deviceManagementConfigurationSettingDefinitions
description: 列出 deviceManagementConfigurationSettingDefinition 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cc5464e663a06c3290f4bded620681ec10c91566
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161059"
---
# <a name="list-devicemanagementconfigurationsettingdefinitions"></a><span data-ttu-id="dad14-103">列出 deviceManagementConfigurationSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="dad14-103">List deviceManagementConfigurationSettingDefinitions</span></span>

<span data-ttu-id="dad14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dad14-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dad14-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dad14-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dad14-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dad14-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dad14-107">列出 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dad14-107">List properties and relationships of the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dad14-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dad14-108">Prerequisites</span></span>
<span data-ttu-id="dad14-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dad14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dad14-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dad14-111">Permission type</span></span>|<span data-ttu-id="dad14-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dad14-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dad14-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dad14-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dad14-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dad14-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dad14-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dad14-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dad14-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dad14-116">Not supported.</span></span>|
|<span data-ttu-id="dad14-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dad14-117">Application</span></span>|<span data-ttu-id="dad14-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dad14-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dad14-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dad14-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationSettings
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="dad14-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dad14-120">Request headers</span></span>
|<span data-ttu-id="dad14-121">标头</span><span class="sxs-lookup"><span data-stu-id="dad14-121">Header</span></span>|<span data-ttu-id="dad14-122">值</span><span class="sxs-lookup"><span data-stu-id="dad14-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dad14-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dad14-123">Authorization</span></span>|<span data-ttu-id="dad14-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dad14-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dad14-125">接受</span><span class="sxs-lookup"><span data-stu-id="dad14-125">Accept</span></span>|<span data-ttu-id="dad14-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dad14-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dad14-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dad14-127">Request body</span></span>
<span data-ttu-id="dad14-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dad14-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dad14-129">响应</span><span class="sxs-lookup"><span data-stu-id="dad14-129">Response</span></span>
<span data-ttu-id="dad14-130">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dad14-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dad14-131">示例</span><span class="sxs-lookup"><span data-stu-id="dad14-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dad14-132">请求</span><span class="sxs-lookup"><span data-stu-id="dad14-132">Request</span></span>
<span data-ttu-id="dad14-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dad14-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationSettings
```

### <a name="response"></a><span data-ttu-id="dad14-134">响应</span><span class="sxs-lookup"><span data-stu-id="dad14-134">Response</span></span>
<span data-ttu-id="dad14-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dad14-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1216

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDefinition",
      "applicability": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
        "description": "Description value",
        "platform": "macOS",
        "deviceMode": "kiosk",
        "technologies": "mdm"
      },
      "accessTypes": "add",
      "keywords": [
        "Keywords value"
      ],
      "infoUrls": [
        "Info Urls value"
      ],
      "occurrence": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
        "minDeviceOccurrence": 3,
        "maxDeviceOccurrence": 3
      },
      "baseUri": "Base Uri value",
      "offsetUri": "Offset Uri value",
      "rootDefinitionId": "Root Definition Id value",
      "categoryId": "Category Id value",
      "settingUsage": "configuration",
      "uxBehavior": "dropdown",
      "id": "7af649e5-49e5-7af6-e549-f67ae549f67a",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value",
      "version": "Version value"
    }
  ]
}
```




