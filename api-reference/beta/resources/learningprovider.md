---
title: learningProvider 资源类型
description: 表示包含有关学习提供程序的详细信息的实体。
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: resourcePageType
ms.openlocfilehash: eb68ab517f0df414202ac8d676838fb3161472cf
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883290"
---
# <a name="learningprovider-resource-type"></a>learningProvider 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个实体，该实体包含有关 Viva learning 中学习提供程序的详细信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 learningProviders](../api/employeeexperience-list-learningproviders.md)|[learningProvider](../resources/learningprovider.md) 集合|获取在租户Viva Learning中注册的 [learningProvider](../resources/learningprovider.md) 资源的列表。|
|[创建 learningProvider](../api/employeeexperience-post-learningproviders.md)|[learningProvider](../resources/learningprovider.md)|创建一个新的 [learningProvider](../resources/learningprovider.md) 对象，并使用不同主题的指定显示名称和徽标向Viva Learning注册该对象。|
|[获取 learningProvider](../api/learningprovider-get.md)|[learningProvider](../resources/learningprovider.md)|读取 [learningProvider](../resources/learningprovider.md) 对象的属性和关系。|
|[更新 learningProvider](../api/learningprovider-update.md)|[learningProvider](../resources/learningprovider.md)|更新 [learningProvider](../resources/learningprovider.md) 对象的属性。|
|[删除 learningProvider](../api/employeeexperience-delete-learningproviders.md)|无|删除 [learningProvider](../resources/learningprovider.md) 资源并在租户的Viva Learning中删除其注册。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|Viva Learning中显示的显示名称。 必需。|
|id|String|学习提供程序的唯一标识符。 必需。|
|isEnabled|Boolean|提供程序的状态。 可选。|
|loginWebUrl|String|用于访问提供程序课程的身份验证 URL。 可选。|
|longLogoWebUrlForDarkTheme|String|深色模式的长徽标 URL，需要是可公开访问的图像。 此映像将保存到 Viva Learning 的 Blob 存储中，以便在Viva Learning应用中呈现。 必需。|
|longLogoWebUrlForLightTheme|String|光模式的长徽标 URL，需要是可公开访问的图像。 此映像将保存到 Viva Learning 的 Blob 存储中，以便在Viva Learning应用中呈现。 必需。|
|squareLogoWebUrlForDarkTheme|String|深色模式的方形徽标 URL，需要是可公开访问的图像。 此映像将保存到 Viva Learning 的 Blob 存储中，以便在Viva Learning应用中呈现。 必需。|
|squareLogoWebUrlForLightTheme|String|光模式的方形徽标 URL，需要是可公开访问的图像。 此映像将保存到 Viva Learning 的 Blob 存储中，以便在Viva Learning应用中呈现。 必填。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|learningContents|[learningContent](../resources/learningcontent.md) 集合|学习提供程序的目录项。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.learningProvider",
  "openType": false
}
-->
``` json
{
    "@odata.type": "#microsoft.graph.learningProvider",
    "displayName": "String",
    "id": "String (identifier)",
    "isEnabled": "Boolean",
    "loginWebUrl": "String",
    "longLogoWebUrlForDarkTheme": "String",
    "longLogoWebUrlForLightTheme": "String",
    "squareLogoWebUrlForDarkTheme": "String",
    "squareLogoWebUrlForLightTheme": "String"
}
```

