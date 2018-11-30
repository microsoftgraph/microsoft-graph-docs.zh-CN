---
title: userAppInstallStatus 资源类型
description: 包含用户的安装状态属性。
ms.openlocfilehash: 06d9be7bc6d5aa72bde80802b5f6bb282dc5707c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047760"
---
# <a name="userappinstallstatus-resource-type"></a>userAppInstallStatus 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含用户的安装状态属性。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 userAppInstallStatuses](../api/intune-apps-userappinstallstatus-list.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)集合|列出属性和[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象之间的关系。|
|[获取 userAppInstallStatus](../api/intune-apps-userappinstallstatus-get.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|读取属性和[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的关系。|
|[创建 userAppInstallStatus](../api/intune-apps-userappinstallstatus-create.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|创建新的[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象。|
|[删除 userAppInstallStatus](../api/intune-apps-userappinstallstatus-delete.md)|无|删除[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)。|
|[更新 userAppInstallStatus](../api/intune-apps-userappinstallstatus-update.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|更新[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|userName|String|用户名。|
|userPrincipalName|字符串|用户主体名称。|
|installedDeviceCount|Int32|已安装设备的计数。|
|failedDeviceCount|Int32|已失败设备的计数。|
|notInstalledDeviceCount|Int32|Not installed device count。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|应用程序|[mobileApp](../resources/intune-apps-mobileapp.md)|导航到移动应用程序链接。|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合|在设备上应用程序的安装状态。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "String (identifier)",
  "userName": "String",
  "userPrincipalName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```





