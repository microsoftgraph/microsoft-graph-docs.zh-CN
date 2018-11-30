---
title: symantecCodeSigningCertificate 资源类型
description: 尚未记录
ms.openlocfilehash: f867f5bf6b0cad43f32dcc5ad9320421eee6d5c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044717"
---
# <a name="symanteccodesigningcertificate-resource-type"></a>symantecCodeSigningCertificate 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-get.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|读取属性和[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的关系。|
|[更新 symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-update.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|更新[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|content|二进制数|中的原始数据格式的 Windows Symantec 代码签名证书。|
|状态|[certificateStatus](../resources/intune-apps-certificatestatus.md)|设置或未设置证书的状态。 可取值为：`notProvisioned`、`provisioned`。|
|password|字符串|.Pfx 文件所需的密码。|
|SubjectName|String|证书使用者名称。|
|subject|字符串|证书使用者值。|
|issuerName|字符串|证书颁发者名称。|
|颁发者|字符串|证书颁发者值。|
|expirationDateTime|DateTimeOffset|证书到期日期。|
|uploadDateTime|DateTimeOffset|作为 Symantec Cert 代码签名证书的类型。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.symantecCodeSigningCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "String (identifier)",
  "content": "binary",
  "status": "String",
  "password": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```





