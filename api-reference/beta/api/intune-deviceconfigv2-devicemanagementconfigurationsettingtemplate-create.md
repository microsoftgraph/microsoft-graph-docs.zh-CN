---
title: 创建 deviceManagementConfigurationSettingTemplate
description: 创建新的 deviceManagementConfigurationSettingTemplate 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75e4f8bdb6cfa6761daf29695cb64d2b04425840
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665867"
---
# <a name="create-devicemanagementconfigurationsettingtemplate"></a><span data-ttu-id="2d22c-103">创建 deviceManagementConfigurationSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="2d22c-103">Create deviceManagementConfigurationSettingTemplate</span></span>

<span data-ttu-id="2d22c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d22c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d22c-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2d22c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d22c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d22c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d22c-107">创建新的 [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2d22c-107">Create a new [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d22c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2d22c-108">Prerequisites</span></span>
<span data-ttu-id="2d22c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d22c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d22c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d22c-111">Permission type</span></span>|<span data-ttu-id="2d22c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d22c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d22c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d22c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2d22c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d22c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d22c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d22c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d22c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d22c-116">Not supported.</span></span>|
|<span data-ttu-id="2d22c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d22c-117">Application</span></span>|<span data-ttu-id="2d22c-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d22c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d22c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d22c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templateSettings
POST /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates
```

## <a name="request-headers"></a><span data-ttu-id="2d22c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d22c-120">Request headers</span></span>
|<span data-ttu-id="2d22c-121">标头</span><span class="sxs-lookup"><span data-stu-id="2d22c-121">Header</span></span>|<span data-ttu-id="2d22c-122">值</span><span class="sxs-lookup"><span data-stu-id="2d22c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d22c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d22c-123">Authorization</span></span>|<span data-ttu-id="2d22c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2d22c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d22c-125">接受</span><span class="sxs-lookup"><span data-stu-id="2d22c-125">Accept</span></span>|<span data-ttu-id="2d22c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2d22c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d22c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d22c-127">Request body</span></span>
<span data-ttu-id="2d22c-128">在请求正文中，提供 deviceManagementConfigurationSettingTemplate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d22c-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingTemplate object.</span></span>

<span data-ttu-id="2d22c-129">下表显示创建 deviceManagementConfigurationSettingTemplate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2d22c-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingTemplate.</span></span>

|<span data-ttu-id="2d22c-130">属性</span><span class="sxs-lookup"><span data-stu-id="2d22c-130">Property</span></span>|<span data-ttu-id="2d22c-131">类型</span><span class="sxs-lookup"><span data-stu-id="2d22c-131">Type</span></span>|<span data-ttu-id="2d22c-132">说明</span><span class="sxs-lookup"><span data-stu-id="2d22c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d22c-133">id</span><span class="sxs-lookup"><span data-stu-id="2d22c-133">id</span></span>|<span data-ttu-id="2d22c-134">String</span><span class="sxs-lookup"><span data-stu-id="2d22c-134">String</span></span>|<span data-ttu-id="2d22c-135">包含此设置模板的策略模板中此设置模板的键。</span><span class="sxs-lookup"><span data-stu-id="2d22c-135">Key of this setting template within the policy template which contains it.</span></span> <span data-ttu-id="2d22c-136">自动生成。</span><span class="sxs-lookup"><span data-stu-id="2d22c-136">Automatically generated.</span></span>|
|<span data-ttu-id="2d22c-137">settingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="2d22c-137">settingInstanceTemplate</span></span>|[<span data-ttu-id="2d22c-138">deviceManagementConfigurationSettingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="2d22c-138">deviceManagementConfigurationSettingInstanceTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)|<span data-ttu-id="2d22c-139">设置实例模板</span><span class="sxs-lookup"><span data-stu-id="2d22c-139">Setting Instance Template</span></span>|



## <a name="response"></a><span data-ttu-id="2d22c-140">响应</span><span class="sxs-lookup"><span data-stu-id="2d22c-140">Response</span></span>
<span data-ttu-id="2d22c-141">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2d22c-141">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d22c-142">示例</span><span class="sxs-lookup"><span data-stu-id="2d22c-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d22c-143">请求</span><span class="sxs-lookup"><span data-stu-id="2d22c-143">Request</span></span>
<span data-ttu-id="2d22c-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d22c-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templateSettings
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

### <a name="response"></a><span data-ttu-id="2d22c-145">响应</span><span class="sxs-lookup"><span data-stu-id="2d22c-145">Response</span></span>
<span data-ttu-id="2d22c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2d22c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




