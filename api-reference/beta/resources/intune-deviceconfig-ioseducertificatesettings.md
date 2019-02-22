---
title: iosEduCertificateSettings 资源类型
description: 适用于 iOS EDU 的受信任的根和 PFX 证书。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c94b7bc75022f8338a41da3b3b9d135dff47ac3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142649"
---
# <a name="ioseducertificatesettings-resource-type"></a>iosEduCertificateSettings 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

适用于 iOS EDU 的受信任的根和 PFX 证书。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|trustedRootCertificate|Binary|受信任的根证书。|
|certFileName|字符串|要在 UI 中显示的文件名。|
|certificationAuthority|字符串|PKCS 证书颁发机构。|
|certificationAuthorityName|字符串|PKCS 证书颁发机构名称。|
|certificateTemplateName|字符串|PKCS 证书模板名称。|
|renewalThresholdPercentage|Int32|证书续订阈值百分比。 有效值为1至99|
|certificateValidityPeriodValue|Int32|证书有效期限的值。|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|证书有效期的小数位数。 可取值为：`days`、`months`、`years`。|

## <a name="relationships"></a>Relationships
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




