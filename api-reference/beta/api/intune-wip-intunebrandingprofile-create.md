---
title: 创建 intuneBrandingProfile
description: 创建新的 intuneBrandingProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b75c9ae8d755b74eb16049570382c123315e606fc26b00f3d9badb8f91c7f37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54158494"
---
# <a name="create-intunebrandingprofile"></a>创建 intuneBrandingProfile

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的 [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) 对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 intuneBrandingProfile 对象的 JSON 表示形式。

下表显示创建 intuneBrandingProfile 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|配置文件密钥|
|profileName|字符串|配置文件的名称|
|profileDescription|String|配置文件的说明|
|isDefaultProfile|布尔值|表示配置文件是否用作默认配置文件的布尔值|
|createdDateTime|DateTimeOffset|BrandingProfile 创建时间|
|lastModifiedDateTime|DateTimeOffset|BrandingProfile 上次修改的时间|
|displayName|字符串|向最终用户显示的公司/组织名称|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|应用程序应用程序和 Web 门户公司门户主题颜色|
|showLogo|布尔值|表示是否显示管理员提供的徽标图像的布尔值|
|showDisplayNameNextToLogo|布尔值|Boolean 值，表示是否显示名称徽标图像旁边显示管理员提供的图像|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|徽标显示在徽标公司门户具有主题颜色背景的应用中显示的徽标图像|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|徽标在徽标公司门户背景浅色的应用中显示的徽标图像|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|自定义图像显示在应用公司门户页面中|
|contactITName|String|负责 IT 支持人员/组织的名称|
|contactITPhoneNumber|String|电话 IT 支持人员/组织的数量|
|contactITEmailAddress|String|负责 IT 支持的人/组织的电子邮件地址|
|contactITNotes|String|有关负责 IT 支持的人/组织的文本注释|
|onlineSupportSiteUrl|String|指向公司/组织的 IT 支持人员网站的 URL|
|onlineSupportSiteName|String|公司/组织的 IT 支持人员网站的显示名称|
|privacyUrl|String|指向公司/组织隐私策略的 URL|
|customPrivacyMessage|String|有关管理员在设备上无法访问的内容的文本注释|
|customCanSeePrivacyMessage|字符串|有关管理员在设备上有权访问的内容的文本注释|
|customCantSeePrivacyMessage|字符串|有关管理员在设备上无法访问的内容的文本注释|
|isRemoveDeviceDisabled|布尔值|Boolean 值，表示 adminsistrator 是否已在公司拥有的设备上禁用"删除设备"操作。|
|isFactoryResetDisabled|布尔值|Boolean 值，表示 adminsistrator 是否已在公司拥有的设备上禁用"恢复出厂设置"操作。|
|companyPortalBlockedActions|[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) 集合|根据平台和设备所有权类型，在公司门户上阻止的操作的集合。|
|showAzureADEnterpriseApps|布尔值|Boolean 值，指示 AzureAD Enterprise应用是否将显示在 公司门户|
|showOfficeWebApps|布尔值|Boolean 值，Office WebApps 是否将显示在公司门户|
|sendDeviceOwnershipChangePushNotification|布尔值|指示当用户的设备所有权类型从个人更改到公司时是否向用户发送推送通知的布尔值|
|enrollmentAvailability|[enrollmentAvailabilityOptions](../resources/intune-shared-enrollmentavailabilityoptions.md)|向最终用户显示的自定义设备注册流。 可取值为：`availableWithPrompts`、`availableWithoutPrompts`、`unavailable`。|
|disableClientTelemetry|布尔值|适用于从所有客户端发送到 Intune 服务的遥测。 禁用后，将关闭客户端内的所有主动故障排除和发出警告，并且遥测设置对设备用户显示为非活动或隐藏。|
|roleScopeTagIds|String collection|分配给品牌配置文件的范围标记列表|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1975

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "displayName": "Display Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "customPrivacyMessage": "Custom Privacy Message value",
  "customCanSeePrivacyMessage": "Custom Can See Privacy Message value",
  "customCantSeePrivacyMessage": "Custom Cant See Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "androidForWork",
      "ownerType": "company",
      "action": "remove"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "availableWithoutPrompts",
  "disableClientTelemetry": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2147

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "customPrivacyMessage": "Custom Privacy Message value",
  "customCanSeePrivacyMessage": "Custom Can See Privacy Message value",
  "customCantSeePrivacyMessage": "Custom Cant See Privacy Message value",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "androidForWork",
      "ownerType": "company",
      "action": "remove"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "availableWithoutPrompts",
  "disableClientTelemetry": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




