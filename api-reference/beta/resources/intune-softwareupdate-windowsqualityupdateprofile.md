---
title: windowsQualityUpdateProfile 资源类型
description: Windows质量更新配置文件
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 090f22169255049482cd561ef509fb6d7aba8f8deca5699873e2c14e0f200e43
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54224311"
---
# <a name="windowsqualityupdateprofile-resource-type"></a>windowsQualityUpdateProfile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows质量更新配置文件

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsQualityUpdateProfiles](../api/intune-softwareupdate-windowsqualityupdateprofile-list.md)|[windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) 集合|列出 [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) 对象的属性和关系。|
|[获取 windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-get.md)|[windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|读取 [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) 对象的属性和关系。|
|[创建 windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-create.md)|[windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|创建新的 [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) 对象。|
|[删除 windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-delete.md)|无|删除 [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)。|
|[更新 windowsQualityUpdateProfile](../api/intune-softwareupdate-windowsqualityupdateprofile-update.md)|[windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)|更新 [windowsQualityUpdateProfile 对象](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) 的属性。|
|[分配操作](../api/intune-softwareupdate-windowsqualityupdateprofile-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|Intune 策略 ID。|
|displayName|String|配置文件显示名称的配置文件。|
|description|String|由用户指定的配置文件的说明。|
|expeditedUpdateSettings|[expeditedWindowsQualityUpdateSettings](../resources/intune-softwareupdate-expeditedwindowsqualityupdatesettings.md)|加速更新设置。|
|createdDateTime|DateTimeOffset|创建配置文件的日期时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改配置文件的日期时间。|
|roleScopeTagIds|String collection|此质量更新实体的范围标记列表。|
|releaseDateDisplayName|字符串|为质量更新版本显示的友好发布日期|
|deployableContentDisplayName|String|质量显示名称配置文件可部署内容的友好解决方案|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) 集合|配置文件的组分配列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsQualityUpdateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "expeditedUpdateSettings": {
    "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings",
    "qualityUpdateRelease": "String",
    "daysUntilForcedReboot": 1024
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "releaseDateDisplayName": "String",
  "deployableContentDisplayName": "String"
}
```




