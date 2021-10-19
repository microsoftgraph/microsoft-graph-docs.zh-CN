---
title: 创建 deviceManagementConfigurationCategory
description: 创建新的 deviceManagementConfigurationCategory 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 43e5ac410af72a26c02bc9b986226812eadec545
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60487161"
---
# <a name="create-devicemanagementconfigurationcategory"></a>创建 deviceManagementConfigurationCategory

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 对象。

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
POST /deviceManagement/configurationCategories
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 deviceManagementConfigurationCategory 对象的 JSON 表示形式。

下表显示创建 deviceManagementConfigurationCategory 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|项的标识符|
|说明|String|项目说明|
|helpText|String|项目的帮助文本|
|name|String|项目名称|
|displayName|String|项目的显示名称|
|平台|[deviceManagementConfigurationPlatforms](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|平台类型，类别中的设置具有。 可取值为：`none`、`android`、`iOS`、`macOS`、`windows10X`、`windows10`。|
|technologies|[deviceManagementConfigurationTechnologies](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|技术类型，类别中的设置具有。 可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`、`microsoftSense`、`exchangeOnline`、`linuxMdm`、`unknownFutureValue`。|
|settingUsage|[deviceManagementConfigurationSettingUsage](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|指示类别包含用于合规性或配置的设置。 可取值为：`none`、`configuration`。|
|parentCategoryId|String|类别的父 ID。|
|rootCategoryId|String|类别的根 ID。|
|childCategoryIds|String collection|类别的子 ID 列表。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementConfigurationCategory](../resources/intune-deviceconfigv2-devicemanagementconfigurationcategory.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationCategories
Content-type: application/json
Content-length: 467

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "android",
  "technologies": "mdm",
  "settingUsage": "configuration",
  "parentCategoryId": "Parent Category Id value",
  "rootCategoryId": "Root Category Id value",
  "childCategoryIds": [
    "Child Category Ids value"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 516

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "id": "cff34dd2-4dd2-cff3-d24d-f3cfd24df3cf",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "platforms": "android",
  "technologies": "mdm",
  "settingUsage": "configuration",
  "parentCategoryId": "Parent Category Id value",
  "rootCategoryId": "Root Category Id value",
  "childCategoryIds": [
    "Child Category Ids value"
  ]
}
```



