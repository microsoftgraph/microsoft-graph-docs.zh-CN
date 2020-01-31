---
title: macOSKerberosSingleSignOnExtension 资源类型
description: 表示 macOS 设备的 Kerberos 类型单一登录扩展配置文件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd43b26ba310cc9d25d719bdcae683b4f1716b41
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636698"
---
# <a name="macoskerberossinglesignonextension-resource-type"></a>macOSKerberosSingleSignOnExtension 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 macOS 设备的 Kerberos 类型单一登录扩展配置文件。


继承自[macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|型|字符串|获取或设置此配置文件的区分大小写的领域名称。|
|域|String 集合|获取或设置应用程序扩展为其执行 SSO 的主机名或域名的列表。|
|blockAutomaticLogin|Boolean|启用或禁用密钥链用法。|
|cacheName|字符串|获取或设置要用于此配置文件的 Kerberos 缓存的通用安全服务名称。|
|credentialBundleIdAccessControlList|String 集合|获取或设置允许访问 Kerberos 票证授予票证的应用捆绑包 Id 的列表。|
|domainRealms|String 集合|获取或设置自定义域领域映射的领域列表。 领域区分大小写。|
|isDefaultRealm|Boolean|如果为 true，则将选择此配置文件的领域作为默认领域。 如果配置了多个 Kerberos 类型配置文件，则必须执行此步骤。|
|passwordBlockModification|Boolean|启用或禁用密码更改。|
|passwordExpirationDays|Int32|替代默认密码到期天数（天）。 对于大多数域，此值是自动计算的。|
|passwordExpirationNotificationDays|Int32|获取或设置通知用户其密码将到期的天数（默认值为15）。|
|userPrincipalName|字符串|获取或设置要用于此配置文件的原理用户名。 不需要包含领域名称。|
|passwordRequireActiveDirectoryComplexity|Boolean|启用或禁用密码是否必须符合 Active Directory 的复杂性要求。|
|passwordPreviousPasswordBlockCount|Int32|获取或设置要阻止的以前密码的数目。|
|passwordMinimumLength|Int32|获取或设置密码的最小长度。|
|passwordMinimumAgeDays|Int32|获取或设置用户可以再次更改密码之前的最小天数。|
|passwordRequirementsDescription|字符串|获取或设置密码复杂性要求的说明。|
|requireUserPresence|Boolean|获取或设置是否需要通过触摸 ID、面孔 ID 或密码进行身份验证以访问密钥链条目。|
|activeDirectorySiteCode|字符串|获取或设置 Active Directory 站点。|
|passwordEnableLocalSync|Boolean|启用或禁用密码同步。 这不会影响使用 macOS 上的移动帐户登录的用户。|
|blockActiveDirectorySiteAutoDiscovery|Boolean|启用或禁用 Kerberos 扩展是否可以自动确定其站点名称。|
|passwordChangeUrl|字符串|获取或设置用户启动密码更改时将发送到的 URL。|

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
  "passwordChangeUrl": "String"
}
```



