---
title: androidManagedStoreAppAssignmentSettings 资源类型
description: 包含用于将 Android 托管应用商店移动应用分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8a2afa3243cc19b016430e2b9960f6aecc349cdf
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60691538"
---
# <a name="androidmanagedstoreappassignmentsettings-resource-type"></a>androidManagedStoreAppAssignmentSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于将 Android 托管应用商店移动应用分配给组的属性。


继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|androidManagedStoreAppTrackIds|String collection|为此应用分配启用的轨 ID。|
|autoUpdateMode|[androidManagedStoreAutoUpdateMode](../resources/intune-shared-androidmanagedstoreautoupdatemode.md)|此应用程序分配的自动更新优先顺序。 可取值为：`default`、`postponed`、`priority`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppAssignmentSettings",
  "androidManagedStoreAppTrackIds": [
    "String"
  ],
  "autoUpdateMode": "String"
}
```



