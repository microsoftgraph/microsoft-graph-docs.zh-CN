---
title: 更新 deviceManagementConfigurationRedirectSettingDefinition
description: 更新 deviceManagementConfigurationRedirectSettingDefinition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f3a7a533451ee077fb449f22041d20072e4b975
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60494353"
---
# <a name="update-devicemanagementconfigurationredirectsettingdefinition"></a>更新 deviceManagementConfigurationRedirectSettingDefinition

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [deviceManagementConfigurationRedirectSettingDefinition 对象](../resources/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition.md) 的属性。

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
PATCH /deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [deviceManagementConfigurationRedirectSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition.md) 对象的 JSON 表示形式。

下表显示创建 [deviceManagementConfigurationRedirectSettingDefinition 时所需的属性](../resources/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition.md)。

|属性|类型|说明|
|:---|:---|:---|
|适用性|[deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|有关哪些设备设置适用于从[deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)继承的详细信息|
|accessTypes|[deviceManagementConfigurationSettingAccessTypes](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|读取/写入访问模式的设置 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。 可取值为：`none`、`add`、`copy`、`delete`、`get`、`replace` 或 `execute`。|
|keywords|String 集合|要搜索上设置的令牌 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|infoUrls|String collection|有关设置详细信息的链接列表，可在 Inherited from [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)找到|
|occurrence|[deviceManagementConfigurationSettingOccurrence](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|指示设置是否必需。继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|baseUri|String|基本云解决方案提供商路径 继承 [自 deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|offsetUri|String|从基本位置偏移 CSP 路径 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|rootDefinitionId|String|根设置定义（如果该设置是子设置）。 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|categoryId|String|指定在指定的配置服务提供程序中配置设置的区域组 (CSP) 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|settingUsage|[deviceManagementConfigurationSettingUsage](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|设置类型，例如，配置和合规性 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。 可取值为：`none`、`configuration`。|
|uxBehavior|[deviceManagementConfigurationControlType](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|设置 UX 中的控件类型表示形式 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。 可取值为：`default`、`dropdown`、`smallTextBox`、`largeTextBox`、`toggle`、`multiheaderGrid` 或 `contextPane`。|
|visibility|[deviceManagementConfigurationSettingVisibility](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|将可见性范围设置为 UX 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)。 可取值为：`none`、`settingsCatalog`、`template`。|
|referredSettingInformationList|[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) 集合|引用的设置信息的列表。 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|id|String|项目的标识符 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|说明|String|项目说明 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|helpText|String|项目的帮助文本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|name|String|项目名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|displayName|String|项目的显示名称 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|version|String|项目版本 继承自 [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)|
|deepLink|String|指向 Intune 控制台中必须管理功能支持的特定位置的深层链接。|
|redirectMessage|String|一条消息，说明单击链接会将用户重定向到支持的页面以管理设置。|
|redirectReason|String|指示将用户重定向到控制台中的备用位置的原因。  例如：WiFi 配置文件在设置目录中不受支持，必须使用模板策略创建。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementConfigurationRedirectSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationredirectsettingdefinition.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1396

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationRedirectSettingDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "Description value",
    "platform": "android",
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
  "visibility": "settingsCatalog",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "deepLink": "Deep Link value",
  "redirectMessage": "Redirect Message value",
  "redirectReason": "Redirect Reason value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1445

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationRedirectSettingDefinition",
  "applicability": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
    "description": "Description value",
    "platform": "android",
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
  "visibility": "settingsCatalog",
  "referredSettingInformationList": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
      "settingDefinitionId": "Setting Definition Id value"
    }
  ],
  "id": "3e6c3eab-3eab-3e6c-ab3e-6c3eab3e6c3e",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value",
  "deepLink": "Deep Link value",
  "redirectMessage": "Redirect Message value",
  "redirectReason": "Redirect Reason value"
}
```



