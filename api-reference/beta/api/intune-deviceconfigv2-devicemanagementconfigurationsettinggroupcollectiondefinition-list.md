---
title: 列出 deviceManagementConfigurationSettingGroupCollectionDefinitions
description: 列出 deviceManagementConfigurationSettingGroupCollectionDefinition 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b9d511522047ba7e677346dbc3af1b0527fc6750
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241603"
---
# <a name="list-devicemanagementconfigurationsettinggroupcollectiondefinitions"></a><span data-ttu-id="1bdb8-103">列出 deviceManagementConfigurationSettingGroupCollectionDefinitions</span><span class="sxs-lookup"><span data-stu-id="1bdb8-103">List deviceManagementConfigurationSettingGroupCollectionDefinitions</span></span>

<span data-ttu-id="1bdb8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bdb8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bdb8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1bdb8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bdb8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1bdb8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bdb8-107">列出 [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1bdb8-107">List properties and relationships of the [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bdb8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1bdb8-108">Prerequisites</span></span>
<span data-ttu-id="1bdb8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1bdb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bdb8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bdb8-111">Permission type</span></span>|<span data-ttu-id="1bdb8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1bdb8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bdb8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bdb8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1bdb8-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bdb8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1bdb8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bdb8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bdb8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bdb8-116">Not supported.</span></span>|
|<span data-ttu-id="1bdb8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bdb8-117">Application</span></span>|<span data-ttu-id="1bdb8-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1bdb8-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bdb8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bdb8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationSettings
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="1bdb8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bdb8-120">Request headers</span></span>
|<span data-ttu-id="1bdb8-121">标头</span><span class="sxs-lookup"><span data-stu-id="1bdb8-121">Header</span></span>|<span data-ttu-id="1bdb8-122">值</span><span class="sxs-lookup"><span data-stu-id="1bdb8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bdb8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bdb8-123">Authorization</span></span>|<span data-ttu-id="1bdb8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1bdb8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bdb8-125">接受</span><span class="sxs-lookup"><span data-stu-id="1bdb8-125">Accept</span></span>|<span data-ttu-id="1bdb8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bdb8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bdb8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bdb8-127">Request body</span></span>
<span data-ttu-id="1bdb8-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1bdb8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bdb8-129">响应</span><span class="sxs-lookup"><span data-stu-id="1bdb8-129">Response</span></span>
<span data-ttu-id="1bdb8-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1bdb8-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bdb8-131">示例</span><span class="sxs-lookup"><span data-stu-id="1bdb8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bdb8-132">请求</span><span class="sxs-lookup"><span data-stu-id="1bdb8-132">Request</span></span>
<span data-ttu-id="1bdb8-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1bdb8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationSettings
```

### <a name="response"></a><span data-ttu-id="1bdb8-134">响应</span><span class="sxs-lookup"><span data-stu-id="1bdb8-134">Response</span></span>
<span data-ttu-id="1bdb8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1bdb8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1786

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionDefinition",
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
      "id": "739da194-a194-739d-94a1-9d7394a19d73",
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
      ],
      "maximumCount": 12,
      "minimumCount": 12
    }
  ]
}
```




