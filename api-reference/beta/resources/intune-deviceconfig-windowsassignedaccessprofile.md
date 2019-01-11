---
title: windowsAssignedAccessProfile 资源类型
description: 用于 Windows 的分配的访问配置文件。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 93f71952c45f4fd8bbd397f0ea115abbe3faafac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890606"
---
# <a name="windowsassignedaccessprofile-resource-type"></a>windowsAssignedAccessProfile 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

用于 Windows 的分配的访问配置文件。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 windowsAssignedAccessProfiles](../api/intune-deviceconfig-windowsassignedaccessprofile-list.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)集合|列出属性和[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)对象之间的关系。|
|[获取 windowsAssignedAccessProfile](../api/intune-deviceconfig-windowsassignedaccessprofile-get.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|读取属性和[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)对象的关系。|
|[创建 windowsAssignedAccessProfile](../api/intune-deviceconfig-windowsassignedaccessprofile-create.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|创建新的[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)对象。|
|[删除 windowsAssignedAccessProfile](../api/intune-deviceconfig-windowsassignedaccessprofile-delete.md)|无|删除[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)。|
|[更新 windowsAssignedAccessProfile](../api/intune-deviceconfig-windowsassignedaccessprofile-update.md)|[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|更新[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|profileName|字符串|这是用于标识一组应用程序，在开始菜单和用户为其分配此网亭配置这些应用程序的布局的友好名称。|
|showTaskBar|布尔|此设置，管理员可以指定任务条形图或不所示。|
|appUserModelIds|String 集合|这些是唯一的 Windows 应用商店应用程序将可以从开始菜单启动。|
|desktopAppPaths|String 集合|在开始菜单可用桌面应用程序的路径和仅应用程序用户都将能够启动。|
|用户帐户|String 集合|将锁定到此网亭配置用户帐户。|
|startMenuLayoutXml|Binary|允许管理员可以重写默认开始布局，并禁止用户更改它。通过基于布局修改模式指定 XML 文件来修改布局。 XML 需要以二进制格式。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAssignedAccessProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "id": "String (identifier)",
  "profileName": "String",
  "showTaskBar": true,
  "appUserModelIds": [
    "String"
  ],
  "desktopAppPaths": [
    "String"
  ],
  "userAccounts": [
    "String"
  ],
  "startMenuLayoutXml": "binary"
}
```





