---
title: iosKerberosSingleSignOnExtension 资源类型
description: 表示适用于 iOS 设备的 Kerberos 类型的单Sign-On扩展配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90cca5e1488ce4fff9742099209b3e3e03bf5716
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347394"
---
# <a name="ioskerberossinglesignonextension-resource-type"></a>iosKerberosSingleSignOnExtension 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示适用于 iOS 设备的 Kerberos 类型的单Sign-On扩展配置文件。


继承自 [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|realm|String|获取或设置此配置文件的区分大小写的领域名称。|
|domains|String collection|获取或设置应用扩展执行 SSO 的主机或域名的列表。|
|blockAutomaticLogin|布尔|启用或禁用钥匙链用法。|
|cacheName|String|获取或设置要用于此配置文件的 Kerberos 缓存的通用安全服务名称。|
|credentialBundleIdAccessControlList|String collection|获取或设置允许访问 Kerberos 票证授予票证的应用程序包 ID 的列表。|
|domainRealms|字符串集合|获取或设置自定义域领域映射的领域列表。 领域区分大小写。|
|isDefaultRealm|Boolean|如果为 true，则此配置文件的领域将选择为默认值。 如果配置了多个 Kerberos 类型的配置文件，则是必需的。|
|passwordBlockModification|布尔|启用或禁用密码更改。|
|passwordExpirationDays|Int32|替代默认密码过期天数。 对于大多数域，此值将自动计算。|
|passwordExpirationNotificationDays|Int32|获取或设置在用户收到密码过期通知之前 (默认值为 15) 。|
|userPrincipalName|String|获取或设置要用于此配置文件的原则用户名。 无需包括领域名称。|
|passwordRequireActiveDirectoryComplexity|Boolean|启用或禁用密码是否必须满足 Active Directory 的复杂性要求。|
|passwordPreviousPasswordBlockCount|Int32|获取或设置要阻止的以前密码的数量。|
|passwordMinimumLength|Int32|获取或设置密码的最小长度。|
|passwordMinimumAgeDays|Int32|获取或设置用户可再次更改其密码之前的最小天数。|
|passwordRequirementsDescription|String|获取或设置密码复杂性要求的说明。|
|requireUserPresence|Boolean|获取或设置是否需要通过触摸 ID、人脸 ID 或密码进行身份验证才能访问钥匙链条目。|
|activeDirectorySiteCode|String|获取或设置 Active Directory 站点。|
|passwordEnableLocalSync|Boolean|启用或禁用密码同步。 这不会影响使用 macOS 上的移动帐户登录的用户。|
|blockActiveDirectorySiteAutoDiscovery|Boolean|启用或禁用 Kerberos 扩展是否可自动确定其站点名称。|
|passwordChangeUrl|String|获取或设置用户启动密码更改时将发送到的 URL。|
|signInHelpText|String|在 Kerberos 登录窗口向用户显示的文本。 适用于运行 iOS 和 iPadOS 版本 14 及更高版本的设备。|
|managedAppsInBundleIdACLIncluded|Boolean|设置为 True 时，Kerberos 扩展允许托管应用以及使用应用程序包 ID 输入的任何应用访问凭据。 设置为 False 时，Kerberos 扩展允许所有应用访问凭据。 适用于运行 iOS 和 iPadOS 版本 14 及更高版本的设备。|

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
  "blockActiveDirectorySiteAutoDiscovery": true,
  "passwordChangeUrl": "String",
  "signInHelpText": "String",
  "managedAppsInBundleIdACLIncluded": true
}
```




