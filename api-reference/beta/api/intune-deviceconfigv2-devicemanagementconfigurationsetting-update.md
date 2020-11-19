---
title: 更新 deviceManagementConfigurationSetting
description: 更新 deviceManagementConfigurationSetting 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: abbf6165a043d18d965c2dd6343908dc3726e572
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241621"
---
# <a name="update-devicemanagementconfigurationsetting"></a><span data-ttu-id="a4bc7-103">更新 deviceManagementConfigurationSetting</span><span class="sxs-lookup"><span data-stu-id="a4bc7-103">Update deviceManagementConfigurationSetting</span></span>

<span data-ttu-id="a4bc7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4bc7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4bc7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a4bc7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4bc7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4bc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4bc7-107">更新 [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a4bc7-107">Update the properties of a [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4bc7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4bc7-108">Prerequisites</span></span>
<span data-ttu-id="a4bc7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4bc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4bc7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4bc7-111">Permission type</span></span>|<span data-ttu-id="a4bc7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a4bc7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4bc7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4bc7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4bc7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4bc7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4bc7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4bc7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4bc7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4bc7-116">Not supported.</span></span>|
|<span data-ttu-id="a4bc7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4bc7-117">Application</span></span>|<span data-ttu-id="a4bc7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4bc7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4bc7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4bc7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}
```

## <a name="request-headers"></a><span data-ttu-id="a4bc7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4bc7-120">Request headers</span></span>
|<span data-ttu-id="a4bc7-121">标头</span><span class="sxs-lookup"><span data-stu-id="a4bc7-121">Header</span></span>|<span data-ttu-id="a4bc7-122">值</span><span class="sxs-lookup"><span data-stu-id="a4bc7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4bc7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4bc7-123">Authorization</span></span>|<span data-ttu-id="a4bc7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4bc7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4bc7-125">接受</span><span class="sxs-lookup"><span data-stu-id="a4bc7-125">Accept</span></span>|<span data-ttu-id="a4bc7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4bc7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4bc7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4bc7-127">Request body</span></span>
<span data-ttu-id="a4bc7-128">在请求正文中，提供 [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4bc7-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object.</span></span>

<span data-ttu-id="a4bc7-129">下表显示创建 [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a4bc7-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md).</span></span>

|<span data-ttu-id="a4bc7-130">属性</span><span class="sxs-lookup"><span data-stu-id="a4bc7-130">Property</span></span>|<span data-ttu-id="a4bc7-131">类型</span><span class="sxs-lookup"><span data-stu-id="a4bc7-131">Type</span></span>|<span data-ttu-id="a4bc7-132">说明</span><span class="sxs-lookup"><span data-stu-id="a4bc7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4bc7-133">id</span><span class="sxs-lookup"><span data-stu-id="a4bc7-133">id</span></span>|<span data-ttu-id="a4bc7-134">String</span><span class="sxs-lookup"><span data-stu-id="a4bc7-134">String</span></span>|<span data-ttu-id="a4bc7-135">此设置在包含它的策略内的键。</span><span class="sxs-lookup"><span data-stu-id="a4bc7-135">Key of this setting within the policy which contains it.</span></span> <span data-ttu-id="a4bc7-136">自动生成。</span><span class="sxs-lookup"><span data-stu-id="a4bc7-136">Automatically generated.</span></span>|
|<span data-ttu-id="a4bc7-137">settingInstance</span><span class="sxs-lookup"><span data-stu-id="a4bc7-137">settingInstance</span></span>|[<span data-ttu-id="a4bc7-138">deviceManagementConfigurationSettingInstance</span><span class="sxs-lookup"><span data-stu-id="a4bc7-138">deviceManagementConfigurationSettingInstance</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|<span data-ttu-id="a4bc7-139">设置实例</span><span class="sxs-lookup"><span data-stu-id="a4bc7-139">Setting Instance</span></span>|



## <a name="response"></a><span data-ttu-id="a4bc7-140">响应</span><span class="sxs-lookup"><span data-stu-id="a4bc7-140">Response</span></span>
<span data-ttu-id="a4bc7-141">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a4bc7-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSetting](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4bc7-142">示例</span><span class="sxs-lookup"><span data-stu-id="a4bc7-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4bc7-143">请求</span><span class="sxs-lookup"><span data-stu-id="a4bc7-143">Request</span></span>
<span data-ttu-id="a4bc7-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4bc7-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}
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

### <a name="response"></a><span data-ttu-id="a4bc7-145">响应</span><span class="sxs-lookup"><span data-stu-id="a4bc7-145">Response</span></span>
<span data-ttu-id="a4bc7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4bc7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




