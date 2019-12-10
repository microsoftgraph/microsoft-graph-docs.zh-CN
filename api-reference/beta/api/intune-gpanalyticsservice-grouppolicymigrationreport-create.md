---
title: 创建 groupPolicyMigrationReport
description: 创建新的 groupPolicyMigrationReport 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b5ba961452e91e2bb5127ddb4f4d85e5db99abd
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943310"
---
# <a name="create-grouppolicymigrationreport"></a>创建 groupPolicyMigrationReport

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 groupPolicyMigrationReport 对象的 JSON 表示形式。

下表显示创建 groupPolicyMigrationReport 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|尚未记录|
|groupPolicyObjectId|Guid|GPO Xml 内容中的组策略对象 GUID|
|displayName|String|来自 GPO Xml 内容的组策略对象的名称|
|ouDistinguishedName|字符串|OU 的可分辨名称。|
|createdDateTime|DateTimeOffset|GroupPolicyMigrationReport 的创建日期和时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改 GroupPolicyMigrationReport 的日期和时间。|
|groupPolicyCreatedDateTime|DateTimeOffset|GroupPolicyMigrationReport 的创建日期和时间。|
|groupPolicyLastModifiedDateTime|DateTimeOffset|上次修改 GroupPolicyMigrationReport 的日期和时间。|
|migrationReadiness|[groupPolicyMigrationReadiness](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|相关联的组策略对象文件的 Intune 覆盖范围。 可取值为：`none`、`partial`、`complete`、`error`、`notApplicable`。|
|targetedInActiveDirectory|Boolean|来自 GPO Xml 内容的 AD 属性中的目标|
|totalSettingsCount|Int32|GPO 文件中的组策略设置总数。|
|supportedSettingsCount|Int32|Intune 支持的组策略设置的数量。|
|supportedSettingsPercent|Int32|Intune 支持的组策略设置的百分比。|



## <a name="response"></a>响应
如果成功，此方法在响应`201 Created`正文中返回响应代码和[groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports
Content-type: application/json
Content-length: 544

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
  "migrationReadiness": "partial",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 2,
  "supportedSettingsCount": 6,
  "supportedSettingsPercent": 8
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 716

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "id": "60663fa8-3fa8-6066-a83f-6660a83f6660",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
  "migrationReadiness": "partial",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 2,
  "supportedSettingsCount": 6,
  "supportedSettingsPercent": 8
}
```





