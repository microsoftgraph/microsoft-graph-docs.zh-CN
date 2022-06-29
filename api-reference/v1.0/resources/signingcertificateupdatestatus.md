---
title: signingCertificateUpdateStatus 资源类型
description: 提供签名证书上次更新的状态。
author: akgoel23
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 59129a7ce9d523c17fd4d497e91bf20da7af10b0
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447410"
---
# <a name="signingcertificateupdatestatus-resource-type"></a>signingCertificateUpdateStatus 资源类型

命名空间：microsoft.graph

提供签名证书上次更新的状态和时间戳。 

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|certificateUpdateResult|String|上次证书更新的状态。 只读。 有关状态列表，请参阅 [certificateUpdateResult 状态](#certificateupdateresult-status)。|
|lastRunDateTime|DateTimeOffset|ISO 8601 格式的日期和时间，以及上次更新证书时的 UTC 时间。 只读。 |

### <a name="certificateupdateresult-status"></a>certificateUpdateResult 状态
| 值 | 说明 |
| :--- | :--- |
|success|尝试是成功的。|
|unknownError|不知道失败的原因。|
|internalServerError|我们这边出了问题。|
|noValidExistingCertFound|找不到有效的现有签名证书。|
|noStsAuthUrlFound|未找到 STS 身份验证 URL。|
|noFederationProtocolFound|未找到联合协议。|
|noNewCertificateFound|未找到新证书。|
|couldNotAccessRemoteHost|无法联系到提供程序来获取新证书。|
|connectionError|出现连接错误|
|xmlParsingError|无法分析 XML|
|badRequest|从 Fed 元数据请求收到 BadRequest 错误。|
|未经 授权|从 Fed 元数据请求收到未经授权的错误。|
|禁止|从 Fed 元数据请求收到禁止错误。|
|notFound|从 Fed 元数据请求收到 NotFound 错误。|
|providerError|从提供程序接收了 InternalServerError。|


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

