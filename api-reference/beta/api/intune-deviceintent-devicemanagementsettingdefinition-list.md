---
title: 列出 deviceManagementSettingDefinitions
description: 列出 deviceManagementSettingDefinition 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d2ca002e7b2055bd1a0b5153b2b7162965e537a1
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635738"
---
# <a name="list-devicemanagementsettingdefinitions"></a><span data-ttu-id="0a3c7-103">列出 deviceManagementSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="0a3c7-103">List deviceManagementSettingDefinitions</span></span>

> <span data-ttu-id="0a3c7-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0a3c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a3c7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0a3c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a3c7-106">列出[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0a3c7-106">List properties and relationships of the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a3c7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0a3c7-107">Prerequisites</span></span>
<span data-ttu-id="0a3c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a3c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a3c7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a3c7-110">Permission type</span></span>|<span data-ttu-id="0a3c7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0a3c7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a3c7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a3c7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0a3c7-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a3c7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0a3c7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a3c7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a3c7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a3c7-115">Not supported.</span></span>|
|<span data-ttu-id="0a3c7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a3c7-116">Application</span></span>|<span data-ttu-id="0a3c7-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a3c7-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a3c7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a3c7-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="0a3c7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a3c7-119">Request headers</span></span>
|<span data-ttu-id="0a3c7-120">标头</span><span class="sxs-lookup"><span data-stu-id="0a3c7-120">Header</span></span>|<span data-ttu-id="0a3c7-121">值</span><span class="sxs-lookup"><span data-stu-id="0a3c7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a3c7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a3c7-122">Authorization</span></span>|<span data-ttu-id="0a3c7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0a3c7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a3c7-124">接受</span><span class="sxs-lookup"><span data-stu-id="0a3c7-124">Accept</span></span>|<span data-ttu-id="0a3c7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0a3c7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a3c7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a3c7-126">Request body</span></span>
<span data-ttu-id="0a3c7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0a3c7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a3c7-128">响应</span><span class="sxs-lookup"><span data-stu-id="0a3c7-128">Response</span></span>
<span data-ttu-id="0a3c7-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="0a3c7-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a3c7-130">示例</span><span class="sxs-lookup"><span data-stu-id="0a3c7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a3c7-131">请求</span><span class="sxs-lookup"><span data-stu-id="0a3c7-131">Request</span></span>
<span data-ttu-id="0a3c7-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0a3c7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="0a3c7-133">响应</span><span class="sxs-lookup"><span data-stu-id="0a3c7-133">Response</span></span>
<span data-ttu-id="0a3c7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0a3c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1142

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





