---
title: managedDeviceCertificateState 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: f26eb40d371c59a65f58bc87ac5a24d38f47a959
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358385"
---
# <a name="manageddevicecertificatestate-resource-type"></a>managedDeviceCertificateState 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 managedDeviceCertificateStates](../api/intune-deviceconfig-manageddevicecertificatestate-list.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)集合|列出属性和[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象之间的关系。|
|[获取 managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-get.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|读取属性和[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象的关系。|
|[创建 managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-create.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|创建新的[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象。|
|[删除 managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-delete.md)|无|删除[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)。|
|[更新 managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-update.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|更新[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|devicePlatform|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|设备平台。 可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。|
|certificateKeyUsage|[keyUsages](../resources/intune-deviceconfig-keyusages.md)|密钥用法。 可取值为：`keyEncipherment`、`digitalSignature`。|
|certificateValidityPeriodUnits|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|有效期单位。 可取值为：`days`、`months`、`years`。|
|certificateIssuanceState|[certificateIssuanceStates](../resources/intune-deviceconfig-certificateissuancestates.md)|发布状态。 可能的值为： `unknown`， `challengeIssued`， `challengeIssueFailed`， `requestCreationFailed`， `requestSubmitFailed`， `challengeValidationSucceeded`， `challengeValidationFailed`， `issueFailed`， `issuePending`， `issued`， `responseProcessingFailed`， `responsePending`， `enrollmentSucceeded`， `enrollmentNotNeeded`， `revoked`， `removedFromCollection`， `renewVerified`， `installFailed`， `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.|
|certificateKeyStorageProvider|[keyStorageProviderOption](../resources/intune-deviceconfig-keystorageprovideroption.md)|密钥存储提供程序。 可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。|
|certificateSubjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|使用者名称格式。 可取值为：`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId`。|
|certificateSubjectAlternativeNameFormat|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|使用者替代名称格式。 可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。|
|certificateRevokeStatus|[certificateRevocationStatus](../resources/intune-deviceconfig-certificaterevocationstatus.md)|吊销状态。 可取值为：`none`、`pending`、`issued`、`failed`、`revoked`。|
|certificateProfileDisplayName|字符串|证书配置文件的显示名称|
|deviceDisplayName|String|设备显示名称|
|userDisplayName|String|用户显示名称|
|certificateExpirationDateTime|DateTimeOffset|证书到期日期|
|certificateLastIssuanceStateChangedDateTime|DateTimeOffset|最后一个证书颁发状态更改|
|lastCertificateStateChangeDateTime|DateTimeOffset|最后一个证书颁发状态更改|
|certificateIssuer|字符串|颁发者|
|certificateThumbprint|字符串|指纹|
|certificateSerialNumber|字符串|序列号|
|certificateKeyLength|Int32|密钥长度|
|certificateEnhancedKeyUsage|字符串|扩展的密钥用法|
|certificateValidityPeriod|Int32|有效期|
|certificateSubjectNameFormatString|字符串|自定义主题名称格式的使用者名称格式字符串|
|certificateSubjectAlternativeNameFormatString|字符串|自定义格式的使用者替代名称格式字符串|
|certificateIssuanceDateTime|DateTimeOffset|发布日期|
|certificateErrorCode|Int32|错误代码|

## <a name="relationships"></a>Relationships
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





