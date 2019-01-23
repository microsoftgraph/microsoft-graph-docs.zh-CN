---
title: iosSingleSignOnSettings 资源类型
description: iOS 的单一登录的 Kerberos 身份验证设置
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 189fb79be741bdf6b731b1e3c2b336934db8c86b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421317"
---
# <a name="iossinglesignonsettings-resource-type"></a>iosSingleSignOnSettings 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

iOS 的单一登录的 Kerberos 身份验证设置

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedAppsList|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|允许使用此登录名的应用程序标识符的列表。 如果省略此字段，则在登录适用于设备上的所有应用程序。 该集合最多可包含 500 个元素。|
|allowedUrls|String 集合|必须匹配才能使用此登录名的 HTTP Url 的列表。 与 iOS 9.0 或更高版本中，可以使用通配符。|
|displayName|String|接收设备上显示的登录设置显示名称。|
|kerberosPrincipalName|String|Kerberos 的主体名称。 如果未提供，一个配置文件安装过程中提示用户。|
|kerberosRealm|String|Kerberos 领域名。 区分大小写。|

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




