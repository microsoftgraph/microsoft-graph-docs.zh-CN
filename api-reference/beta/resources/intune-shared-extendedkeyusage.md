---
title: extendedKeyUsage 资源类型
description: 自定义扩展密钥使用定义
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5b05bd1d1c608161e70d69fab483a383c716ec5f6f1378a4ea98eef4890d329f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126870"
---
# <a name="extendedkeyusage-resource-type"></a>extendedKeyUsage 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

自定义扩展密钥使用定义

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|String|扩展密钥使用名称|
|objectIdentifier|String|扩展密钥使用对象标识符|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```




