---
title: symantecCodeSigningCertificate 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5f22f86f6facfbe1b21bb0f857b8401393ed1a77
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425993"
---
# <a name="symanteccodesigningcertificate-resource-type"></a>symantecCodeSigningCertificate 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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
|content|Binary|中的原始数据格式的 Windows Symantec 代码签名证书。|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|设置或未设置证书的状态。 可取值为：`notProvisioned`、`provisioned`。|
|password|String|.Pfx 文件所需的密码。|
|SubjectName|String|证书使用者名称。|
|subject|String|证书使用者值。|
|issuerName|String|证书颁发者名称。|
|颁发者|String|证书颁发者值。|
|expirationDateTime|DateTimeOffset|证书到期日期。|
|uploadDateTime|DateTimeOffset|作为 Symantec Cert 代码签名证书的类型。|

## <a name="relationships"></a>关系
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




