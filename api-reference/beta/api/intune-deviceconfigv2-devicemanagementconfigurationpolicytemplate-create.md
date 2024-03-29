---
title: 创建 deviceManagementConfigurationPolicyTemplate
description: 创建新的 deviceManagementConfigurationPolicyTemplate 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ae19e6f29b97bfd25eb7d3ba553ef541dac4501
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66667304"
---
# <a name="create-devicemanagementconfigurationpolicytemplate"></a>创建 deviceManagementConfigurationPolicyTemplate

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicyTemplates
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，为 deviceManagementConfigurationPolicyTemplate 对象提供 JSON 表示形式。

下表显示了创建 deviceManagementConfigurationPolicyTemplate 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|模板文档的键，由 BaseId 和 Version 组成。 自动生成。|
|baseId|String|模板基本标识符|
|version|Int32|模板版本。 有效值 1 到2147483647。 此属性是只读的。|
|displayName|String|模板显示名称|
|说明|字符串|模板说明|
|displayVersion|字符串|模板版本说明|
|lifecycleState|[deviceManagementTemplateLifecycleState](../resources/intune-deviceconfigv2-devicemanagementtemplatelifecyclestate.md)|指示模板的当前生命周期状态。 可取值为：`invalid`、`draft`、`active`、`superseded`、`deprecated`、`retired`。|
|平台|[deviceManagementConfigurationPlatforms](../resources/intune-shared-devicemanagementconfigurationplatforms.md)|此模板的平台。 可取值为：`none`、`android`、`iOS`、`macOS`、`windows10X`、`windows10`、`linux`、`unknownFutureValue`。|
|技术|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|此模板的技术。 可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`appleRemoteManagement`、`microsoftSense`、`exchangeOnline`、`linuxMdm`、`enrollment`、`unknownFutureValue`。|
|templateFamily|[deviceManagementConfigurationTemplateFamily](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|此模板的 TemplateFamily。 可取值为：`none`、`endpointSecurityAntivirus`、`endpointSecurityDiskEncryption`、`endpointSecurityFirewall`、`endpointSecurityEndpointDetectionAndResponse`、`endpointSecurityAttackSurfaceReduction`、`endpointSecurityAccountProtection`、`endpointSecurityApplicationControl`、`baseline`。|
|allowUnmanagedSettings|Boolean|允许非托管设置模板|
|settingTemplateCount|Int32|设置模板的数目。 要2147483647的有效值 0。 此属性是只读的。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceManagementConfigurationPolicyTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicytemplate.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicyTemplates
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
  "baseId": "Base Id value",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "displayVersion": "Display Version value",
  "lifecycleState": "draft",
  "platforms": "android",
  "technologies": "mdm",
  "templateFamily": "endpointSecurityAntivirus",
  "allowUnmanagedSettings": true,
  "settingTemplateCount": 4
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplate",
  "id": "424ddb9a-db9a-424d-9adb-4d429adb4d42",
  "baseId": "Base Id value",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "displayVersion": "Display Version value",
  "lifecycleState": "draft",
  "platforms": "android",
  "technologies": "mdm",
  "templateFamily": "endpointSecurityAntivirus",
  "allowUnmanagedSettings": true,
  "settingTemplateCount": 4
}
```




