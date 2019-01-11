---
title: officeSuiteApp 资源类型
description: Office365 套件应用程序中包含的属性和继承的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 65ba9d39b2648ecf47e66c3b907eee50c57e906b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820557"
---
# <a name="officesuiteapp-resource-type"></a>officeSuiteApp 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Office365 套件应用程序中包含的属性和继承的属性。

继承自 [mobileApp](../resources/intune-apps-mobileapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 officeSuiteApps](../api/intune-apps-officesuiteapp-list.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)集合|列出属性和[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象之间的关系。|
|[获取 officeSuiteApp](../api/intune-apps-officesuiteapp-get.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|读取属性和[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象的关系。|
|[创建 officeSuiteApp](../api/intune-apps-officesuiteapp-create.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|创建新的[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象。|
|[删除 officeSuiteApp](../api/intune-apps-officesuiteapp-delete.md)|无|删除[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)。|
|[更新 officeSuiteApp](../api/intune-apps-officesuiteapp-update.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|更新[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象的属性。|

## <a name="properties"></a>属性
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
|autoAcceptEula|布尔|要接受 EULA 自动在最终用户的设备上的值。|
|productIds|[officeProductId](../resources/intune-apps-officeproductid.md)集合|表示 Office365 套件 SKU 产品 Id。|
|excludedApps|[excludedApps](../resources/intune-apps-excludedapps.md)|该属性表示的应用程序即排除从所选 Office365 产品 id。|
|useSharedComputerActivation|布尔|是否在共享的计算机激活不用于 Office365 应用程序套件表示的属性。|
|updateChannel|[officeUpdateChannel](../resources/intune-apps-officeupdatechannel.md)|表示 Office365 更新频道属性。 可取值为：`none`、`current`、`deferred`、`firstReleaseCurrent`、`firstReleaseDeferred`。|
|officePlatformArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|要代表 Office365 应用程序套件版本的属性。 可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。|
|localesToInstall|String 集合|表示安装的区域设置的属性中 Office365 应用程序在安装时。 它使用标准 RFC 6033。 参考：https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx|
|installProgressDisplayLevel|[officeSuiteInstallProgressDisplayLevel](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|若要指定在设备上显示安装进度安装程序 UI 的级别。 可取值为：`none`、`full`。|
|shouldUninstallOlderVersionsOfOffice|布尔|要确定是否如果 Office365 应用程序套件部署到设备，或不卸载现有 Office MSI 的属性。|
|targetVersion|字符串|要代表应保持在设备上部署的 Office365 应用程序套件的特定目标版本的属性。|
|updateVersion|字符串|要代表特定目标版本处于可供 Office365 应用程序套件的更新版本的属性。|

## <a name="relationships"></a>Relationships
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|移动应用安装摘要。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合|此移动应用程序的安装状态的列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)集合|此移动应用程序的安装状态的列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeSuiteApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": 1024,
  "publishingState": "String",
  "autoAcceptEula": true,
  "productIds": [
    "String"
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
  "updateChannel": "String",
  "officePlatformArchitecture": "String",
  "localesToInstall": [
    "String"
  ],
  "installProgressDisplayLevel": "String",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "String",
  "updateVersion": "String"
}
```





