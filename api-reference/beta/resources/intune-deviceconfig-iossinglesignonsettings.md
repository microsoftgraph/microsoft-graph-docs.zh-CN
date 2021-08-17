---
title: iosSingleSignOnSettings 资源类型
description: 单一登录的 iOS Kerberos 身份验证设置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 724b6d0deb2fff796c5f7d43d961a014eadc84c2659e47392def0e803c172b5f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145395"
---
# <a name="iossinglesignonsettings-resource-type"></a>iosSingleSignOnSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

单一登录的 iOS Kerberos 身份验证设置

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedAppsList|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|允许使用此登录名的应用标识符列表。 如果省略此字段，登录名将应用于设备上的所有应用程序。 该集合最多可包含 500 个元素。|
|allowedUrls|String collection|必须匹配才能使用此登录名的 HTTP URL 列表。 对于 iOS 9.0 或更高版本，可能会使用通配符。|
|displayName|String|接收显示名称上显示的登录设置列表。|
|kerberosPrincipalName|String|Kerberos 主体名称。 如果未提供，在配置文件安装过程中将提示用户输入一个。|
|kerberosRealm|String|Kerberos 领域名称。 区分大小写。|

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




