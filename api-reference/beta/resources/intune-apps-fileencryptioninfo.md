---
title: fileEncryptionInfo 资源类型
description: 包含业务线应用内容版本文件加密信息的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e5bb90354172fab1f691a49b2488871109df3532
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274269"
---
# <a name="fileencryptioninfo-resource-type"></a>fileEncryptionInfo 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




