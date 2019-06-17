---
title: 创建 intuneBrandingProfile
description: 创建新的 intuneBrandingProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec5e863d171c952c07acfb0ecf2c312dcd89a366
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990664"
---
# <a name="create-intunebrandingprofile"></a>创建 intuneBrandingProfile

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

创建新的[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

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
在请求正文中, 提供 intuneBrandingProfile 对象的 JSON 表示形式。

下表显示创建 intuneBrandingProfile 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|配置文件键|
|profileName|String|配置文件的名称|
|profileDescription|String|配置文件的说明|
|isDefaultProfile|Boolean|一个 Boolean 类型的值, 该值表示是否将配置文件用作默认配置文件|
|createdDateTime|DateTimeOffset|创建 BrandingProfile 的时间|
|lastModifiedDateTime|DateTimeOffset|上次修改 BrandingProfile 的时间|
|displayName|字符串|向最终用户显示的公司/组织名称|
|contactITName|String|负责 IT 支持的人员/组织的名称|
|contactITPhoneNumber|String|负责 IT 支持的个人/组织的电话号码|
|contactITEmailAddress|String|负责 IT 支持的个人/组织的电子邮件地址|
|contactITNotes|String|关于负责 IT 支持的人员/组织的文本注释|
|privacyUrl|String|指向公司/组织的隐私策略的 URL|
|onlineSupportSiteUrl|String|指向公司/组织的 IT 支持人员网站的 URL|
|onlineSupportSiteName|String|公司/组织的 IT 支持人员网站的显示名称|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|公司门户应用程序和 web 门户中使用的主要主题颜色|
|showLogo|Boolean|Boolean 类型的值, 该值表示是否显示管理员提供的徽标图像|
|showDisplayNameNextToLogo|布尔值|一个 Boolean 类型的值, 该值表示是否在徽标图像旁边显示管理员提供的显示名称|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|在公司门户应用程序中显示的徽标图像, 其徽标后面有主题颜色背景|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|在公司门户应用程序中显示的徽标图像, 徽标后面有浅背景|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|在公司门户应用登录页中显示的自定义图像|
|customPrivacyMessage|String|有关管理员在设备上有权访问的内容的文本注释|



## <a name="response"></a>响应
如果成功, 此方法在响应`201 Created`正文中返回响应代码和[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1264

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
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
  "customPrivacyMessage": "Custom Privacy Message value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1436

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
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
  "customPrivacyMessage": "Custom Privacy Message value"
}
```





