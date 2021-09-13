---
title: 更新 groupPolicySettingMapping
description: 更新 groupPolicySettingMapping 对象的属性。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c0b40b3deb68dc406d030c4e2b3579df9215ed97
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59124810"
---
# <a name="update-grouppolicysettingmapping"></a>更新 groupPolicySettingMapping

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [groupPolicySettingMapping 对象](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 的属性。

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
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [groupPolicySettingMapping 对象的](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) JSON 表示形式。

下表显示创建 [groupPolicySettingMapping 时所需的属性](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|parentId|String|组策略设置的父 ID。|
|childIdList|字符串集合|组策略设置的子 ID 列表。|
|settingName|String|此组策略设置的名称。|
|settingValue|String|此组策略设置的值。|
|settingValueType|String|此组策略设置的值类型。|
|settingDisplayName|String|此显示名称策略设置的成员。|
|settingDisplayValue|String|此组策略设置的显示值。|
|settingDisplayValueType|String|此组策略设置的显示值类型。|
|settingValueDisplayUnits|String|此组策略设置值的显示单位|
|settingCategory|String|组策略设置位于的类别。|
|mdmCspName|String|此组策略设置映射到的云解决方案提供商名称。|
|mdmSettingUri|String|此组策略设置映射到的 MDM CSP URI。|
|mdmMinimumOSVersion|Int32|此 mdm 设置支持的最低操作系统版本。|
|settingType|[groupPolicySettingType](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|设置类型 (安全或 admx) 组策略的一部分。 可取值为：`unknown`、`policy`、`account`、`securityOptions`、`userRightsAssignment`、`auditSetting` 或 `windowsFirewallSettings`。|
|isMdmSupported|Boolean|指示 Intune 是否支持该设置|
|mdmSupportedState|[mdmSupportedState](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|指示设置在 Mdm 中是否受支持。 可取值为：`unknown`、`supported`、`unsupported`、`deprecated`。|
|settingScope|[groupPolicySettingScope](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|设置的范围。 可取值为：`unknown`、`device`、`user`。|
|intuneSettingUriList|字符串集合|此组策略设置映射到的 Intune 设置 URI 列表|
|intuneSettingDefinitionId|String|Intune 设置定义 ID|
|admxSettingDefinitionId|String|Admx 组策略 ID|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
Content-type: application/json
Content-length: 1023

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
  ],
  "intuneSettingDefinitionId": "Intune Setting Definition Id value",
  "admxSettingDefinitionId": "Admx Setting Definition Id value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1072

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
  ],
  "intuneSettingDefinitionId": "Intune Setting Definition Id value",
  "admxSettingDefinitionId": "Admx Setting Definition Id value"
}
```



