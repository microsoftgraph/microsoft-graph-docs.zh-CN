---
title: 列出 deviceManagementConfigurationChoiceSettingDefinitions
description: 列出 deviceManagementConfigurationChoiceSettingDefinition 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 32968c321e42a57622ef092c99d4b86885ba0c8b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159722"
---
# <a name="list-devicemanagementconfigurationchoicesettingdefinitions"></a><span data-ttu-id="b57f7-103">列出 deviceManagementConfigurationChoiceSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="b57f7-103">List deviceManagementConfigurationChoiceSettingDefinitions</span></span>

<span data-ttu-id="b57f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b57f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b57f7-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b57f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b57f7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b57f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b57f7-107">列出 [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b57f7-107">List properties and relationships of the [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b57f7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b57f7-108">Prerequisites</span></span>
<span data-ttu-id="b57f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b57f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b57f7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b57f7-111">Permission type</span></span>|<span data-ttu-id="b57f7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b57f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b57f7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b57f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b57f7-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b57f7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b57f7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b57f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b57f7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b57f7-116">Not supported.</span></span>|
|<span data-ttu-id="b57f7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b57f7-117">Application</span></span>|<span data-ttu-id="b57f7-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b57f7-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b57f7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b57f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationSettings
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="b57f7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b57f7-120">Request headers</span></span>
|<span data-ttu-id="b57f7-121">标头</span><span class="sxs-lookup"><span data-stu-id="b57f7-121">Header</span></span>|<span data-ttu-id="b57f7-122">值</span><span class="sxs-lookup"><span data-stu-id="b57f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b57f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b57f7-123">Authorization</span></span>|<span data-ttu-id="b57f7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b57f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b57f7-125">接受</span><span class="sxs-lookup"><span data-stu-id="b57f7-125">Accept</span></span>|<span data-ttu-id="b57f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b57f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b57f7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b57f7-127">Request body</span></span>
<span data-ttu-id="b57f7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b57f7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b57f7-129">响应</span><span class="sxs-lookup"><span data-stu-id="b57f7-129">Response</span></span>
<span data-ttu-id="b57f7-130">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b57f7-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationChoiceSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b57f7-131">示例</span><span class="sxs-lookup"><span data-stu-id="b57f7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b57f7-132">请求</span><span class="sxs-lookup"><span data-stu-id="b57f7-132">Request</span></span>
<span data-ttu-id="b57f7-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b57f7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationSettings
```

### <a name="response"></a><span data-ttu-id="b57f7-134">响应</span><span class="sxs-lookup"><span data-stu-id="b57f7-134">Response</span></span>
<span data-ttu-id="b57f7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b57f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10672

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingDefinition",
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
      "id": "30b2258a-258a-30b2-8a25-b2308a25b230",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value",
      "version": "Version value",
      "options": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinition",
          "optionValue": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValue",
            "children": [
              {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                "settingDefinitionId": "Setting Definition Id value",
                "choiceSettingValue": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                  "value": "Value value",
                  "children": [
                    {
                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                      "settingDefinitionId": "Setting Definition Id value",
                      "choiceSettingValue": {
                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                        "value": "Value value",
                        "children": [
                          {
                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                            "settingDefinitionId": "Setting Definition Id value",
                            "choiceSettingValue": {
                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                              "value": "Value value",
                              "children": [
                                {
                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                  "settingDefinitionId": "Setting Definition Id value",
                                  "choiceSettingValue": {
                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                    "value": "Value value",
                                    "children": [
                                      {
                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                        "settingDefinitionId": "Setting Definition Id value",
                                        "choiceSettingValue": {
                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                          "value": "Value value",
                                          "children": [
                                            {
                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                              "settingDefinitionId": "Setting Definition Id value",
                                              "choiceSettingValue": {
                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                "value": "Value value",
                                                "children": [
                                                  {
                                                    "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                    "settingDefinitionId": "Setting Definition Id value",
                                                    "choiceSettingValue": {
                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                      "value": "Value value",
                                                      "children": [
                                                        {
                                                          "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                          "settingDefinitionId": "Setting Definition Id value",
                                                          "choiceSettingValue": {
                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                            "value": "Value value",
                                                            "children": [
                                                              {
                                                                "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                "settingDefinitionId": "Setting Definition Id value",
                                                                "choiceSettingValue": {
                                                                  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                  "value": "Value value",
                                                                  "children": [
                                                                    {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                      "settingDefinitionId": "Setting Definition Id value",
                                                                      "choiceSettingValue": {
                                                                        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                        "value": "Value value",
                                                                        "children": [
                                                                          {
                                                                            "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                            "settingDefinitionId": "Setting Definition Id value",
                                                                            "choiceSettingValue": {
                                                                              "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValue",
                                                                              "value": "Value value",
                                                                              "children": null
                                                                            }
                                                                          }
                                                                        ]
                                                                      }
                                                                    }
                                                                  ]
                                                                }
                                                              }
                                                            ]
                                                          }
                                                        }
                                                      ]
                                                    }
                                                  }
                                                ]
                                              }
                                            }
                                          ]
                                        }
                                      }
                                    ]
                                  }
                                }
                              ]
                            }
                          }
                        ]
                      }
                    }
                  ]
                }
              }
            ]
          },
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
          "itemId": "Item Id value",
          "description": "Description value",
          "helpText": "Help Text value",
          "name": "Name value",
          "displayName": "Display Name value"
        }
      ],
      "defaultOptionId": "Default Option Id value"
    }
  ]
}
```




