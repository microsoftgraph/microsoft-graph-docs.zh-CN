---
title: 更新 officeSuiteApp
description: 更新 officeSuiteApp 对象的属性。
ms.openlocfilehash: b98a7da8d268894adce8c9f5bb9790c924e8b64c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042738"
---
# <a name="update-officesuiteapp"></a>更新 officeSuiteApp

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象的属性。
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
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象的 JSON 表示形式。

下表显示时创建[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|String|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|description|String|应用的说明。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|publisher|String|应用的发布者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|要显示在应用详细信息中并用于图标上传的大图标。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|String|隐私声明 Url。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|informationUrl|String|详细信息 Url。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|String|应用的所有者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|应用的开发者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|notes|String|应用的备注。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|uploadState|Int32|上载状态。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|应用的发布状态。 除非应用已发布，否则无法分配应用。 继承自[mobileApp](../resources/intune-apps-mobileapp.md)。 可取值为：`notPublished`、`processing`、`published`。|
|autoAcceptEula|布尔值|要接受 EULA 自动在最终用户的设备上的值。|
|productIds|[officeProductId](../resources/intune-apps-officeproductid.md)集合|表示 Office365 套件 SKU 产品 Id。 可取值为：`o365ProPlusRetail`、`o365BusinessRetail`、`visioProRetail`、`projectProRetail`。|
|excludedApps|[excludedApps](../resources/intune-apps-excludedapps.md)|该属性表示的应用程序即排除从所选 Office365 产品 id。|
|useSharedComputerActivation|布尔值|是否在共享的计算机激活不用于 Office365 应用程序套件表示的属性。|
|updateChannel|[officeUpdateChannel](../resources/intune-apps-officeupdatechannel.md)|表示 Office365 更新频道属性。 可取值为：`none`、`current`、`deferred`、`firstReleaseCurrent`、`firstReleaseDeferred`。|
|officePlatformArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|要代表 Office365 应用程序套件版本的属性。 可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。|
|localesToInstall|String 集合|表示安装的区域设置的属性中 Office365 应用程序在安装时。 它使用标准 RFC 6033。 参考：https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx|
|installProgressDisplayLevel|[officeSuiteInstallProgressDisplayLevel](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|若要指定在设备上显示安装进度安装程序 UI 的级别。 可取值为：`none`、`full`。|
|shouldUninstallOlderVersionsOfOffice|布尔值|要确定是否如果 Office365 应用程序套件部署到设备，或不卸载现有 Office MSI 的属性。|
|targetVersion|字符串|要代表应保持在设备上部署的 Office365 应用程序套件的特定目标版本的属性。|
|updateVersion|字符串|要代表特定目标版本处于可供 Office365 应用程序套件的更新版本的属性。|



## <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1413

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "id": "9b263b46-3b46-9b26-463b-269b463b269b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value"
}
```





