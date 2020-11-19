---
title: windows10XSCEPCertificateProfile 资源类型
description: Windows X SCEP 证书配置文件
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8e242140c1a27ed299849158df67c18444ab362
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301562"
---
# <a name="windows10xscepcertificateprofile-resource-type"></a>windows10XSCEPCertificateProfile 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows X SCEP 证书配置文件


继承自 [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windows10XSCEPCertificateProfiles](../api/intune-rapolicy-windows10xscepcertificateprofile-list.md)|[windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) 集合|列出 [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) 对象的属性和关系。|
|[获取 windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-get.md)|[windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|读取 [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) 对象的属性和关系。|
|[创建 windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-create.md)|[windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|创建新的 [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) 对象。|
|[删除 windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-delete.md)|无|删除 [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)。|
|[更新 windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-update.md)|[windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|更新 [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件标识符|
|version|Int32|继承自[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)的配置文件的版本|
|displayName|字符串|从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件显示名称|
|description|字符串|从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的配置文件说明|
|creationDateTime|DateTimeOffset|已创建从[DeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)继承的 DateTime 配置文件|
|lastModifiedDateTime|DateTimeOffset|上次修改的日期时间配置文件继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|roleScopeTagIds|String 集合|继承自[deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)的范围标记|
|certificateStore|[certificateStore](../resources/intune-shared-certificatestore.md)|目标存储证书。 可取值为：`user`、`machine`。|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-shared-certificatevalidityperiodscale.md)|证书有效期的小数位数。 可取值为：`days`、`months`、`years`。|
|certificateValidityPeriodValue|Int32|证书有效期限的值|
|extendedKeyUsages|[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) 集合| (EKU) 设置的扩展密钥用法。|
|hashAlgorithm|[hashAlgorithms](../resources/intune-shared-hashalgorithms.md) 集合|SCEP 哈希算法。|
|keySize|[keySize](../resources/intune-shared-keysize.md)|SCEP 密钥大小。 可取值为：`size1024`、`size2048`、`size4096`。|
|keyStorageProvider|[keyStorageProviderOption](../resources/intune-shared-keystorageprovideroption.md)|密钥存储提供程序 (KSP) 。 可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。|
|keyUsage|[keyUsages](../resources/intune-shared-keyusages.md)|SCEP 密钥用法。 可取值为：`keyEncipherment`、`digitalSignature`。|
|renewalThresholdPercentage|Int32|证书续订阈值百分比|
|rootCertificateId|Guid|受信任的根证书 ID|
|scepServerUrls|String 集合|SCEP (s) 的服务器 Url。|
|subjectAlternativeNameFormats|[windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md) 集合|自定义 AAD 属性。|
|subjectNameFormatString|字符串|要与 SubjectNameFormat = Custom 一起使用的自定义格式。 示例： CN = {{EmailAddress}}，E = {{EmailAddress}}，OU = 企业用户，O = Contoso Corporation，L = Redmond，ST = WA，C = US|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10XSCEPCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XSCEPCertificateProfile",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "certificateStore": "String",
  "certificateValidityPeriodScale": "String",
  "certificateValidityPeriodValue": 1024,
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "String",
      "objectIdentifier": "String"
    }
  ],
  "hashAlgorithm": [
    "String"
  ],
  "keySize": "String",
  "keyStorageProvider": "String",
  "keyUsage": "String",
  "renewalThresholdPercentage": 1024,
  "rootCertificateId": "Guid",
  "scepServerUrls": [
    "String"
  ],
  "subjectAlternativeNameFormats": [
    {
      "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName",
      "sanType": "String",
      "name": "String"
    }
  ],
  "subjectNameFormatString": "String"
}
```




