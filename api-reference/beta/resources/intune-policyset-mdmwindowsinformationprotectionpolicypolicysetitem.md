---
title: mdmWindowsInformationProtectionPolicyPolicySetItem 资源类型
description: 包含用于 mdm windows 信息保护策略 PolicySetItem 的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6fb67456954652c6f468cd163815ebeb198e2dc3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288073"
---
# <a name="mdmwindowsinformationprotectionpolicypolicysetitem-resource-type"></a>mdmWindowsInformationProtectionPolicyPolicySetItem 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于 mdm windows 信息保护策略 PolicySetItem 的属性的类。


继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 mdmWindowsInformationProtectionPolicyPolicySetItems](../api/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem-list.md)|[mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) 集合|列出 [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) 对象的属性和关系。|
|[获取 mdmWindowsInformationProtectionPolicyPolicySetItem](../api/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem-get.md)|[mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)|读取 [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) 对象的属性和关系。|
|[创建 mdmWindowsInformationProtectionPolicyPolicySetItem](../api/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem-create.md)|[mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)|创建新的 [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) 对象。|
|[删除 mdmWindowsInformationProtectionPolicyPolicySetItem](../api/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem-delete.md)|无|删除 [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)。|
|[更新 mdmWindowsInformationProtectionPolicyPolicySetItem](../api/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem-update.md)|[mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)|更新 [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|MobileAppPolicySetItem 的键。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|PolicySetItem 的创建时间。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|PolicySetItem 的上次修改时间。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|字符串|PolicySetItem 的 PayloadId。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|字符串|PolicySetItem 的 policySetType。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|字符串|PolicySetItem 的 DisplayName。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|PolicySetItem 的状态。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。 可取值为：`unknown`、`validating`、`partialSuccess`、`success`、`error`、`notAssigned`。|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|错误代码（如果发生）。 继承自 [policySetItem](../resources/intune-policyset-policysetitem.md)。 可取值为：`noError`、`unauthorized`、`notFound`、`deleted`。|
|guidedDeploymentTags|String 集合|继承自[policySetItem](../resources/intune-policyset-policysetitem.md)的引导部署的标记|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mdmWindowsInformationProtectionPolicyPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicyPolicySetItem",
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




