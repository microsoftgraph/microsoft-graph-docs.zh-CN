---
title: extendedKeyUsage 资源类型
description: 自定义扩展密钥使用率定义
author: tfitzmac
ms.openlocfilehash: 2b6155a0fbb234cb0b2081a8a4a226a8d218dbc2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337287"
---
# <a name="extendedkeyusage-resource-type"></a>extendedKeyUsage 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

自定义扩展密钥使用率定义
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|字符串|扩展的密钥用法名称|
|objectIdentifier|字符串|扩展密钥用法对象标识符|

## <a name="relationships"></a>Relationships
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





