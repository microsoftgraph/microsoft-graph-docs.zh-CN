---
title: fileEncryptionInfo 资源类型
description: 包含业务线应用内容版本文件加密信息的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 03d8adbbf43b38bfc7d13bec2db09c2be8c3b2ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868969"
---
# <a name="fileencryptioninfo-resource-type"></a>fileEncryptionInfo 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含业务线应用内容版本文件加密信息的属性。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|encryptionKey|Binary|用于加密文件内容的密钥。|
|initializationVector|Binary|用于加密算法的初始化向量。|
|mac|Binary|加密文件内容和 IV 的哈希（内容哈希）。|
|macKey|Binary|用于获取 mac 的密钥。|
|profileIdentifier|String|配置文件标识符。|
|fileDigest|Binary|加密前的文件摘要。|
|fileDigestAlgorithm|String|文件摘要算法。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```





