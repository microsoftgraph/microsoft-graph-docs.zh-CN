---
title: win32LobAppRestartSettings 资源类型
description: 包含描述应用安装后重启协调的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 075ef2eae803566a8201365e3f7df4a435f1b0ab
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805687"
---
# <a name="win32lobapprestartsettings-resource-type"></a>win32LobAppRestartSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含描述应用安装后重启协调的属性。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|gracePeriodInMinutes|Int32|应用安装后重启设备之前等待的分钟数。|
|countdownDisplayBeforeRestartInMinutes|Int32|重启时间前显示挂起重启的倒计时器对话框的分钟数。|
|restartNotificationSnoozeDurationInMinutes|Int32|选择"暂停"按钮时暂停重新启动通知对话框的分钟数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRestartSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRestartSettings",
  "gracePeriodInMinutes": 1024,
  "countdownDisplayBeforeRestartInMinutes": 1024,
  "restartNotificationSnoozeDurationInMinutes": 1024
}
```



