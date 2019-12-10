---
title: 更新 groupPolicySettingMapping
description: 更新 groupPolicySettingMapping 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 68d5b1f3c48229677889f47c8adfff73e5821e7b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943240"
---
# <a name="update-grouppolicysettingmapping"></a>更新 groupPolicySettingMapping

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象的属性。

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
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象的 JSON 表示形式。

下表显示创建[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|尚未记录|
|parentId|字符串|组策略设置的父 Id。|
|childIdList|String collection|组策略设置的子 Id 列表。|
|settingName|String|此组策略设置的名称。|
|settingValue|字符串|此组策略设置的值。|
|settingValueType|字符串|此组策略设置的值类型。|
|settingDisplayName|字符串|此组策略设置的显示名称。|
|settingDisplayValue|字符串|此组策略设置的显示值。|
|settingDisplayValueType|字符串|此组策略设置的显示值类型。|
|settingValueDisplayUnits|字符串|此组策略设置值的显示单位|
|settingCategory|字符串|组策略设置所属的类别。|
|mdmCspName|字符串|将此组策略设置映射到的 CSP 名称。|
|mdmSettingUri|字符串|将此组策略设置映射到的 MDM CSP URI。|
|mdmMinimumOSVersion|Int32|此 mdm 设置支持的最低 OS 版本。|
|settingType|[groupPolicySettingType](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|组策略的设置类型（安全性或 admx）。 可取值为：`unknown`、`policy`、`account`、`securityOptions`、`userRightsAssignment`、`auditSetting` 或 `windowsFirewallSettings`。|
|isMdmSupported|Boolean|指示此设置是否由 Intune 支持|
|mdmSupportedState|[mdmSupportedState](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|指示是否支持 Mdm 中的设置。 可取值为：`unknown`、`supported`、`unsupported`、`deprecated`。|
|settingScope|[groupPolicySettingScope](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|设置的范围。 可取值为：`unknown`、`device`、`user`。|
|intuneSettingUriList|String collection|此组策略设置映射到的 Intune 设置 Uri 列表|



## <a name="response"></a>响应
如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
Content-type: application/json
Content-length: 887

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "policy",
  "isMdmSupported": true,
  "mdmSupportedState": "supported",
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 936

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "8fa04560-4560-8fa0-6045-a08f6045a08f",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "policy",
  "isMdmSupported": true,
  "mdmSupportedState": "supported",
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ]
}
```





