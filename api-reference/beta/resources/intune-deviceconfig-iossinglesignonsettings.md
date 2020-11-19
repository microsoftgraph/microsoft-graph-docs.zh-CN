---
title: iosSingleSignOnSettings 资源类型
description: 单一登录的 iOS Kerberos 身份验证设置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 02f8b554fef07de6a429cf38722f0c867432f909
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49303123"
---
# <a name="iossinglesignonsettings-resource-type"></a>iosSingleSignOnSettings 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

单一登录的 iOS Kerberos 身份验证设置

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|allowedAppsList|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|允许使用此登录名的应用程序标识符列表。 如果省略此字段，则登录将应用于设备上的所有应用程序。 该集合最多可包含 500 个元素。|
|allowedUrls|String 集合|必须匹配才能使用此登录的 HTTP Url 的列表。 对于 iOS 9.0 或更高版本，可以使用通配符。|
|displayName|字符串|在接收设备上显示的登录设置的显示名称。|
|kerberosPrincipalName|字符串|Kerberos 主体名称。 如果未提供，则在配置文件安装过程中系统会提示用户一个。|
|kerberosRealm|字符串|Kerberos 领域名称。 区分大小写。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```




