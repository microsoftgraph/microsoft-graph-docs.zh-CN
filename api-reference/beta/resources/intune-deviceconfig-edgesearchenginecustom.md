---
title: edgeSearchEngineCustom 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 69395d09c01c1b92f2ae3ee1abf26eeff09618f8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425979"
---
# <a name="edgesearchenginecustom-resource-type"></a>edgeSearchEngineCustom 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

允许 IT 管理员为 MDM 控制的设备设置自定义默认搜索引擎。


继承自 [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|edgeSearchEngineOpenSearchXmlUrl|String|指向包含 OpenSearch xml 文件的 https 链接，文件中至少包含指向搜索引擎的短名称和 URL。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```




