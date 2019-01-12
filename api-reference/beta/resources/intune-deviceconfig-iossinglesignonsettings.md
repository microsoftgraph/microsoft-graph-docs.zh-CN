---
title: iosSingleSignOnSettings 资源类型
description: iOS 的单一登录的 Kerberos 身份验证设置
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 54c5656de6262692324cce8ab71a0e100672c050
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952669"
---
# <a name="iossinglesignonsettings-resource-type"></a>iosSingleSignOnSettings 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

iOS 的单一登录的 Kerberos 身份验证设置
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowedAppsList|[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合|允许使用此登录名的应用程序标识符的列表。 如果省略此字段，则在登录适用于设备上的所有应用程序。 该集合最多可包含 500 个元素。|
|allowedUrls|String 集合|必须匹配才能使用此登录名的 HTTP Url 的列表。 与 iOS 9.0 或更高版本中，可以使用通配符。|
|displayName|字符串|接收设备上显示的登录设置显示名称。|
|kerberosPrincipalName|字符串|Kerberos 的主体名称。 如果未提供，一个配置文件安装过程中提示用户。|
|kerberosRealm|字符串|Kerberos 领域名。 区分大小写。|

## <a name="relationships"></a>Relationships
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





