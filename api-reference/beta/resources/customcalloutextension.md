---
title: customCalloutExtension 资源类型
description: 一个抽象类型，用于定义逻辑应用的配置，这些应用可以与客户的权利管理用例集成，以实施更广泛的治理工作流。 此抽象类型由 customAccessPackageWorkflowExtension 资源类型继承
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7a76c37663fb3d9c5a49c1c539d1238d7423ba4a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338409"
---
# <a name="customcalloutextension-resource-type"></a>customCalloutExtension 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一个抽象类型，用于定义逻辑应用的配置，这些应用可以与客户的权利管理用例集成，以实施更广泛的治理工作流。 此抽象类型由 [customAccessPackageWorkflowExtension](customaccesspackageworkflowextension.md) 资源类型继承。

继承自 [实体](entity.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|authenticationConfiguration|[customExtensionAuthenticationConfiguration](../resources/customextensionauthenticationconfiguration.md)|用于保护对逻辑应用的 API 调用的配置。 例如，使用 OAuth 客户端凭据流。 |
|clientConfiguration|[customExtensionClientConfiguration](../resources/customextensionclientconfiguration.md)| HTTP 连接设置，用于定义 Azure AD 可以等待连接到逻辑应用的时间、可以重试已退出连接多少次以及允许重试时出现异常情况。|
|说明|String|customCalloutExtension 对象的说明。|
|displayName|String|customCalloutExtension 对象的显示名称。|
|endpointConfiguration|[customExtensionEndpointConfiguration](../resources/customextensionendpointconfiguration.md)|用于配置终结点以调用逻辑应用的工作流的类型和详细信息。|
|id|String|customCalloutExtension 对象的标识符。 继承自 [实体](../resources/entity.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.customCalloutExtension",
  "openType": false,
  "abstract": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customCalloutExtension",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "endpointConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionEndpointConfiguration"
  },
  "clientConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionClientConfiguration"
  },
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionAuthenticationConfiguration"
  }
}
```

