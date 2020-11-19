---
title: 列出 deviceManagementAbstractComplexSettingDefinitions
description: 列出 deviceManagementAbstractComplexSettingDefinition 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d033926433c55a05071a300606a3e453a4b66394
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49290509"
---
# <a name="list-devicemanagementabstractcomplexsettingdefinitions"></a><span data-ttu-id="8c1de-103">列出 deviceManagementAbstractComplexSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="8c1de-103">List deviceManagementAbstractComplexSettingDefinitions</span></span>

<span data-ttu-id="8c1de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c1de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c1de-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c1de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c1de-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c1de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c1de-107">列出 [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8c1de-107">List properties and relationships of the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c1de-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8c1de-108">Prerequisites</span></span>
<span data-ttu-id="8c1de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c1de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c1de-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c1de-111">Permission type</span></span>|<span data-ttu-id="8c1de-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8c1de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c1de-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c1de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c1de-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c1de-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8c1de-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c1de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c1de-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c1de-116">Not supported.</span></span>|
|<span data-ttu-id="8c1de-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c1de-117">Application</span></span>|<span data-ttu-id="8c1de-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c1de-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c1de-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c1de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/settingDefinitions
GET /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="8c1de-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c1de-120">Request headers</span></span>
|<span data-ttu-id="8c1de-121">标头</span><span class="sxs-lookup"><span data-stu-id="8c1de-121">Header</span></span>|<span data-ttu-id="8c1de-122">值</span><span class="sxs-lookup"><span data-stu-id="8c1de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c1de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c1de-123">Authorization</span></span>|<span data-ttu-id="8c1de-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8c1de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c1de-125">接受</span><span class="sxs-lookup"><span data-stu-id="8c1de-125">Accept</span></span>|<span data-ttu-id="8c1de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c1de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c1de-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c1de-127">Request body</span></span>
<span data-ttu-id="8c1de-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8c1de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c1de-129">响应</span><span class="sxs-lookup"><span data-stu-id="8c1de-129">Response</span></span>
<span data-ttu-id="8c1de-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c1de-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c1de-131">示例</span><span class="sxs-lookup"><span data-stu-id="8c1de-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c1de-132">请求</span><span class="sxs-lookup"><span data-stu-id="8c1de-132">Request</span></span>
<span data-ttu-id="8c1de-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c1de-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="8c1de-134">响应</span><span class="sxs-lookup"><span data-stu-id="8c1de-134">Response</span></span>
<span data-ttu-id="8c1de-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c1de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1322

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
      "id": "1b703309-3309-1b70-0933-701b0933701b",
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
      "implementations": [
        "Implementations value"
      ]
    }
  ]
}
```




