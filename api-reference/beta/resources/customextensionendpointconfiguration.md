---
title: customExtensionEndpointConfiguration 资源类型
description: 抽象基类型，公开用于配置自定义访问包工作流扩展对象的 endpointConfiguration 属性的派生类型。
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8607ee8311c0cfc64eef06c3dc2716fb775473fa
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338394"
---
# <a name="customextensionendpointconfiguration-resource-type"></a>customExtensionEndpointConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

抽象基类型，公开用于配置自定义访问包工作流扩展对象的 **endpointConfiguration** 属性的 [派生](customaccesspackageworkflowextension.md) 类型。 此抽象类型由 [logicAppTriggerEndpointConfiguration 对象](logicapptriggerendpointconfiguration.md) 继承。

## <a name="properties"></a>属性

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customExtensionEndpointConfiguration",
  "abstract": true
}
-->
``` json
{ 
  "@odata.type": "#microsoft.graph.customExtensionEndpointConfiguration" 
} 
```