---
title: windowsDefenderApplicationControlSupplementalPolicy 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d5d8e0ccfdf23a16c4fa713cb75a30299bb4e269
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58800336"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicy-resource-type"></a>windowsDefenderApplicationControlSupplementalPolicy 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsDefenderApplicationControlSupplementalPolicies](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-list.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) 集合|列出 [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) 对象的属性和关系。|
|[获取 windowsDefenderApplicationControlSupplementalPolicy](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-get.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|读取 [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) 对象的属性和关系。|
|[创建 windowsDefenderApplicationControlSupplementalPolicy](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-create.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|创建新的 [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) 对象。|
|[删除 windowsDefenderApplicationControlSupplementalPolicy](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-delete.md)|无|删除 [windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)。|
|[更新 windowsDefenderApplicationControlSupplementalPolicy](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-update.md)|[windowsDefenderApplicationControlSupplementalPolicy](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md)|更新 [windowsDefenderApplicationControlSupplementalPolicy 对象](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy.md) 的属性。|
|[分配操作](../api/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicy-assign.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|WindowsDefenderApplicationControl 补充策略的密钥。|
|displayName|String|WindowsDefenderApplicationControl 显示名称策略的策略集。|
|description|String|WindowsDefenderApplicationControl 补充策略的说明。|
|content|二进制|采用字节数组格式的 WindowsDefenderApplicationControl 补充策略内容。|
|contentFileName|String|WindowsDefenderApplicationControl 补充策略内容的文件名。|
|version|String|WindowsDefenderApplicationControl 补充策略的版本。|
|creationDateTime|DateTimeOffset|上载 WindowsDefenderApplicationControl 补充策略的日期和时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改 WindowsDefenderApplicationControl 补充策略的日期和时间。|
|roleScopeTagIds|字符串集合|此 WindowsDefenderApplicationControl 补充策略实体的范围标记列表。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) 集合|此 WindowsDefenderApplicationControl 补充策略的关联组分配。|
|deploySummary|[windowsDefenderApplicationControlSupplementalPolicyDeploymentSummary](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentsummary.md)|WindowsDefenderApplicationControl 补充策略部署摘要。|
|deviceStatuses|[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) 集合|此 WindowsDefenderApplicationControl 补充策略的设备部署状态列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "content": "binary",
  "contentFileName": "String",
  "version": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```



