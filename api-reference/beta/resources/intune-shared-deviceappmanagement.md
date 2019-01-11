---
title: deviceAppManagement 资源类型
description: 充当所有设备应用管理功能的容器的单例实体。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7be07f04c33dcb81ab0dfe350290fa95fb8c1679
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885104"
---
# <a name="deviceappmanagement-resource-type"></a>deviceAppManagement 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

充当所有设备应用管理功能的容器的单例实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceAppManagement](../api/intune-shared-deviceappmanagement-get.md)|读取 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性和关系。|
|[更新 deviceAppManagement](../api/intune-shared-deviceappmanagement-update.md)|更新 [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 对象的属性。|
|**入职培训**|
|[syncMicrosoftStoreForBusinessApps 操作](../api/intune-shared-deviceappmanagement-syncmicrosoftstoreforbusinessapps.md)|无|将 Intune 帐户与适用于企业的 Microsoft Store 同步|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|**入职培训**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|帐户是否已启用从适用于企业的 Microsoft Store 同步应用程序。|
|microsoftStoreForBusinessLanguage|String|用于从适用于企业的 Microsoft Store 同步应用程序的区域设置信息。 特定于国家/地区的区域性。 这些区域性的名称遵循 RFC 4646（Windows Vista 和更高版本）。 格式为 <languagecode2>-<country/regioncode2>，其中 <languagecode2> 是从 ISO 639-1 派生的两个小写字母组成的代码，<country/regioncode2> 是从 ISO 3166 派生的两个大写字母组成的代码。 例如，“en-US”（“英语(美国)）是一个特定的区域性。|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|从适用于企业的 Microsoft Store 的应用程序同步上次完成的时间。|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|适用于企业的 Microsoft Store 的应用上次成功同步帐户的时间。|
|microsoftStoreForBusinessPortalSelection|[microsoftStoreForBusinessPortalSelectionOptions](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|最终用户门户信息用于同步 Intune 的公司门户从 Microsoft 存储的业务应用程序。 有三个选项，可以从中进行选取\[公司仅门户、 公司门户和专用存储、 仅专用存储\]。 可取值为：`none`、`companyPortal`、`privateStore`。|

## <a name="relationships"></a>Relationships
|关系|类型|Description|
|:---|:---|:---|
|**应用程序**|
|enterpriseCodeSigningCertificates|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)集合|Windows 企业代码签名证书。|
|iosLobAppProvisioningConfigurations|[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)集合|IOS Lob 应用程序设置配置。|
|mobileAppCategories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|移动应用类别。|
|mobileAppConfigurations|[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) 集合|托管设备移动应用程序配置。|
|mobileApps|[mobileApp](../resources/intune-apps-mobileapp.md) 集合|移动应用。|
|symantecCodeSigningCertificate|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|WinPhone Symantec 代码签名证书。|
|**书籍**|
|managedEBooks|[managedEBook](../resources/intune-books-managedebook.md) 集合|托管的电子书。|
|managedEBookCategories|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)集合|移动电子图书类别。|
|**设备管理**|
|windowsManagementApp|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|Windows 管理应用程序。|
|**移动应用程序管理 (MAM)**|
|androidManagedAppProtections|[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) 集合|Android 托管应用策略。|
|defaultManagedAppProtections|[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 集合|默认的托管应用策略。|
|iosManagedAppProtections|[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) 集合|iOS 托管应用策略。|
|managedAppPolicies|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合|托管应用策略。|
|managedAppRegistrations|[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合|托管应用注册。|
|managedAppStatuses|[managedAppStatus](../resources/intune-mam-managedappstatus.md) 集合|托管应用状态。|
|mdmWindowsInformationProtectionPolicies|[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 集合|对已注册 MDM 的设备上运行的应用的 Windows 信息保护。|
|targetedManagedAppConfigurations|[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) 集合|托管应用配置目标。|
|windowsInformationProtectionPolicies|[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 集合|对未注册 MDM 的设备上运行的应用的 Windows 信息保护。|
|**入职培训**|
|sideLoadingKeys|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)集合|端加载所需的 Windows 8 和 8.1 应用程序安装的键。|
|vppTokens|[vppToken](../resources/intune-onboarding-vpptoken.md) 集合|此组织的 Vpp 令牌列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。  请注意，这只是一个示例;实际查询的查询响应将包含相应的上下文的属性。  
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



