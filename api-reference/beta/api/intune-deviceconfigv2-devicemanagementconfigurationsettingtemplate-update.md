---
title: 更新 deviceManagementConfigurationSettingTemplate
description: 更新 deviceManagementConfigurationSettingTemplate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 98cd26899ec0b2661635dc0758997ecb876cf7d3
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664834"
---
# <a name="update-devicemanagementconfigurationsettingtemplate"></a><span data-ttu-id="d1b16-103">更新 deviceManagementConfigurationSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="d1b16-103">Update deviceManagementConfigurationSettingTemplate</span></span>

<span data-ttu-id="d1b16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1b16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1b16-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1b16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1b16-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1b16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1b16-107">更新 [deviceManagementConfigurationSettingTemplate 对象](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="d1b16-107">Update the properties of a [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1b16-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d1b16-108">Prerequisites</span></span>
<span data-ttu-id="d1b16-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1b16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1b16-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1b16-111">Permission type</span></span>|<span data-ttu-id="d1b16-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1b16-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1b16-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1b16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1b16-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1b16-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1b16-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1b16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1b16-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1b16-116">Not supported.</span></span>|
|<span data-ttu-id="d1b16-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1b16-117">Application</span></span>|<span data-ttu-id="d1b16-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1b16-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1b16-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1b16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/templateSettings/{deviceManagementConfigurationSettingTemplateId}
PATCH /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="d1b16-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1b16-120">Request headers</span></span>
|<span data-ttu-id="d1b16-121">标头</span><span class="sxs-lookup"><span data-stu-id="d1b16-121">Header</span></span>|<span data-ttu-id="d1b16-122">值</span><span class="sxs-lookup"><span data-stu-id="d1b16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1b16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1b16-123">Authorization</span></span>|<span data-ttu-id="d1b16-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d1b16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1b16-125">接受</span><span class="sxs-lookup"><span data-stu-id="d1b16-125">Accept</span></span>|<span data-ttu-id="d1b16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1b16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1b16-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1b16-127">Request body</span></span>
<span data-ttu-id="d1b16-128">在请求正文中，提供 [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1b16-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) object.</span></span>

<span data-ttu-id="d1b16-129">下表显示创建 [deviceManagementConfigurationSettingTemplate 时所需的属性](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="d1b16-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md).</span></span>

|<span data-ttu-id="d1b16-130">属性</span><span class="sxs-lookup"><span data-stu-id="d1b16-130">Property</span></span>|<span data-ttu-id="d1b16-131">类型</span><span class="sxs-lookup"><span data-stu-id="d1b16-131">Type</span></span>|<span data-ttu-id="d1b16-132">说明</span><span class="sxs-lookup"><span data-stu-id="d1b16-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1b16-133">id</span><span class="sxs-lookup"><span data-stu-id="d1b16-133">id</span></span>|<span data-ttu-id="d1b16-134">String</span><span class="sxs-lookup"><span data-stu-id="d1b16-134">String</span></span>|<span data-ttu-id="d1b16-135">包含此设置模板的策略模板中此设置模板的键。</span><span class="sxs-lookup"><span data-stu-id="d1b16-135">Key of this setting template within the policy template which contains it.</span></span> <span data-ttu-id="d1b16-136">自动生成。</span><span class="sxs-lookup"><span data-stu-id="d1b16-136">Automatically generated.</span></span>|
|<span data-ttu-id="d1b16-137">settingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="d1b16-137">settingInstanceTemplate</span></span>|[<span data-ttu-id="d1b16-138">deviceManagementConfigurationSettingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="d1b16-138">deviceManagementConfigurationSettingInstanceTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|<span data-ttu-id="d1b16-139">设置实例模板</span><span class="sxs-lookup"><span data-stu-id="d1b16-139">Setting Instance Template</span></span>|



## <a name="response"></a><span data-ttu-id="d1b16-140">响应</span><span class="sxs-lookup"><span data-stu-id="d1b16-140">Response</span></span>
<span data-ttu-id="d1b16-141">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d1b16-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1b16-142">示例</span><span class="sxs-lookup"><span data-stu-id="d1b16-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1b16-143">请求</span><span class="sxs-lookup"><span data-stu-id="d1b16-143">Request</span></span>
<span data-ttu-id="d1b16-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d1b16-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templateSettings/{deviceManagementConfigurationSettingTemplateId}
Content-type: application/json
Content-length: 784

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingTemplate",
  "settingInstanceTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
    "settingInstanceTemplateId": "Setting Instance Template Id value",
    "settingDefinitionId": "Setting Definition Id value",
    "isRequired": true,
    "simpleSettingValueTemplate": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
      "settingValueTemplateId": "Setting Value Template Id value",
      "defaultValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
        "constantValue": "Constant Value value"
      }
    }
  }
}
```

### <a name="response"></a><span data-ttu-id="d1b16-145">响应</span><span class="sxs-lookup"><span data-stu-id="d1b16-145">Response</span></span>
<span data-ttu-id="d1b16-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d1b16-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 833

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingTemplate",
  "id": "203fd028-d028-203f-28d0-3f2028d03f20",
  "settingInstanceTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
    "settingInstanceTemplateId": "Setting Instance Template Id value",
    "settingDefinitionId": "Setting Definition Id value",
    "isRequired": true,
    "simpleSettingValueTemplate": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
      "settingValueTemplateId": "Setting Value Template Id value",
      "defaultValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
        "constantValue": "Constant Value value"
      }
    }
  }
}
```




