---
title: iosRedirectSingleSignOnExtension 资源类型
description: 表示 iOS 设备的重定向类型单一登录扩展配置文件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 85048bbbdf66166a053be93a124653b17d680a21
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636691"
---
# <a name="iosredirectsinglesignonextension-resource-type"></a>iosRedirectSingleSignOnExtension 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 iOS 设备的重定向类型单一登录扩展配置文件。


继承自[iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|extensionIdentifier|字符串|获取或设置对指定 Url 执行 SSO 的应用扩展的捆绑包 ID。|
|teamIdentifier|字符串|获取或设置为指定的 Url 执行 SSO 的应用程序扩展的团队 ID。|
|配置|[keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)集合|获取或设置用于配置凭据类型配置文件的类型键/值对的列表。 该集合最多可包含 500 个元素。|
|urlPrefixes|String 集合|标识提供程序的一个或多个 URL 前缀，代表其应用程序扩展执行单一登录。 Url 必须以 http://或 https://开头。 所有 URL 前缀对所有配置文件都必须是唯一的。|

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
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ],
  "urlPrefixes": [
    "String"
  ]
}
```



