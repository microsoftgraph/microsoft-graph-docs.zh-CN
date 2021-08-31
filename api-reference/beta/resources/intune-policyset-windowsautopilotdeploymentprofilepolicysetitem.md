---
title: windowsAutopilotDeploymentProfilePolicySetItem 资源类型
description: 一个包含用于 Windows autopilot 部署配置文件 PolicySetItem 的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d91c0dab6a32832644de1073fab7297c5bc257b5
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58821912"
---
# <a name="windowsautopilotdeploymentprofilepolicysetitem-resource-type"></a>windowsAutopilotDeploymentProfilePolicySetItem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一个包含用于 Windows autopilot 部署配置文件 PolicySetItem 的属性的类。


继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsAutopilotDeploymentProfilePolicySetItems](../api/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem-list.md)|[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) 集合|列出 [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) 对象的属性和关系。|
|[获取 windowsAutopilotDeploymentProfilePolicySetItem](../api/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem-get.md)|[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)|读取 [windowsAutopilotDeploymentProfilePolicySetItem 对象的属性和](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) 关系。|
|[创建 windowsAutopilotDeploymentProfilePolicySetItem](../api/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem-create.md)|[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)|创建新的 [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) 对象。|
|[删除 windowsAutopilotDeploymentProfilePolicySetItem](../api/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem-delete.md)|无|删除 [windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)。|
|[更新 windowsAutopilotDeploymentProfilePolicySetItem](../api/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem-update.md)|[windowsAutopilotDeploymentProfilePolicySetItem](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md)|更新 [windowsAutopilotDeploymentProfilePolicySetItem 对象](../resources/intune-policyset-windowsautopilotdeploymentprofilepolicysetitem.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|PolicySetItem 的键。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|PolicySetItem 的创建时间。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|PolicySetItem 的上次修改时间。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|String|PolicySetItem 的 PayloadId。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|String|PolicySetItem 的 policySetType。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|字符串|PolicySetItem 的 DisplayName。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|状态|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|PolicySetItem 的状态。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。 可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|错误代码（如果发生了任何错误）。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。 可能的值是：`noError`、`unauthorized`、`notFound`、`deleted`。|
|guidedDeploymentTags|字符串集合|引导式部署的标记 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfilePolicySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ]
}
```



