---
title: customExtensionAuthenticationConfiguration 资源类型
description: 抽象基类型，公开从 customCalloutExtension 抽象类型继承的派生类型的 **authenticationConfiguration** 属性的配置
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3fbe85e5cca096ad0af24b7d0ffa04e035be63a9
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338219"
---
# <a name="customextensionauthenticationconfiguration-resource-type"></a>customExtensionAuthenticationConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

抽象基类型，公开从 [customCalloutExtension](customcalloutextension.md) 抽象类型继承的派生类型的 **authenticationConfiguration** 属性的配置。 此抽象类型由 [azureAdTokenAuthentication 资源](../resources/azureadtokenauthentication.md) 类型继承。

## <a name="properties"></a>属性

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customExtensionAuthenticationConfiguration",
  "abstract": true
}
-->

``` json
{ 
  "@odata.type": "#microsoft.graph.customExtensionAuthenticationConfiguration " 
} 
```