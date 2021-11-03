---
title: macOSKerberosSingleSignOnExtension 资源类型
description: 表示适用于 macOS 设备的 Kerberos 类型的单Sign-On扩展配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9401d3cf92a3f153d7bb1547416d866c2833010a
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695263"
---
# <a name="macoskerberossinglesignonextension-resource-type"></a>macOSKerberosSingleSignOnExtension 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示适用于 macOS 设备的 Kerberos 类型的单Sign-On扩展配置文件。


继承自 [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|realm|String|获取或设置此配置文件的区分大小写的领域名称。|
|domains|String collection|获取或设置应用扩展执行 SSO 的主机或域名的列表。|
|blockAutomaticLogin|布尔值|启用或禁用钥匙链用法。|
|cacheName|String|获取或设置要用于此配置文件的 Kerberos 缓存的通用安全服务名称。|
|credentialBundleIdAccessControlList|String collection|获取或设置允许访问 Kerberos 票证授予票证的应用程序包 ID 的列表。|
|domainRealms|String collection|获取或设置自定义域领域映射的领域列表。 领域区分大小写。|
|isDefaultRealm|布尔值|如果为 true，则此配置文件的领域将选择为默认值。 如果配置了多个 Kerberos 类型的配置文件，则是必需的。|
|passwordBlockModification|布尔值|启用或禁用密码更改。|
|passwordExpirationDays|Int32|替代默认密码过期天数。 对于大多数域，此值将自动计算。|
|passwordExpirationNotificationDays|Int32|获取或设置在通知用户其密码将过期的天数 (默认值为 15) 。|
|userPrincipalName|String|获取或设置要用于此配置文件的原则用户名。 无需包括领域名称。|
|passwordRequireActiveDirectoryComplexity|布尔值|启用或禁用密码是否必须满足 Active Directory 的复杂性要求。|
|passwordPreviousPasswordBlockCount|Int32|获取或设置要阻止的以前密码的数量。|
|passwordMinimumLength|Int32|获取或设置密码的最小长度。|
|passwordMinimumAgeDays|Int32|获取或设置用户可再次更改其密码之前的最小天数。|
|passwordRequirementsDescription|String|获取或设置密码复杂性要求的说明。|
|requireUserPresence|布尔值|获取或设置是否需要通过触摸 ID、人脸 ID 或密码进行身份验证才能访问钥匙链条目。|
|activeDirectorySiteCode|String|获取或设置 Active Directory 站点。|
|passwordEnableLocalSync|布尔值|启用或禁用密码同步。 这不会影响使用 macOS 上的移动帐户登录的用户。|
|blockActiveDirectorySiteAutoDiscovery|布尔值|启用或禁用 Kerberos 扩展是否可自动确定其站点名称。|
|passwordChangeUrl|字符串|获取或设置用户启动密码更改时将发送到的 URL。|
|modeCredentialUsed|String|选择其他进程如何使用 Kerberos 扩展凭据。|
|usernameLableCustom|字符串|即将被弃用。|
|usernameLabelCustom|String|此标签替换 Kerberos 扩展中显示的用户名。 可以输入名称以匹配公司或组织的名称。 适用于运行 macOS 版本 11 和更高版本的设备。|
|userSetupDelayed|布尔值|设置为 True 时，在管理员启用该扩展或收到 Kerberos 质询之前，不会提示用户设置 Kerberos 扩展。 适用于运行 macOS 版本 11 和更高版本的设备。|
|signInHelpText|String|在 Kerberos 登录窗口向用户显示的文本。 适用于运行 iOS 和 iPadOS 版本 14 及更高版本的设备。|
|kerberosAppsInBundleIdACLIncluded|布尔值|设置为 True 时，Kerberos 扩展允许使用应用程序包 ID、托管应用和标准 Kerberos 实用工具（如 TicketViewer 和 klist）输入的任何应用访问和使用凭据。 适用于运行 macOS 版本 12 和更高版本的设备。|
|managedAppsInBundleIdACLIncluded|布尔值|设置为 True 时，Kerberos 扩展允许托管应用以及使用应用程序包 ID 输入的任何应用访问凭据。 设置为 False 时，Kerberos 扩展允许所有应用访问凭据。 适用于运行 iOS 和 iPadOS 版本 14 及更高版本的设备。|
|credentialsCacheMonitored|布尔值|设置为 True 时，在下次匹配的 Kerberos 质询或网络状态更改时请求凭据。 当凭据过期或丢失时，将创建一个新凭据。 适用于运行 macOS 版本 12 和更高版本的设备。|
|singleSignOnExtensionPreferredKDCs|String collection|即将被弃用。|
|preferredKDC|String collection|Add 创建用于 Kerberos 流量 (KDC) 首选密钥分发中心的有序列表。 当服务器不可使用 DNS 发现时，将使用此列表。 当服务器可发现时，该列表用于两种连接检查，并首先用于 Kerberos 流量。 如果服务器未响应，则设备使用 DNS 发现。 删除 将删除现有列表，设备使用 DNS 发现。 适用于运行 macOS 版本 12 和更高版本的设备。|
|tlsForLDAPRequired|布尔值|设置为 True 时，LDAP 连接需要使用传输层安全性 (TLS) 。 适用于运行 macOS 版本 11 和更高版本的设备。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKerberosSingleSignOnExtension",
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
  "blockActiveDirectorySiteAutoDiscovery": true,
  "passwordChangeUrl": "String",
  "modeCredentialUsed": "String",
  "usernameLableCustom": "String",
  "usernameLabelCustom": "String",
  "userSetupDelayed": true,
  "signInHelpText": "String",
  "kerberosAppsInBundleIdACLIncluded": true,
  "managedAppsInBundleIdACLIncluded": true,
  "credentialsCacheMonitored": true,
  "singleSignOnExtensionPreferredKDCs": [
    "String"
  ],
  "preferredKDCs": [
    "String"
  ],
  "tlsForLDAPRequired": true
}
```



