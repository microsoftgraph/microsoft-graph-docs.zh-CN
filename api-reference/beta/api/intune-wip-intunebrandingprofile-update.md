---
title: 更新 intuneBrandingProfile
description: 更新 intuneBrandingProfile 对象的属性。
author: tfitzmac
ms.openlocfilehash: c4321b0197e30126c4d83371a31425af1d8e73bd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309945"
---
# <a name="update-intunebrandingprofile"></a>更新 intuneBrandingProfile

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的属性。
## <a name="prerequisites"></a>先决条件
需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。


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
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象的 JSON 表示形式。

下表显示时创建[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|配置文件密钥|
|profileName|字符串|配置文件的名称|
|profileDescription|字符串|配置文件的说明|
|isDefaultProfile|Boolean|如果在配置文件使用的默认，呈现。|
|createdDateTime|DateTimeOffset|创建 BrandingProfile 时。|
|lastModifiedDateTime|DateTimeOffset|当 BrandingProfile 上次修改。|
|displayName|String|向最终用户显示的公司/组织名称。|
|contactITName|String|负责 IT 支持的员工/组织名称。|
|contactITPhoneNumber|String|负责 IT 支持的员工/组织的电话号码。|
|contactITEmailAddress|String|负责 IT 支持的员工/组织的电子邮件地址。|
|contactITNotes|String|负责 IT 支持的员工/组织的文本注释。|
|privacyUrl|String|指向公司/组织隐私策略的 URL。|
|onlineSupportSiteUrl|String|指向公司/组织 IT 支持人员网站的 URL。|
|onlineSupportSiteName|String|显示公司/组织 IT 支持人员网站的名称。|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|公司门户应用程序和 Web 门户中使用的主要主题颜色。|
|showLogo|布尔值|表示是否显示管理员提供的徽标图像的布尔值。|
|showDisplayNameNextToLogo|布尔值|表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|主题颜色背景上的公司门户应用程序中显示的徽标图像。|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|浅色背景上的公司门户应用程序中显示的徽标图像。|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|自定义登录页的公司门户应用程序中显示的图像|



## <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1209

{
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
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
  }
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1377

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
  }
}
```





