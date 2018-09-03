# <a name="windowsinformationprotectionpolicy-resource-type"></a>windowsInformationProtectionPolicy 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

不使用 MDM 进行 Windows 信息保护的策略

继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 windowsInformationProtectionPolicies](../api/intune_mam_windowsinformationprotectionpolicy_list.md)|[windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) 集合|列出 [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) 对象的属性和关系。|
|[获取 windowsInformationProtectionPolicy](../api/intune_mam_windowsinformationprotectionpolicy_get.md)|[windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)|读取 [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) 对象的属性和关系。|
|[创建 windowsInformationProtectionPolicy](../api/intune_mam_windowsinformationprotectionpolicy_create.md)|[windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)|创建新的 [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) 对象。|
|[删除 windowsInformationProtectionPolicy](../api/intune_mam_windowsinformationprotectionpolicy_delete.md)|无|删除 [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)。|
|[更新 windowsInformationProtectionPolicy](../api/intune_mam_windowsinformationprotectionpolicy_update.md)|[windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)|更新 [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|策略显示名称。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|描述|字符串|策略的说明。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|id|字符串|实体的键。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|版本|字符串|实体的版本。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|enforcementLevel|[windowsInformationProtectionEnforcementLevel](../resources/intune_mam_windowsinformationprotectionenforcementlevel.md)|WIP 强制级别。请参见对继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) 的支持值枚举定义。 可能的值为： `noProtection` 、 `encryptAndAuditOnly` 、 `encryptAuditAndPrompt` 、 `encryptAuditAndBlock` 。|
|enterpriseDomain|字符串|主企业域。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|enterpriseProtectedDomainNames|[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合|要保护的企业域列表。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|protectionUnderLockConfigRequired|布尔|指定是否应配置锁定功能下的保护（也称为 PIN 下的加密）。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/intune_mam_windowsinformationprotectiondatarecoverycertificate.md)|指定可用于加密文件数据恢复的恢复证书。 这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|revokeOnUnenrollDisabled|布尔|此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。 如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。 如果未撤销密钥，随后将不会撤销文件清除。 继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|rightsManagementServicesTemplateId|Guid|用于 RMS 加密的 TemplateID GUID。 RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|azureRightsManagementServicesAllowed|布尔|指定是否允许 WIP 使用 Azure RMS 加密。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|iconsVisible|布尔|确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。 从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|protectedApps|[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) 集合|受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|exemptApps|[windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md) 集合|豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。 这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。 继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|enterpriseNetworkDomainNames|[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合|这是构成企业边界的域列表。 发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|enterpriseProxiedDomains|[windowsInformationProtectionProxiedDomainCollection](../resources/intune_mam_windowsinformationprotectionproxieddomaincollection.md) 集合|包含需要保护的托管在云中的企业资源域列表。 与这些资源的连接被视为企业数据。 如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。 用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|enterpriseIPRanges|[windowsInformationProtectionIPRangeCollection](../resources/intune_mam_windowsinformationprotectioniprangecollection.md) 集合|设置可定义企业网络中计算机的企业 IP 范围。 来自这些计算机的数据将被视为企业的一部分并受保护。 这些位置将被视为共享企业数据的安全目标。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|enterpriseIPRangesAreAuthoritative|布尔|用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。 默认值为 false。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|enterpriseProxyServers|[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合|这是代理服务器的列表。 任何不在此列表中的服务器都被视为非企业服务器。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|enterpriseInternalProxyServers|[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合|这是逗号分隔的内部代理服务器列表。 例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。 这些代理已由管理员配置为连接到 Internet 上的特定资源。 它们被视为企业版网络位置。 仅在配置 EnterpriseProxiedDomains 策略时利用代理，强制流量通过这些代理传输到匹配的域。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|enterpriseProxyServersAreAuthoritative|布尔|用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。 默认值为 false。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|neutralDomainResources|[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合|可用于工作或个人资源的域名列表。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|indexingEncryptedStoresOrItemsBlocked|布尔|此开关用于 Windows Search 索引器，以允许或禁止建立项目索引。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|smbAutoEncryptedFileExtensions|[windowsInformationProtectionResourceCollection](../resources/intune_mam_windowsinformationprotectionresourcecollection.md) 集合|指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件。继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|isAssigned|布尔|指示策略是否部署到任何包含组。 继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|revokeOnMdmHandoffDisabled|布尔|RS2 中的新属性，待定文档|
|mdmEnrollmentUrl|字符串|MDM 的注册 URL|
|windowsHelloForBusinessBlocked|布尔|将 Windows Hello 企业版设置为登录 Windows 的方法的布尔值。|
|pinMinimumLength|Int32|整数值，用于设置 PIN 所需的最少字符数。 默认值为 4。 可以为此策略设置配置的最小数量为 4。 可以配置的最大数量必须小于最大 PIN 长度策略设置中配置的数量或 127（以最低者为准）。|
|pinUppercaseLetters|[windowsInformationProtectionPinCharacterRequirements](../resources/intune_mam_windowsinformationprotectionpincharacterrequirements.md)|用于配置 Windows Hello for Business PIN 中大写字母使用的整数值。 默认方式为 NotAllow。 可能的值为： `notAllow` 、 `requireAtLeastOne` 、 `allow` 。|
|pinLowercaseLetters|[windowsInformationProtectionPinCharacterRequirements](../resources/intune_mam_windowsinformationprotectionpincharacterrequirements.md)|用于配置 Windows Hello for Business PIN 中小写字母使用整数值。 默认方式为 NotAllow。 可能的值为： `notAllow` 、 `requireAtLeastOne` 、 `allow` 。|
|pinSpecialCharacters|[windowsInformationProtectionPinCharacterRequirements](../resources/intune_mam_windowsinformationprotectionpincharacterrequirements.md)|配置 Windows Hello for Business PIN 中特殊字母使用整数值。 Windows Hello 企业版 PIN 手势的有效特殊字符包括：! " # $ % & ' ( ) * + , - . / : ; < = > ? @ \[ \ \] ^ _ ` { | } ~。 默认方式为 NotAllow。 可能的值为： `notAllow` 、 `requireAtLeastOne` 、 `allow` 。|
|pinExpirationDays|Int32|整数值指定在系统要求用户更改 PIN 之前可以使用 PIN 的时间段（以天为单位）。 可以为此策略设置配置的最大数量为 730。 可以为此策略设置配置的最小数量为 0。 如果此策略设置为 0，则用户的 PIN 永远不会过期。 此节点在 Windows 10 版本 1511 中添加。 默认值为 0。|
|numberOfPastPinsRemembered|Int32|整数值，用于指定可以关联到无法重用的用户帐户的过去 PIN 的数量。 可以为此策略设置配置的最大数量为 50。 可以为此策略设置配置的最小数量为 0。 如果此策略设置为 0，则不需要存储以前的 PIN。 此节点在 Windows 10 版本 1511 中添加。 默认值为 0。|
|passwordMaximumAttemptCount|Int32|在擦除设备之前允许的身份验证失败次数。 值为 0 将禁用设备擦除功能。 范围是一个整数 X，其中对于台式机 4 <= X <= 16，对于移动设备 0 <= X <= 999。|
|minutesOfInactivityBeforeDeviceLock|Int32|指定设备闲置后将导致设备变为 PIN 或密码锁定的允许的最长时间（以分钟为单位）。   范围是整数 X，其中 0 < = X < = 999。|
|daysWithoutContactBeforeUnenroll|Int32|擦除应用数据之前的脱机间隔时间（天） |

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|protectedAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) 集合|通过 xml 文件输入受保护应用的另一种方法 继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|exemptAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) 集合|通过 xml 文件输入豁免应用的另一种方法 继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|
|工作分配|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) 集合|针对策略的安全组列表的导航属性。 继承自 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.windowsInformationProtection",
  "@odata.type": "microsoft.graph.windowsInformationProtectionPolicy"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "enforcementLevel": "String",
  "enterpriseDomain": "String",
  "enterpriseProtectedDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "protectionUnderLockConfigRequired": true,
  "dataRecoveryCertificate": {
    "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
    "subjectName": "String",
    "description": "String",
    "expirationDateTime": "String (timestamp)",
    "certificate": "binary"
  },
  "revokeOnUnenrollDisabled": true,
  "rightsManagementServicesTemplateId": "79199ed9-e50b-4257-8de4-70b9c8685061",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "enterpriseNetworkDomainNames": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxiedDomains": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
      "displayName": "String",
      "proxiedDomains": [
        {
          "@odata.type": "microsoft.graph.proxiedDomain",
          "ipAddressOrFQDN": "String",
          "proxy": "String"
        }
      ]
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
      "displayName": "String",
      "ranges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ]
    }
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseInternalProxyServers": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "indexingEncryptedStoresOrItemsBlocked": true,
  "smbAutoEncryptedFileExtensions": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
      "displayName": "String",
      "resources": [
        "String"
      ]
    }
  ],
  "isAssigned": true,
  "revokeOnMdmHandoffDisabled": true,
  "mdmEnrollmentUrl": "String",
  "windowsHelloForBusinessBlocked": true,
  "pinMinimumLength": 1024,
  "pinUppercaseLetters": "String",
  "pinLowercaseLetters": "String",
  "pinSpecialCharacters": "String",
  "pinExpirationDays": 1024,
  "numberOfPastPinsRemembered": 1024,
  "passwordMaximumAttemptCount": 1024,
  "minutesOfInactivityBeforeDeviceLock": 1024,
  "daysWithoutContactBeforeUnenroll": 1024
}
```



