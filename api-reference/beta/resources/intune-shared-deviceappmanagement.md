---
title: deviceAppManagement 资源类型
description: 充当所有设备应用管理功能的容器的单例实体。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 12394a2335968bfe06ea3ce5e35161c1c100615893cd1597a1249e1151d7e756
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54219757"
---
# <a name="deviceappmanagement-resource-type"></a>deviceAppManagement 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

充当所有设备应用管理功能的容器的单例实体。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceAppManagement](../api/intune-shared-deviceappmanagement-get.md)|读取 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性和关系。|
|[更新 deviceAppManagement](../api/intune-shared-deviceappmanagement-update.md)|更新 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性。|
|**载入**|
|[syncMicrosoftStoreForBusinessApps 操作](../api/intune-shared-deviceappmanagement-syncmicrosoftstoreforbusinessapps.md)|无|将 Intune 帐户与适用于企业的 Microsoft Store 同步|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|**载入**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|帐户是否已启用从适用于企业的 Microsoft Store 同步应用程序。|
|microsoftStoreForBusinessLanguage|String|用于从适用于企业的 Microsoft Store 同步应用程序的区域设置信息。 特定于国家/地区的区域性。 这些区域性的名称遵循 RFC 4646（Windows Vista 和更高版本）。 格式为 <languagecode2>-<country/regioncode2>，其中 <languagecode2> 是从 ISO 639-1 派生的两个小写字母组成的代码，<country/regioncode2> 是从 ISO 3166 派生的两个大写字母组成的代码。 例如，“en-US”（“英语(美国)）是一个特定的区域性。|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|上次完成从适用于企业的 Microsoft Store 的应用程序同步的时间。|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|适用于企业的 Microsoft Store 的应用上次成功同步帐户的时间。|
|microsoftStoreForBusinessPortalSelection|[microsoftStoreForBusinessPortalSelectionOptions](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|最终用户门户信息用于将应用程序从 适用于企业的 Microsoft Store 同步到Intune 公司门户。 有三个选项可供选择：仅公司门户、公司门户和专用应用商店、仅 \[ 专用应用商店 \] 。 可取值为：`none`、`companyPortal`、`privateStore`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|**应用**|
|enterpriseCodeSigningCertificates|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) 集合|代码Windows Enterprise证书。|
|iosLobAppProvisioningConfigurations|[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 集合|IOS Lob 应用预配配置。|
|mobileAppCategories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|移动应用类别。|
|mobileAppConfigurations|[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 集合|托管设备移动应用程序配置。|
|mobileApps|[mobileApp](../resources/intune-shared-mobileapp.md) 集合|移动应用。|
|symantecCodeSigningCertificate|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|WinPhone Symantec 代码签名证书。|
|**书籍**|
|managedEBooks|[managedEBook](../resources/intune-books-managedebook.md) 集合|托管的电子书。|
|managedEBookCategories|[managedEBookCategory](../resources/intune-books-managedebookcategory.md) 集合|移动电子书类别。|
|**设备管理**|
|windowsManagementApp|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Windows管理应用。|
|**移动应用管理(MAM)**|
|androidManagedAppProtections|[androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) 集合|Android 托管应用策略。|
|defaultManagedAppProtections|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 集合|默认的托管应用策略。|
|iosManagedAppProtections|[iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) 集合|iOS 托管应用策略。|
|managedAppPolicies|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合|托管应用策略。|
|managedAppRegistrations|[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合|托管应用注册。|
|managedAppStatuses|[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合|托管应用状态。|
|mdmWindowsInformationProtectionPolicies|[mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) 集合|对已注册 MDM 的设备上运行的应用的 Windows 信息保护。|
|targetedManagedAppConfigurations|[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 集合|托管应用配置目标。|
|windowsInformationProtectionPolicies|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 集合|对未注册 MDM 的设备上运行的应用的 Windows 信息保护。|
|**载入**|
|sideLoadingKeys|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 集合|旁加载安装和 8.1 应用Windows 8所需的密钥。|
|vppTokens|[vppToken](../resources/intune-onboarding-vpptoken.md) 集合|此组织的 Vpp 令牌列表。|
|**策略集**|
|policySets|[policySet](../resources/intune-policyset-policyset.md) 集合|策略和应用程序的策略集|
|mobileApps|[mobileApp](../resources/intune-shared-mobileapp.md) 集合|移动应用。|
|targetedManagedAppConfigurations|[targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 集合|托管应用配置目标。|
|androidManagedAppProtections|[androidManagedAppProtection](../resources/intune-shared-androidmanagedappprotection.md) 集合|Android 托管应用策略。|
|iosManagedAppProtections|[iosManagedAppProtection](../resources/intune-shared-iosmanagedappprotection.md) 集合|iOS 托管应用策略。|
|mdmWindowsInformationProtectionPolicies|[mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) 集合|对已注册 MDM 的设备上运行的应用的 Windows 信息保护。|
|iosLobAppProvisioningConfigurations|[iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 集合|IOS Lob 应用预配配置。|
|**合作伙伴集成**|
|deviceAppManagementTasks|[deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) 集合|设备应用管理任务。|
|**Unlock**|
|wdacSupplementalPolicies|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) 集合|应用程序控制Windows Defender策略的集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。  请注意，这仅仅是一个示例;对实际查询的查询响应将包含适用于上下文的属性。  
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "String (timestamp)",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "String",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "String (timestamp)"
}
```




