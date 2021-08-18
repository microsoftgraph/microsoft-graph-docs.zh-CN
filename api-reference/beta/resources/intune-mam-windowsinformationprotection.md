---
title: windowsInformationProtection 资源类型
description: 用于配置详细管理设置的 Windows 信息保护策略
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 24ea9f9195c45c234a99fc87a5b65f93a9cb9891aab8e926ff321bdd75913df0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54242508"
---
# <a name="windowsinformationprotection-resource-type"></a>windowsInformationProtection 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于配置详细管理设置的 Windows 信息保护策略


继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[List windowsInformationProtections](../api/intune-mam-windowsinformationprotection-list.md)|[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) 集合|列出 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) 对象的属性和关系。|
|[Get windowsInformationProtection](../api/intune-mam-windowsinformationprotection-get.md)|[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)|读取 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) 对象的属性和关系。|
|[assign 操作](../api/intune-mam-windowsinformationprotection-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|策略显示名称。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|description|String|策略的说明。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|roleScopeTagIds|String collection|此实体实例的范围标记列表。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|id|字符串|实体的键。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|version|String|实体的版本。 继承自 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|
|enforcementLevel|[windowsInformationProtectionEnforcementLevel](../resources/intune-mam-windowsinformationprotectionenforcementlevel.md)|WIP 强制级别。有关支持的值，请参阅 Enum 定义。 可取值为：`noProtection`、`encryptAndAuditOnly`、`encryptAuditAndPrompt`、`encryptAuditAndBlock`。|
|enterpriseDomain|String|主企业域|
|enterpriseProtectedDomainNames|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合|要保护的企业域列表|
|protectionUnderLockConfigRequired|Boolean|指定是否应配置锁定功能下的保护（也称为 pin 下的加密）|
|dataRecoveryCertificate|[windowsInformationProtectionDataRecoveryCertificate](../resources/intune-mam-windowsinformationprotectiondatarecoverycertificate.md)|指定可用于加密文件数据恢复的恢复证书。 这与用于加密文件系统 (EFS) 的数据恢复代理 (DRA) 证书相同。|
|revokeOnUnenrollDisabled|Boolean|此策略控制设备从管理服务中取消注册时是否撤销 WIP 密钥。 如果设置为 1（不撤销密钥），则不会撤销密钥，并且用户在取消注册后可继续访问受保护的文件。 如果未撤销密钥，随后将不会撤销文件清除。|
|rightsManagementServicesTemplateId|Guid|用于 RMS 加密的 TemplateID GUID。 RMS 模板允许 IT 管理员配置有关谁有权访问受 RMS 保护的文件以及他们可以访问多长时间的详细信息。|
|azureRightsManagementServicesAllowed|Boolean|指定是否允许 Azure RMS 加密用于 WIP。|
|iconsVisible|Boolean|确定是否在“开始”菜单的资源管理器和仅企业应用磁贴中向受 WIP 保护的文件的图标添加覆盖图。 从 Windows 10 版本 1703 开始，此设置还配置 WIP 图标在受 WIP 保护的应用的标题栏中的可见性|
|protectedApps|[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合|受保护的应用程序可以访问企业数据，并且由这些应用程序处理的数据受加密保护|
|exemptApps|[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 集合|豁免应用程序还可以访问企业数据，但由这些应用程序处理的数据不受保护。 这是因为一些关键的企业应用程序可能与加密数据存在兼容性问题。|
|enterpriseNetworkDomainNames|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合|这是构成企业边界的域列表。 发送到某设备的来自这些域之一的数据将被视为企业数据并受到保护。这些位置将被视为共享企业数据的安全目标。|
|enterpriseProxiedDomains|[windowsInformationProtectionProxiedDomainCollection](../resources/intune-mam-windowsinformationprotectionproxieddomaincollection.md) 集合|包含需要保护的托管在云中的企业资源域列表。 与这些资源的连接被视为企业数据。 如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。 用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。|
|enterpriseIPRanges|[windowsInformationProtectionIPRangeCollection](../resources/intune-mam-windowsinformationprotectioniprangecollection.md) 集合|设置定义企业网络中计算机的企业 IP 范围。 来自这些计算机的数据将被视为企业的一部分并受保护。 这些位置将被视为共享企业数据的安全目标|
|enterpriseIPRangesAreAuthoritative|Boolean|用于通知客户端接受已配置的列表，并且不使用试探法来尝试查找其他子网的布尔值。 默认值为 false|
|enterpriseProxyServers|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合|这是代理服务器的列表。 任何不在此列表中的服务器都被视为非企业服务器|
|enterpriseInternalProxyServers|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合|这是逗号分隔的内部代理服务器列表。 例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。 这些代理已由管理员配置为连接到 Internet 上的特定资源。 它们被视为是企业版网络位置。 代理仅在配置 EnterpriseProxiedDomains 策略时利用以强制流量通过这些代理传输到匹配的域|
|enterpriseProxyServersAreAuthoritative|Boolean|用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。 默认值为 false|
|neutralDomainResources|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合|可用于工作或个人资源的域名列表|
|indexingEncryptedStoresOrItemsBlocked|Boolean|此开关用于 Windows Search 索引器，以允许或禁止建立项目索引|
|smbAutoEncryptedFileExtensions|[windowsInformationProtectionResourceCollection](../resources/intune-mam-windowsinformationprotectionresourcecollection.md) 集合|指定文件扩展名列表，以便从公司边界内的 SMB 共享复制时加密具有这些扩展名的文件|
|isAssigned|Boolean|指示策略是否部署到任何包含组。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|protectedAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合|通过 xml 文件输入受保护应用的另一种方法|
|exemptAppLockerFiles|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合|通过 xml 文件输入豁免应用的另一种方法|
|assignments|[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 集合|针对策略的安全组列表的导航属性。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
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
  "rightsManagementServicesTemplateId": "Guid",
  "azureRightsManagementServicesAllowed": true,
  "iconsVisible": true,
  "protectedApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
      "displayName": "String",
      "description": "String",
      "publisherName": "String",
      "productName": "String",
      "denied": true
    }
  ],
  "exemptApps": [
    {
      "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
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
          "@odata.type": "microsoft.graph.ipRange"
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
  "isAssigned": true
}
```




