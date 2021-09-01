---
title: symantecCodeSigningCertificate 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 817911afa2d18a0c0dc50a1f98afbbe412f7aba9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58784000"
---
# <a name="symanteccodesigningcertificate-resource-type"></a>symantecCodeSigningCertificate 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-get.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|读取 [symantecCodeSigningCertificate 对象的属性和](../resources/intune-apps-symanteccodesigningcertificate.md) 关系。|
|[更新 symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-update.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|更新 [symantecCodeSigningCertificate 对象](../resources/intune-apps-symanteccodesigningcertificate.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|content|二进制|The Windows Symantec Code-Signing Certificate in the raw data format.|
|状态|[certificateStatus](../resources/intune-apps-certificatestatus.md)|已设置或未预配证书状态。 可取值为：`notProvisioned`、`provisioned`。|
|密码|String|.pfx 文件所需的密码。|
|SubjectName|String|证书的主题名称。|
|subject|String|证书的 Subject 值。|
|issuerName|字符串|证书的颁发者名称。|
|issuer|字符串|证书的 Issuer 值。|
|expirationDateTime|DateTimeOffset|证书到期日期。|
|uploadDateTime|DateTimeOffset|作为 Symantec 证书的 CodeSigning 证书的类型。|

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



