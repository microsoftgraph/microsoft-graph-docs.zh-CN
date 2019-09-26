---
title: iosKerberosSingleSignOnExtension 资源类型
description: 表示 iOS 设备的 Kerberos 类型单一登录扩展配置文件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 110557ac7ee3b03c63b013406ed660cdcd24122b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37200019"
---
# <a name="ioskerberossinglesignonextension-resource-type"></a>iosKerberosSingleSignOnExtension 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 iOS 设备的 Kerberos 类型单一登录扩展配置文件。


继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|型|String|获取或设置此配置文件的区分大小写的领域名称。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|域|String collection|获取或设置应用程序扩展为其执行 SSO 的主机名或域名的列表。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|blockAutomaticLogin|Boolean|启用或禁用密钥链用法。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|cacheName|String|获取或设置要用于此配置文件的 Kerberos 缓存的通用安全服务名称。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|credentialBundleIdAccessControlList|String collection|获取或设置允许访问 Kerberos 票证授予票证的应用捆绑包 Id 的列表。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|domainRealms|String collection|获取或设置自定义域领域映射的领域列表。 领域区分大小写。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|isDefaultRealm|Boolean|如果为 true，则将选择此配置文件的领域作为默认领域。 如果配置了多个 Kerberos 类型配置文件，则必须执行此步骤。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordBlockModification|Boolean|启用或禁用密码更改。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordExpirationDays|Int32|替代默认密码到期天数（天）。 对于大多数域，此值是自动计算的。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordExpirationNotificationDays|Int32|获取或设置通知用户其密码将到期的天数（默认值为15）。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|userPrincipalName|String|获取或设置要用于此配置文件的原理用户名。 不需要包含领域名称。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordRequireActiveDirectoryComplexity|Boolean|启用或禁用密码是否必须符合 Active Directory 的复杂性要求。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordPreviousPasswordBlockCount|Int32|获取或设置要阻止的以前密码的数目。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordMinimumLength|Int32|获取或设置密码的最小长度。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordMinimumAgeDays|Int32|获取或设置用户可以再次更改密码之前的最小天数。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordRequirementsDescription|String|获取或设置密码复杂性要求的说明。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|requireUserPresence|Boolean|获取或设置是否需要通过触摸 ID、面孔 ID 或密码进行身份验证以访问密钥链条目。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|activeDirectorySiteCode|String|获取或设置 Active Directory 站点。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|passwordEnableLocalSync|Boolean|启用或禁用密码同步。 这不会影响使用 macOS 上的移动帐户登录的用户。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|
|blockActiveDirectorySiteAutoDiscovery|Boolean|启用或禁用 Kerberos 扩展是否可以自动确定其站点名称。 继承自[kerberosSingleSignOnExtension](../resources/intune-deviceconfig-kerberossinglesignonextension.md)|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosKerberosSingleSignOnExtension",
  "realm": "String",
  "domains": [
    "String"
  ],
  "blockAutomaticLogin": true,
  "cacheName": "String",
  "credentialBundleIdAccessControlList": [
    "String"
  ],
  "domainRealms": [
    "String"
  ],
  "isDefaultRealm": true,
  "passwordBlockModification": true,
  "passwordExpirationDays": 1024,
  "passwordExpirationNotificationDays": 1024,
  "userPrincipalName": "String",
  "passwordRequireActiveDirectoryComplexity": true,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumAgeDays": 1024,
  "passwordRequirementsDescription": "String",
  "requireUserPresence": true,
  "activeDirectorySiteCode": "String",
  "passwordEnableLocalSync": true,
  "blockActiveDirectorySiteAutoDiscovery": true
}
```



