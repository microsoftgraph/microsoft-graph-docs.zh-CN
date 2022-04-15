---
title: signingCertificateUpdateStatus 资源类型
description: 提供签名证书上次更新的状态。
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 108b5169ac9b043e4ce2a80f5c620a266d391338
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2022
ms.locfileid: "64852664"
---
# <a name="signingcertificateupdatestatus-resource-type"></a>signingCertificateUpdateStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供签名证书上次更新的状态和时间戳。 

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|certificateUpdateResult|字符串|上次证书更新的状态。 只读。 有关状态列表，请参阅 [certificateUpdateResult 状态](#certificateupdateresult-status)。|
|lastRunDateTime|DateTimeOffset|ISO 8601 格式的日期和时间，以及上次更新证书时的 UTC 时间。 只读。 |

### <a name="certificateupdateresult-status"></a>certificateUpdateResult 状态
| 值 | 说明 |
| :--- | :--- |
|success|证书更新操作成功。|
|unknownError|失败的原因未定义。|
|internalServerError|处理请求时出现内部服务器错误。|
|noValidExistingCertFound|找不到有效的现有签名证书。|
|noStsAuthUrlFound|未找到 STS 身份验证 URL。|
|noFederationProtocolFound|联合协议未定义。|
|noNewCertificateFound|未找到新证书。|
|couldNotAccessRemoteHost|无法联系到提供程序来获取新证书。|
|connectionError|出现连接错误，例如连接超时。|
|xmlParsingError|无法分析 XML。|
|badRequest|`400 BadRequest`在 Fed 元数据请求中收到错误代码。|
|未经 授权|在 Fed 元数据请求中收到 `401 Unauthorized` 错误代码。|
|禁止|在 Fed 元数据请求中收到 `403 Forbidden` 错误代码。|
|notFound|在 Fed 元数据请求中收到 `404 NotFound` 错误代码。|
|providerError|`500 InternalServerError`从提供程序收到错误代码。|


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.signingCertificateUpdateStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.signingCertificateUpdateStatus",
  "certificateUpdateResult": "String",
  "lastRunDateTime": "String (timestamp)"
}
```

