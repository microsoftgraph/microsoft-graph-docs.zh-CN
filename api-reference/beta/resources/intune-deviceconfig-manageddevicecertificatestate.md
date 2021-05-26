---
title: managedDeviceCertificateState 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 02595eddaa897d415dd7fc992207793420e1102d
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665012"
---
# <a name="manageddevicecertificatestate-resource-type"></a>managedDeviceCertificateState 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedDeviceCertificateStates](../api/intune-deviceconfig-manageddevicecertificatestate-list.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) 集合|列出 [managedDeviceCertificateState 对象的属性和](../resources/intune-deviceconfig-manageddevicecertificatestate.md) 关系。|
|[获取 managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-get.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|读取 [managedDeviceCertificateState 对象的属性和](../resources/intune-deviceconfig-manageddevicecertificatestate.md) 关系。|
|[创建 managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-create.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|创建新的 [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) 对象。|
|[删除 managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-delete.md)|无|删除 [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)。|
|[更新 managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-update.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|更新 [managedDeviceCertificateState 对象](../resources/intune-deviceconfig-manageddevicecertificatestate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|devicePlatform|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|设备平台。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`、`androidAOSP`。|
|certificateKeyUsage|[keyUsages](../resources/intune-shared-keyusages.md)|密钥用法。 可取值为：`keyEncipherment`、`digitalSignature`。|
|certificateValidityPeriodUnits|[certificateValidityPeriodScale](../resources/intune-shared-certificatevalidityperiodscale.md)|有效期单位。 可取值为：`days`、`months`、`years`。|
|certificateIssuanceState|[certificateIssuanceStates](../resources/intune-deviceconfig-certificateissuancestates.md)|颁发状态。 可能的值是 `unknown` `challengeIssued` `challengeIssueFailed` ：、、、、、、、、、、 `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `issueFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending` `enrollmentSucceeded` `enrollmentNotNeeded` `revoked` `removedFromCollection` `renewVerified` `installFailed` `installed` `deleteFailed` `deleted` `renewalRequested` `requested` 。|
|certificateKeyStorageProvider|[keyStorageProviderOption](../resources/intune-shared-keystorageprovideroption.md)|密钥存储提供程序。 可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。|
|certificateSubjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|主题名称格式。 可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。|
|certificateSubjectAlternativeNameFormat|[subjectAlternativeNameType](../resources/intune-shared-subjectalternativenametype.md)|主题备用名称格式。 可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。|
|certificateRevokeStatus|[certificateRevocationStatus](../resources/intune-deviceconfig-certificaterevocationstatus.md)|撤销状态。 可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。|
|certificateProfileDisplayName|String|证书配置文件显示名称|
|deviceDisplayName|String|设备显示名称|
|userDisplayName|String|用户显示名称|
|certificateExpirationDateTime|DateTimeOffset|证书到期日期|
|certificateLastIssuanceStateChangedDateTime|DateTimeOffset|上次证书颁发状态更改|
|lastCertificateStateChangeDateTime|DateTimeOffset|上次证书颁发状态更改|
|certificateIssuer|String|颁发者|
|certificateThumbprint|String|指纹|
|certificateSerialNumber|String|序列号|
|certificateKeyLength|Int32|密钥长度|
|certificateEnhancedKeyUsage|String|扩展密钥用法|
|certificateValidityPeriod|Int32|有效期|
|certificateSubjectNameFormatString|String|自定义主题名称格式的主题名称格式字符串|
|certificateSubjectAlternativeNameFormatString|String|自定义格式的主题替代名称格式字符串|
|certificateIssuanceDateTime|DateTimeOffset|发布日期|
|certificateErrorCode|Int32|错误代码|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceCertificateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "id": "String (identifier)",
  "devicePlatform": "String",
  "certificateKeyUsage": "String",
  "certificateValidityPeriodUnits": "String",
  "certificateIssuanceState": "String",
  "certificateKeyStorageProvider": "String",
  "certificateSubjectNameFormat": "String",
  "certificateSubjectAlternativeNameFormat": "String",
  "certificateRevokeStatus": "String",
  "certificateProfileDisplayName": "String",
  "deviceDisplayName": "String",
  "userDisplayName": "String",
  "certificateExpirationDateTime": "String (timestamp)",
  "certificateLastIssuanceStateChangedDateTime": "String (timestamp)",
  "lastCertificateStateChangeDateTime": "String (timestamp)",
  "certificateIssuer": "String",
  "certificateThumbprint": "String",
  "certificateSerialNumber": "String",
  "certificateKeyLength": 1024,
  "certificateEnhancedKeyUsage": "String",
  "certificateValidityPeriod": 1024,
  "certificateSubjectNameFormatString": "String",
  "certificateSubjectAlternativeNameFormatString": "String",
  "certificateIssuanceDateTime": "String (timestamp)",
  "certificateErrorCode": 1024
}
```




