---
title: 列出 deviceManagementConfigurationSettingGroupDefinitions
description: 列出 deviceManagementConfigurationSettingGroupDefinition 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 173a649d15bc247a927ff42c709b2eb649426747
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665446"
---
# <a name="list-devicemanagementconfigurationsettinggroupdefinitions"></a><span data-ttu-id="bcd3a-103">列出 deviceManagementConfigurationSettingGroupDefinitions</span><span class="sxs-lookup"><span data-stu-id="bcd3a-103">List deviceManagementConfigurationSettingGroupDefinitions</span></span>

<span data-ttu-id="bcd3a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcd3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bcd3a-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bcd3a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcd3a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bcd3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcd3a-107">列出 [deviceManagementConfigurationSettingGroupDefinition 对象的属性和](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="bcd3a-107">List properties and relationships of the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcd3a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bcd3a-108">Prerequisites</span></span>
<span data-ttu-id="bcd3a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bcd3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcd3a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bcd3a-111">Permission type</span></span>|<span data-ttu-id="bcd3a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bcd3a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcd3a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bcd3a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bcd3a-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcd3a-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bcd3a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bcd3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcd3a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bcd3a-116">Not supported.</span></span>|
|<span data-ttu-id="bcd3a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bcd3a-117">Application</span></span>|<span data-ttu-id="bcd3a-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcd3a-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcd3a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bcd3a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reusableSettings
GET /deviceManagement/configurationSettings
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
GET /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="bcd3a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bcd3a-120">Request headers</span></span>
|<span data-ttu-id="bcd3a-121">标头</span><span class="sxs-lookup"><span data-stu-id="bcd3a-121">Header</span></span>|<span data-ttu-id="bcd3a-122">值</span><span class="sxs-lookup"><span data-stu-id="bcd3a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcd3a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcd3a-123">Authorization</span></span>|<span data-ttu-id="bcd3a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bcd3a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcd3a-125">接受</span><span class="sxs-lookup"><span data-stu-id="bcd3a-125">Accept</span></span>|<span data-ttu-id="bcd3a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bcd3a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcd3a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bcd3a-127">Request body</span></span>
<span data-ttu-id="bcd3a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bcd3a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcd3a-129">响应</span><span class="sxs-lookup"><span data-stu-id="bcd3a-129">Response</span></span>
<span data-ttu-id="bcd3a-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bcd3a-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcd3a-131">示例</span><span class="sxs-lookup"><span data-stu-id="bcd3a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcd3a-132">请求</span><span class="sxs-lookup"><span data-stu-id="bcd3a-132">Request</span></span>
<span data-ttu-id="bcd3a-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bcd3a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reusableSettings
```

### <a name="response"></a><span data-ttu-id="bcd3a-134">响应</span><span class="sxs-lookup"><span data-stu-id="bcd3a-134">Response</span></span>
<span data-ttu-id="bcd3a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bcd3a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2035

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
      "uxBehavior": "dropdown",
      "visibility": "settingsCatalog",
      "referredSettingInformationList": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
          "settingDefinitionId": "Setting Definition Id value"
        }
      ],
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




