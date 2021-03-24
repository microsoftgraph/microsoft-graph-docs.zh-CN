---
title: 获取 deviceManagementComplexSettingDefinition
description: 读取 deviceManagementComplexSettingDefinition 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c8709c6003ce34a908a646c0a89c42c464219de6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128962"
---
# <a name="get-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="da326-103">获取 deviceManagementComplexSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="da326-103">Get deviceManagementComplexSettingDefinition</span></span>

<span data-ttu-id="da326-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da326-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da326-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da326-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da326-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da326-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da326-107">读取 [deviceManagementComplexSettingDefinition 对象的属性和](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="da326-107">Read properties and relationships of the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da326-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="da326-108">Prerequisites</span></span>
<span data-ttu-id="da326-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da326-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da326-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="da326-111">Permission type</span></span>|<span data-ttu-id="da326-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="da326-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da326-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da326-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da326-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da326-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da326-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da326-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da326-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="da326-116">Not supported.</span></span>|
|<span data-ttu-id="da326-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="da326-117">Application</span></span>|<span data-ttu-id="da326-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da326-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da326-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da326-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
GET /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da326-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="da326-120">Optional query parameters</span></span>
<span data-ttu-id="da326-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="da326-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da326-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="da326-122">Request headers</span></span>
|<span data-ttu-id="da326-123">标头</span><span class="sxs-lookup"><span data-stu-id="da326-123">Header</span></span>|<span data-ttu-id="da326-124">值</span><span class="sxs-lookup"><span data-stu-id="da326-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da326-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="da326-125">Authorization</span></span>|<span data-ttu-id="da326-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da326-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da326-127">接受</span><span class="sxs-lookup"><span data-stu-id="da326-127">Accept</span></span>|<span data-ttu-id="da326-128">application/json</span><span class="sxs-lookup"><span data-stu-id="da326-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da326-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="da326-129">Request body</span></span>
<span data-ttu-id="da326-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="da326-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da326-131">响应</span><span class="sxs-lookup"><span data-stu-id="da326-131">Response</span></span>
<span data-ttu-id="da326-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da326-132">If successful, this method returns a `200 OK` response code and [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da326-133">示例</span><span class="sxs-lookup"><span data-stu-id="da326-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="da326-134">请求</span><span class="sxs-lookup"><span data-stu-id="da326-134">Request</span></span>
<span data-ttu-id="da326-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da326-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="da326-136">响应</span><span class="sxs-lookup"><span data-stu-id="da326-136">Response</span></span>
<span data-ttu-id="da326-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da326-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1238

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
    "id": "823ca4f9-a4f9-823c-f9a4-3c82f9a43c82",
    "valueType": "boolean",
    "displayName": "Display Name value",
    "isTopLevel": true,
    "description": "Description value",
    "placeholderText": "Placeholder Text value",
    "documentationUrl": "https://example.com/documentationUrl/",
    "headerTitle": "Header Title value",
    "headerSubtitle": "Header Subtitle value",
    "keywords": [
      "Keywords value"
    ],
    "constraints": [
      {
        "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
        "supportedTypes": [
          "Supported Types value"
        ]
      }
    ],
    "dependencies": [
      {
        "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
        "definitionId": "Definition Id value",
        "constraints": [
          {
            "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint",
            "supportedTypes": [
              "Supported Types value"
            ]
          }
        ]
      }
    ],
    "propertyDefinitionIds": [
      "Property Definition Ids value"
    ]
  }
}
```




