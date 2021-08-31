---
title: windows10XSCEPCertificateProfile 资源类型
description: WindowsX SCEP 证书配置文件
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da2045765a944b6468555ff2b07338c93d162235
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796472"
---
# <a name="windows10xscepcertificateprofile-resource-type"></a>windows10XSCEPCertificateProfile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

WindowsX SCEP 证书配置文件


继承自 [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windows10XSCEPCertificateProfiles](../api/intune-rapolicy-windows10xscepcertificateprofile-list.md)|[windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) 集合|列出 [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) 对象的属性和关系。|
|[获取 windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-get.md)|[windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|读取 [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) 对象的属性和关系。|
|[创建 windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-create.md)|[windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|创建新的 [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) 对象。|
|[删除 windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-delete.md)|无|删除 [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)。|
|[更新 windows10XSCEPCertificateProfile](../api/intune-rapolicy-windows10xscepcertificateprofile-update.md)|[windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md)|更新 [windows10XSCEPCertificateProfile 对象](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|配置文件标识符 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|version|Int32|配置文件的版本 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|displayName|String|配置文件显示名称继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|description|String|配置文件说明 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|creationDateTime|DateTimeOffset|DateTime 配置文件已创建 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime 配置文件上次修改时间 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|roleScopeTagIds|字符串集合|范围标记 继承自 [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|certificateStore|[certificateStore](../resources/intune-shared-certificatestore.md)|目标存储证书。 可取值为：`user`、`machine`。|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-shared-certificatevalidityperiodscale.md)|证书有效期的缩放。 可取值为：`days`、`months`、`years`。|
|certificateValidityPeriodValue|Int32|证书有效期的值|
|extendedKeyUsages|[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) 集合|扩展密钥使用 (EKU) 设置。|
|hashAlgorithm|[hashAlgorithms](../resources/intune-shared-hashalgorithms.md) 集合|SCEP 哈希算法。|
|keySize|[keySize](../resources/intune-shared-keysize.md)|SCEP 密钥大小。 可取值为：`size1024`、`size2048`、`size4096`。|
|keyStorageProvider|[keyStorageProviderOption](../resources/intune-shared-keystorageprovideroption.md)|Key 存储 Provider (KSP) 。 可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。|
|keyUsage|[keyUsages](../resources/intune-shared-keyusages.md)|SCEP 密钥用法。 可取值为：`keyEncipherment`、`digitalSignature`。|
|renewalThresholdPercentage|Int32|证书续订阈值百分比|
|rootCertificateId|Guid|受信任的根证书 ID|
|scepServerUrls|字符串集合|SCEP 服务器 URL () 。|
|subjectAlternativeNameFormats|[windows10XCustomSubjectAlternativeName](../resources/intune-rapolicy-windows10xcustomsubjectalternativename.md) 集合|自定义 AAD 属性。|
|subjectNameFormatString|String|要与 SubjectNameFormat 一同使用的自定义格式 = Custom。 示例：CN={{EmailAddress}}，E={{EmailAddress}，OU=Enterprise Users，O=Contoso Corporation，L=Redmond，ST=WA，C=US|

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



