---
title: officeSuiteApp 资源类型
description: 包含 Office365 套件应用程序的属性和继承的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1bef472078781b63173deb7896946590a5d9e129
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335849"
---
# <a name="officesuiteapp-resource-type"></a>officeSuiteApp 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含 Office365 套件应用程序的属性和继承的属性。


继承自 [mobileApp](../resources/intune-apps-mobileapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 officeSuiteApps](../api/intune-apps-officesuiteapp-list.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)集合|列出[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象的属性和关系。|
|[获取 officeSuiteApp](../api/intune-apps-officesuiteapp-get.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|读取[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象的属性和关系。|
|[创建 officeSuiteApp](../api/intune-apps-officesuiteapp-create.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|创建新的[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象。|
|[删除 officeSuiteApp](../api/intune-apps-officesuiteapp-delete.md)|无|删除[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)。|
|[更新 officeSuiteApp](../api/intune-apps-officesuiteapp-update.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|更新[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|String|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|说明|字符串|应用的说明。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|publisher|String|应用的发布者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|要显示在应用详细信息中并用于图标上传的大图标。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|String|隐私声明 URL。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|informationUrl|String|详细信息 URL。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|String|应用的所有者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|应用的开发者。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|notes|String|应用的备注。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|uploadState|Int32|上载状态。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|应用的发布状态。 除非应用已发布，否则无法分配应用。 继承自[mobileApp](../resources/intune-apps-mobileapp.md)。 可取值为：`notPublished`、`processing`、`published`。|
|isAssigned|Boolean|指示是否至少向一个组分配了应用程序的值。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|roleScopeTagIds|String collection|此移动应用的作用域标记 id 列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|dependentAppCount|Int32|子应用程序的依赖项总数。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|autoAcceptEula|Boolean|要在 enduser 的设备上自动接受 EULA 的值。|
|productIds|[officeProductId](../resources/intune-apps-officeproductid.md)集合|表示 Office365 套件 SKU 的产品 Id。|
|excludedApps|[excludedApps](../resources/intune-apps-excludedapps.md)|表示从所选 Office365 产品 Id 中排除的应用程序的属性。|
|useSharedComputerActivation|Boolean|表示共享计算机激活是否不适用于 Office365 应用程序套件的属性。|
|updateChannel|[officeUpdateChannel](../resources/intune-apps-officeupdatechannel.md)|用于表示 Office365 更新通道的属性。 可取值为：`none`、`current`、`deferred`、`firstReleaseCurrent`、`firstReleaseDeferred`。|
|officePlatformArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|表示 Office365 应用程序套件版本的属性。 可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。|
|localesToInstall|String collection|用于表示安装 Office365 中的应用程序时所安装的区域设置的属性。 它使用标准 RFC 6033。 Refhttps://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx|
|installProgressDisplayLevel|[officeSuiteInstallProgressDisplayLevel](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|指定设备上安装进度设置 UI 的显示级别。 可取值为：`none`、`full`。|
|shouldUninstallOlderVersionsOfOffice|Boolean|用于确定是否在将 Office365 应用套件部署到设备时是否卸载现有 Office MSI 的属性。|
|targetVersion|String|表示应在设备上保持部署的 Office365 应用程序套件的特定目标版本的属性。|
|updateVersion|String|表示可用于 Office365 应用程序套件的特定目标版本的更新版本的属性。|
|officeConfigurationXml|Binary|表示可为 Office 专业增强版应用程序指定的 XML 配置文件的属性。 优先于所有其他属性。 如果存在, 将使用 XML 配置文件来创建应用程序。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|移动应用安装摘要。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合|此移动应用程序的安装状态列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|userStatuses|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)集合|此移动应用程序的安装状态列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|
|相互|[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)集合|此移动应用的关系列表。 继承自 [mobileApp](../resources/intune-apps-mobileapp.md)|

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024,
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
    "teams": true,
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
  "updateVersion": "String",
  "officeConfigurationXml": "binary"
}
```



