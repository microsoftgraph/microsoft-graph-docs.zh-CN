---
title: iosEduCertificateSettings 资源类型
description: 适用于 iOS EDU 的受信任的根和 PFX 证书。
author: tfitzmac
ms.openlocfilehash: 8e373a7c878dd06870b13a32c428f837d741964c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332324"
---
# <a name="ioseducertificatesettings-resource-type"></a>iosEduCertificateSettings 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

适用于 iOS EDU 的受信任的根和 PFX 证书。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|trustedRootCertificate|Binary|受信任的根证书。|
|certFileName|字符串|若要在 UI 中显示的文件名。|
|certificationAuthority|字符串|PKCS 证书颁发机构。|
|certificationAuthorityName|字符串|PKCS 证书颁发机构的名称。|
|certificateTemplateName|字符串|PKCS 证书模板名称。|
|renewalThresholdPercentage|Int32|证书续订阈值百分比。 有效的值 1 到 99|
|certificateValidityPeriodValue|Int32|证书有效期限的值。|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|证书有效期限的小数位数。 可取值为：`days`、`months`、`years`。|

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





