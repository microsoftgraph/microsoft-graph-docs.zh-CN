---
title: 创建 deviceManagementReusablePolicySetting
description: 创建新的 deviceManagementReusablePolicySetting 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 146dfbe24f2380f639ec7715c9ab7cb3278191da
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868733"
---
# <a name="create-devicemanagementreusablepolicysetting"></a><span data-ttu-id="29589-103">创建 deviceManagementReusablePolicySetting</span><span class="sxs-lookup"><span data-stu-id="29589-103">Create deviceManagementReusablePolicySetting</span></span>

<span data-ttu-id="29589-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29589-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29589-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="29589-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29589-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29589-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29589-107">创建新的 [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29589-107">Create a new [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29589-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="29589-108">Prerequisites</span></span>
<span data-ttu-id="29589-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29589-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29589-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="29589-111">Permission type</span></span>|<span data-ttu-id="29589-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="29589-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29589-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29589-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29589-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29589-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="29589-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29589-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29589-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="29589-116">Not supported.</span></span>|
|<span data-ttu-id="29589-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="29589-117">Application</span></span>|<span data-ttu-id="29589-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29589-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29589-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29589-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reusablePolicySettings
```

## <a name="request-headers"></a><span data-ttu-id="29589-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="29589-120">Request headers</span></span>
|<span data-ttu-id="29589-121">标头</span><span class="sxs-lookup"><span data-stu-id="29589-121">Header</span></span>|<span data-ttu-id="29589-122">值</span><span class="sxs-lookup"><span data-stu-id="29589-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29589-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="29589-123">Authorization</span></span>|<span data-ttu-id="29589-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="29589-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29589-125">接受</span><span class="sxs-lookup"><span data-stu-id="29589-125">Accept</span></span>|<span data-ttu-id="29589-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29589-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29589-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="29589-127">Request body</span></span>
<span data-ttu-id="29589-128">在请求正文中，提供 deviceManagementReusablePolicySetting 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29589-128">In the request body, supply a JSON representation for the deviceManagementReusablePolicySetting object.</span></span>

<span data-ttu-id="29589-129">下表显示创建 deviceManagementReusablePolicySetting 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="29589-129">The following table shows the properties that are required when you create the deviceManagementReusablePolicySetting.</span></span>

|<span data-ttu-id="29589-130">属性</span><span class="sxs-lookup"><span data-stu-id="29589-130">Property</span></span>|<span data-ttu-id="29589-131">类型</span><span class="sxs-lookup"><span data-stu-id="29589-131">Type</span></span>|<span data-ttu-id="29589-132">说明</span><span class="sxs-lookup"><span data-stu-id="29589-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29589-133">id</span><span class="sxs-lookup"><span data-stu-id="29589-133">id</span></span>|<span data-ttu-id="29589-134">String</span><span class="sxs-lookup"><span data-stu-id="29589-134">String</span></span>|<span data-ttu-id="29589-135">系统生成的可重用设置 ID。</span><span class="sxs-lookup"><span data-stu-id="29589-135">system generated reusable setting id.</span></span>|
|<span data-ttu-id="29589-136">displayName</span><span class="sxs-lookup"><span data-stu-id="29589-136">displayName</span></span>|<span data-ttu-id="29589-137">String</span><span class="sxs-lookup"><span data-stu-id="29589-137">String</span></span>|<span data-ttu-id="29589-138">由显示名称的可重用设置。</span><span class="sxs-lookup"><span data-stu-id="29589-138">reusable setting display name supplied by user.</span></span>|
|<span data-ttu-id="29589-139">说明</span><span class="sxs-lookup"><span data-stu-id="29589-139">description</span></span>|<span data-ttu-id="29589-140">String</span><span class="sxs-lookup"><span data-stu-id="29589-140">String</span></span>|<span data-ttu-id="29589-141">由用户提供的可重用设置说明。</span><span class="sxs-lookup"><span data-stu-id="29589-141">reusable setting description supplied by user.</span></span>|
|<span data-ttu-id="29589-142">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="29589-142">settingDefinitionId</span></span>|<span data-ttu-id="29589-143">String</span><span class="sxs-lookup"><span data-stu-id="29589-143">String</span></span>|<span data-ttu-id="29589-144">与此可重用设置关联的设置定义 ID。</span><span class="sxs-lookup"><span data-stu-id="29589-144">setting definition id associated with this reusable setting.</span></span>|
|<span data-ttu-id="29589-145">settingInstance</span><span class="sxs-lookup"><span data-stu-id="29589-145">settingInstance</span></span>|[<span data-ttu-id="29589-146">deviceManagementConfigurationSettingInstance</span><span class="sxs-lookup"><span data-stu-id="29589-146">deviceManagementConfigurationSettingInstance</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)|<span data-ttu-id="29589-147">可重用的设置配置实例</span><span class="sxs-lookup"><span data-stu-id="29589-147">reusable setting configuration instance</span></span>|
|<span data-ttu-id="29589-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29589-148">createdDateTime</span></span>|<span data-ttu-id="29589-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29589-149">DateTimeOffset</span></span>|<span data-ttu-id="29589-150">可重用设置创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="29589-150">reusable setting creation date and time.</span></span> <span data-ttu-id="29589-151">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="29589-151">This property is read-only.</span></span>|
|<span data-ttu-id="29589-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29589-152">lastModifiedDateTime</span></span>|<span data-ttu-id="29589-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29589-153">DateTimeOffset</span></span>|<span data-ttu-id="29589-154">上次修改可重用设置的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="29589-154">date and time when reusable setting was last modified.</span></span> <span data-ttu-id="29589-155">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="29589-155">This property is read-only.</span></span>|
|<span data-ttu-id="29589-156">version</span><span class="sxs-lookup"><span data-stu-id="29589-156">version</span></span>|<span data-ttu-id="29589-157">Int32</span><span class="sxs-lookup"><span data-stu-id="29589-157">Int32</span></span>|<span data-ttu-id="29589-158">可重复使用设置的版本号。</span><span class="sxs-lookup"><span data-stu-id="29589-158">version number for reusable setting.</span></span> <span data-ttu-id="29589-159">有效值为 0 到 2147483647。</span><span class="sxs-lookup"><span data-stu-id="29589-159">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="29589-160">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="29589-160">This property is read-only.</span></span>|
|<span data-ttu-id="29589-161">referencingConfigurationPolicyCount</span><span class="sxs-lookup"><span data-stu-id="29589-161">referencingConfigurationPolicyCount</span></span>|<span data-ttu-id="29589-162">Int32</span><span class="sxs-lookup"><span data-stu-id="29589-162">Int32</span></span>|<span data-ttu-id="29589-163">引用当前可重用设置的配置策略计数。</span><span class="sxs-lookup"><span data-stu-id="29589-163">count of configuration policies referencing the current reusable setting.</span></span> <span data-ttu-id="29589-164">有效值为 0 到 2147483647。</span><span class="sxs-lookup"><span data-stu-id="29589-164">Valid values 0 to 2147483647.</span></span> <span data-ttu-id="29589-165">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="29589-165">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="29589-166">响应</span><span class="sxs-lookup"><span data-stu-id="29589-166">Response</span></span>
<span data-ttu-id="29589-167">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29589-167">If successful, this method returns a `201 Created` response code and a [deviceManagementReusablePolicySetting](../resources/intune-deviceconfigv2-devicemanagementreusablepolicysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29589-168">示例</span><span class="sxs-lookup"><span data-stu-id="29589-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="29589-169">请求</span><span class="sxs-lookup"><span data-stu-id="29589-169">Request</span></span>
<span data-ttu-id="29589-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29589-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reusablePolicySettings
Content-type: application/json
Content-length: 7888

{
  "@odata.type": "#microsoft.graph.deviceManagementReusablePolicySetting",
  "displayName": "Display Name value",
  "description": "Description value",
  "settingDefinitionId": "Setting Definition Id value",
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
  },
  "version": 7,
  "referencingConfigurationPolicyCount": 3
}
```

### <a name="response"></a><span data-ttu-id="29589-171">响应</span><span class="sxs-lookup"><span data-stu-id="29589-171">Response</span></span>
<span data-ttu-id="29589-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29589-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 8060

{
  "@odata.type": "#microsoft.graph.deviceManagementReusablePolicySetting",
  "id": "7a4f9bd7-9bd7-7a4f-d79b-4f7ad79b4f7a",
  "displayName": "Display Name value",
  "description": "Description value",
  "settingDefinitionId": "Setting Definition Id value",
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
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "referencingConfigurationPolicyCount": 3
}
```




