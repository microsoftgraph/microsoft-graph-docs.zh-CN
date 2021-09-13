---
title: iosRedirectSingleSignOnExtension 资源类型
description: 表示 iOS 设备的重定向Sign-On类型单一应用扩展配置文件。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e80bb592364e82c155c11e65c5ec48a781e53e4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057472"
---
# <a name="iosredirectsinglesignonextension-resource-type"></a>iosRedirectSingleSignOnExtension 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 iOS 设备的重定向Sign-On类型单一应用扩展配置文件。


继承自 [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|extensionIdentifier|String|获取或设置为指定 URL 执行 SSO 的应用扩展的捆绑 ID。|
|teamIdentifier|String|获取或设置为指定 URL 执行 SSO 的应用扩展的团队 ID。|
|配置|[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) 集合|获取或设置用于配置凭据类型配置文件的键入键值对的列表。 该集合最多可包含 500 个元素。|
|urlPrefixes|字符串集合|标识提供程序的一个或多个 URL 前缀，应用扩展代表这些提供程序执行单一登录。 URL 必须以 http:// 或 https:// 开头。 所有 URL 前缀对于所有配置文件都必须是唯一的。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosRedirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosRedirectSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyTypedValuePair",
      "key": "String"
    }
  ],
  "urlPrefixes": [
    "String"
  ]
}
```



