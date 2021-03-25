---
title: 创建 deviceManagementTemplate
description: 创建新的 deviceManagementTemplate 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b7002f0aff39ad54a5cfed4c2930fb72cad3936
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150715"
---
# <a name="create-devicemanagementtemplate"></a>创建 deviceManagementTemplate

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) 对象。

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
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 deviceManagementTemplate 对象的 JSON 表示形式。

下表显示创建 deviceManagementTemplate 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|模板 ID|
|displayName|String|模板的显示名称|
|说明|String|模板的说明|
|versionInfo|String|模板的版本信息|
|isDeprecated|Boolean|模板是否被弃用。 无法从已弃用模板创建意图。|
|intentCount|Int32|从此模板创建的意图数。|
|templateType|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|模板的类型。 可取值为：`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom`、`securityTemplate`、`microsoftEdgeSecurityBaseline`、`microsoftOffice365ProPlusSecurityBaseline`、`deviceCompliance`、`deviceConfigurationForOffice365`、`cloudPC`、`firewallSharedSettings`。|
|platformType|[policyPlatformType](../resources/intune-shared-policyplatformtype.md)|模板的平台。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`all`。|
|templateSubtype|[deviceManagementTemplateSubtype](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|模板的子类型。 可取值为：`none`、`firewall`、`diskEncryption`、`attackSurfaceReduction`、`endpointDetectionReponse`、`accountProtection`、`antivirus`、`firewallSharedAppList`、`firewallSharedIpList`、`firewallSharedPortlist`。|
|publishedDateTime|DateTimeOffset|模板发布时间|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "templateSubtype": "firewall",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 454

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "templateSubtype": "firewall",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```




