---
title: iosEduCertificateSettings 资源类型
description: iOS EDU 的受信任的根证书和 PFX 证书。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4d97070415d65f8193bcf69bbcf771cd59684ff4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59047147"
---
# <a name="ioseducertificatesettings-resource-type"></a>iosEduCertificateSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

iOS EDU 的受信任的根证书和 PFX 证书。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|trustedRootCertificate|二进制|受信任的根证书。|
|certFileName|String|要显示在 UI 中的文件名。|
|certificationAuthority|String|PKCS 证书颁发机构。|
|certificationAuthorityName|String|PKCS 证书颁发机构名称。|
|certificateTemplateName|String|PKCS 证书模板名称。|
|renewalThresholdPercentage|Int32|证书续订阈值百分比。 有效值为 1 到 99|
|certificateValidityPeriodValue|Int32|证书有效期的值。|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-shared-certificatevalidityperiodscale.md)|证书有效期的缩放。 可取值为：`days`、`months`、`years`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosEduCertificateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduCertificateSettings",
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "renewalThresholdPercentage": 1024,
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String"
}
```



