---
title: windowsKioskConfiguration 资源类型
description: 此实体提供了属性、 网亭资源由公开的关系的声明方法的说明。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f091d9700721a1be1baf5982b0fb8ce0fe3b00ec
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403957"
---
# <a name="windowskioskconfiguration-resource-type"></a>windowsKioskConfiguration 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

此实体提供了属性、 网亭资源由公开的关系的声明方法的说明。


继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 windowsKioskConfigurations](../api/intune-deviceconfig-windowskioskconfiguration-list.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)集合|列出属性和[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象之间的关系。|
|[获取 windowsKioskConfiguration](../api/intune-deviceconfig-windowskioskconfiguration-get.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)|读取属性和[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的关系。|
|[创建 windowsKioskConfiguration](../api/intune-deviceconfig-windowskioskconfiguration-create.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)|创建新的[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象。|
|[删除 windowsKioskConfiguration](../api/intune-deviceconfig-windowskioskconfiguration-delete.md)|无|删除[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)。|
|[更新 windowsKioskConfiguration](../api/intune-deviceconfig-windowskioskconfiguration-update.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)|更新[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String 集合|此实体实例范围标记的列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|指示基础的设备配置支持分配的范围标记。 此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。 这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。 此属性是只读的。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|kioskProfiles|[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)集合|此策略设置允许定义网亭配置网亭配置文件的列表。 此集合可以包含 3 个元素的最大值。|
|kioskBrowserDefaultUrl|String|在启动上指定浏览器应导航到的默认 URL。|
|kioskBrowserEnableHomeButton|Boolean|启用网亭浏览器的主页按钮。 默认情况下禁用主页按钮。|
|kioskBrowserEnableNavigationButtons|Boolean|启用网亭浏览器的导航 buttons(forward/back)。 默认情况下，禁用导航按钮。|
|kioskBrowserEnableEndSessionButton|Boolean|启用网亭浏览器的结束会话按钮。 默认情况下禁用结束会话按钮。|
|kioskBrowserRestartOnIdleTimeInMinutes|Int32|指定网亭浏览器中刷新状态重新启动之前，会话处于空闲状态的分钟数。  有效值为 1 1440年。 1 到 1440 之间的有效值|
|kioskBrowserBlockedURLs|String 集合|指定网亭浏览器不应导航到的 Url|
|kioskBrowserBlockedUrlExceptions|String 集合|指定允许网亭浏览器导航到的 Url|
|edgeKioskEnablePublicBrowsing|Boolean|启用 Microsoft 边缘浏览器的公共浏览展台模式。 默认值为 false。|
|edgeKioskResetAfterIdleTimeInMinutes|Int32|Microsoft 边缘网亭重置之前，请以分钟为单位的最后一个用户活动从指定的时间。  有效值为 0 1440年。 默认值为 5。 0 指示不重置。 0 到 1440 之间的有效值|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)集合|设备配置文件的组分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) 集合|用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsKioskConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "String",
      "profileName": "String",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "String",
            "name": "String",
            "appType": "String",
            "appUserModelId": "String",
            "appId": "String",
            "containedAppId": "String"
          }
        ],
        "showTaskBar": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "binary"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "String",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 1024,
  "kioskBrowserBlockedURLs": [
    "String"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "String"
  ],
  "edgeKioskEnablePublicBrowsing": true,
  "edgeKioskResetAfterIdleTimeInMinutes": 1024
}
```




