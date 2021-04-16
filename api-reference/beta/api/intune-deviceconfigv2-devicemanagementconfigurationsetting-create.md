---
title: 创建 deviceManagementConfigurationSetting
description: 创建新的 deviceManagementConfigurationSetting 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 664b1e9876dc069a047d5619ad8bfb49708102fa
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864009"
---
# <a name="create-devicemanagementconfigurationsetting"></a><span data-ttu-id="03af5-103">创建 deviceManagementConfigurationSetting</span><span class="sxs-lookup"><span data-stu-id="03af5-103">Create deviceManagementConfigurationSetting</span></span>

<span data-ttu-id="03af5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03af5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03af5-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03af5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03af5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03af5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03af5-107">创建新的 [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03af5-107">Create a new [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03af5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="03af5-108">Prerequisites</span></span>
<span data-ttu-id="03af5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03af5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03af5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="03af5-111">Permission type</span></span>|<span data-ttu-id="03af5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03af5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03af5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03af5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03af5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03af5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03af5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03af5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03af5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="03af5-116">Not supported.</span></span>|
|<span data-ttu-id="03af5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="03af5-117">Application</span></span>|<span data-ttu-id="03af5-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03af5-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03af5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03af5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings
```

## <a name="request-headers"></a><span data-ttu-id="03af5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="03af5-120">Request headers</span></span>
|<span data-ttu-id="03af5-121">标头</span><span class="sxs-lookup"><span data-stu-id="03af5-121">Header</span></span>|<span data-ttu-id="03af5-122">值</span><span class="sxs-lookup"><span data-stu-id="03af5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03af5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03af5-123">Authorization</span></span>|<span data-ttu-id="03af5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="03af5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03af5-125">接受</span><span class="sxs-lookup"><span data-stu-id="03af5-125">Accept</span></span>|<span data-ttu-id="03af5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03af5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03af5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="03af5-127">Request body</span></span>
<span data-ttu-id="03af5-128">在请求正文中，提供 deviceManagementConfigurationSetting 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03af5-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSetting object.</span></span>

<span data-ttu-id="03af5-129">下表显示创建 deviceManagementConfigurationSetting 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="03af5-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSetting.</span></span>

|<span data-ttu-id="03af5-130">属性</span><span class="sxs-lookup"><span data-stu-id="03af5-130">Property</span></span>|<span data-ttu-id="03af5-131">类型</span><span class="sxs-lookup"><span data-stu-id="03af5-131">Type</span></span>|<span data-ttu-id="03af5-132">说明</span><span class="sxs-lookup"><span data-stu-id="03af5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03af5-133">id</span><span class="sxs-lookup"><span data-stu-id="03af5-133">id</span></span>|<span data-ttu-id="03af5-134">String</span><span class="sxs-lookup"><span data-stu-id="03af5-134">String</span></span>|<span data-ttu-id="03af5-135">包含此设置的策略中的此设置的键。</span><span class="sxs-lookup"><span data-stu-id="03af5-135">Key of this setting within the policy which contains it.</span></span> <span data-ttu-id="03af5-136">自动生成。</span><span class="sxs-lookup"><span data-stu-id="03af5-136">Automatically generated.</span></span>|
|<span data-ttu-id="03af5-137">settingInstance</span><span class="sxs-lookup"><span data-stu-id="03af5-137">settingInstance</span></span>|[<span data-ttu-id="03af5-138">deviceManagementConfigurationSettingInstance</span><span class="sxs-lookup"><span data-stu-id="03af5-138">deviceManagementConfigurationSettingInstance</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|<span data-ttu-id="03af5-139">设置实例</span><span class="sxs-lookup"><span data-stu-id="03af5-139">Setting Instance</span></span>|



## <a name="response"></a><span data-ttu-id="03af5-140">响应</span><span class="sxs-lookup"><span data-stu-id="03af5-140">Response</span></span>
<span data-ttu-id="03af5-141">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03af5-141">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03af5-142">示例</span><span class="sxs-lookup"><span data-stu-id="03af5-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="03af5-143">请求</span><span class="sxs-lookup"><span data-stu-id="03af5-143">Request</span></span>
<span data-ttu-id="03af5-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03af5-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings
Content-type: application/json
Content-length: 7689

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSetting",
  "settingInstance": {
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
                                                                  "children": [
                                                                    {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                      "settingDefinitionId": null,
                                                                      "choiceSettingValue": null
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
    }
  }
}
```

### <a name="response"></a><span data-ttu-id="03af5-145">响应</span><span class="sxs-lookup"><span data-stu-id="03af5-145">Response</span></span>
<span data-ttu-id="03af5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03af5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7738

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSetting",
  "id": "9acf977e-977e-9acf-7e97-cf9a7e97cf9a",
  "settingInstance": {
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
                                                                  "children": [
                                                                    {
                                                                      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingInstance",
                                                                      "settingDefinitionId": null,
                                                                      "choiceSettingValue": null
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
    }
  }
}
```




