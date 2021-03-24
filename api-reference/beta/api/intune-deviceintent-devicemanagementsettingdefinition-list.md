---
title: 列出 deviceManagementSettingDefinitions
description: 列出 deviceManagementSettingDefinition 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 991ced33cc07d03dd6921b4034647918a6838331
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146578"
---
# <a name="list-devicemanagementsettingdefinitions"></a><span data-ttu-id="697fa-103">列出 deviceManagementSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="697fa-103">List deviceManagementSettingDefinitions</span></span>

<span data-ttu-id="697fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="697fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="697fa-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="697fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="697fa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="697fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="697fa-107">列出 [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="697fa-107">List properties and relationships of the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="697fa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="697fa-108">Prerequisites</span></span>
<span data-ttu-id="697fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="697fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="697fa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="697fa-111">Permission type</span></span>|<span data-ttu-id="697fa-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="697fa-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="697fa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="697fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="697fa-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="697fa-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="697fa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="697fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="697fa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="697fa-116">Not supported.</span></span>|
|<span data-ttu-id="697fa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="697fa-117">Application</span></span>|<span data-ttu-id="697fa-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="697fa-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="697fa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="697fa-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="697fa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="697fa-120">Request headers</span></span>
|<span data-ttu-id="697fa-121">标头</span><span class="sxs-lookup"><span data-stu-id="697fa-121">Header</span></span>|<span data-ttu-id="697fa-122">值</span><span class="sxs-lookup"><span data-stu-id="697fa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="697fa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="697fa-123">Authorization</span></span>|<span data-ttu-id="697fa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="697fa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="697fa-125">接受</span><span class="sxs-lookup"><span data-stu-id="697fa-125">Accept</span></span>|<span data-ttu-id="697fa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="697fa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="697fa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="697fa-127">Request body</span></span>
<span data-ttu-id="697fa-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="697fa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="697fa-129">响应</span><span class="sxs-lookup"><span data-stu-id="697fa-129">Response</span></span>
<span data-ttu-id="697fa-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="697fa-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="697fa-131">示例</span><span class="sxs-lookup"><span data-stu-id="697fa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="697fa-132">请求</span><span class="sxs-lookup"><span data-stu-id="697fa-132">Request</span></span>
<span data-ttu-id="697fa-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="697fa-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="697fa-134">响应</span><span class="sxs-lookup"><span data-stu-id="697fa-134">Response</span></span>
<span data-ttu-id="697fa-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="697fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1236

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
      "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
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
      ]
    }
  ]
}
```




