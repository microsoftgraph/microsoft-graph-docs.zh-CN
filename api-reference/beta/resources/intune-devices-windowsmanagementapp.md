---
title: windowsManagementApp 资源类型
description: Windows 管理应用实体。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b86d6d6ddad847b1a4b39fd96d61f619e19afaac
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365221"
---
# <a name="windowsmanagementapp-resource-type"></a>windowsManagementApp 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 管理应用实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 windowsManagementApp](../api/intune-devices-windowsmanagementapp-get.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|读取[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的属性和关系。|
|[更新 windowsManagementApp](../api/intune-devices-windowsmanagementapp-update.md)|[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)|更新[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Windows 管理应用程序的唯一标识符|
|availableVersion|String|Windows 管理应用程序的可用版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|healthStates|[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)集合|已安装的 Windows management 应用的运行状况状态列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String"
}
```



