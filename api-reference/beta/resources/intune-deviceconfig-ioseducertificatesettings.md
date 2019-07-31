---
title: iosEduCertificateSettings 资源类型
description: 适用于 iOS EDU 的受信任的根和 PFX 证书。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd063ec70dd794ffb151036ea7bbbda090829343
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001251"
---
# <a name="ioseducertificatesettings-resource-type"></a>iosEduCertificateSettings 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

适用于 iOS EDU 的受信任的根和 PFX 证书。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|trustedRootCertificate|Binary|受信任的根证书。|
|certFileName|String|要在 UI 中显示的文件名。|
|certificationAuthority|String|PKCS 证书颁发机构。|
|certificationAuthorityName|String|PKCS 证书颁发机构名称。|
|certificateTemplateName|String|PKCS 证书模板名称。|
|renewalThresholdPercentage|Int32|证书续订阈值百分比。 有效值为1至99|
|certificateValidityPeriodValue|Int32|证书有效期限的值。|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|证书有效期的小数位数。 可取值为：`days`、`months`、`years`。|

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





