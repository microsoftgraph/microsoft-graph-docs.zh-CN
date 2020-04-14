---
title: 更新 securityBaselineTemplate
description: 更新 securityBaselineTemplate 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5d20b7f5b27f130393996573a27b9e00b42a2f0d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43427095"
---
# <a name="update-securitybaselinetemplate"></a>更新 securityBaselineTemplate

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
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
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象的 JSON 表示形式。

下表显示创建[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板 ID|
|displayName|String|从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承的模板的显示名称|
|description|String|模板的说明继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|versionInfo|String|模板的版本信息继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|isDeprecated|Boolean|模板已弃用或不已弃用。 无法从已弃用的模板创建意向。 继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|intentCount|Int32|从此模板创建的意向数。 继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|templateType|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|模板的类型。 继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。 可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`、`securityTemplate`、`microsoftEdgeSecurityBaseline`、`microsoftOffice365ProPlusSecurityBaseline`、`deviceCompliance`。|
|platformType|[policyPlatformType](../resources/intune-shared-policyplatformtype.md)|模板的平台。 继承自[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`all`。|
|publishedDateTime|DateTimeOffset|从[DeviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)继承发布模板时|



## <a name="response"></a>响应
如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 420

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```



