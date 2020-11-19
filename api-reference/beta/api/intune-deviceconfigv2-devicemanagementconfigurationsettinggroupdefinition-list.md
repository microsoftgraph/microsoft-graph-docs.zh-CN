---
title: 列出 deviceManagementConfigurationSettingGroupDefinitions
description: 列出 deviceManagementConfigurationSettingGroupDefinition 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 045d4572f166b7755d4e2b50704fe086e7320fc7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241588"
---
# <a name="list-devicemanagementconfigurationsettinggroupdefinitions"></a><span data-ttu-id="874dc-103">列出 deviceManagementConfigurationSettingGroupDefinitions</span><span class="sxs-lookup"><span data-stu-id="874dc-103">List deviceManagementConfigurationSettingGroupDefinitions</span></span>

<span data-ttu-id="874dc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="874dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="874dc-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="874dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="874dc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="874dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="874dc-107">列出 [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="874dc-107">List properties and relationships of the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="874dc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="874dc-108">Prerequisites</span></span>
<span data-ttu-id="874dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="874dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="874dc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="874dc-111">Permission type</span></span>|<span data-ttu-id="874dc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="874dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="874dc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="874dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="874dc-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="874dc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="874dc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="874dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="874dc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="874dc-116">Not supported.</span></span>|
|<span data-ttu-id="874dc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="874dc-117">Application</span></span>|<span data-ttu-id="874dc-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="874dc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="874dc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="874dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationSettings
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="874dc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="874dc-120">Request headers</span></span>
|<span data-ttu-id="874dc-121">标头</span><span class="sxs-lookup"><span data-stu-id="874dc-121">Header</span></span>|<span data-ttu-id="874dc-122">值</span><span class="sxs-lookup"><span data-stu-id="874dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="874dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="874dc-123">Authorization</span></span>|<span data-ttu-id="874dc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="874dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="874dc-125">接受</span><span class="sxs-lookup"><span data-stu-id="874dc-125">Accept</span></span>|<span data-ttu-id="874dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="874dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="874dc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="874dc-127">Request body</span></span>
<span data-ttu-id="874dc-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="874dc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="874dc-129">响应</span><span class="sxs-lookup"><span data-stu-id="874dc-129">Response</span></span>
<span data-ttu-id="874dc-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="874dc-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="874dc-131">示例</span><span class="sxs-lookup"><span data-stu-id="874dc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="874dc-132">请求</span><span class="sxs-lookup"><span data-stu-id="874dc-132">Request</span></span>
<span data-ttu-id="874dc-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="874dc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationSettings
```

### <a name="response"></a><span data-ttu-id="874dc-134">响应</span><span class="sxs-lookup"><span data-stu-id="874dc-134">Response</span></span>
<span data-ttu-id="874dc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="874dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1722

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupDefinition",
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
      "id": "95dc9604-9604-95dc-0496-dc950496dc95",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value",
      "version": "Version value",
      "childIds": [
        "Child Ids value"
      ],
      "dependentOn": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
          "dependentOn": "Dependent On value",
          "parentSettingId": "Parent Setting Id value"
        }
      ],
      "dependedOnBy": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
          "dependedOnBy": "Depended On By value",
          "required": true
        }
      ]
    }
  ]
}
```




