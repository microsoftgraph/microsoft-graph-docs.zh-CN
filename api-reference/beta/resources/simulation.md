---
title: 模拟资源类型
description: 表示租户中的攻击模拟培训活动。
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: fbd043bd16176834c523d3b5083fab5ce69c406d
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757834"
---
# <a name="simulation-resource-type"></a>模拟资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户中的攻击模拟培训活动。

攻击模拟和培训是一项服务，作为 [Microsoft Defender for Office 365 的一Office 365](/microsoft-365/security/office-365-security/defender-for-office-365?view=o365-worldwide&preserve-view=true)。 此服务可让租户中的用户体验真实的恶意钓鱼攻击，并从中学习。 该服务使租户管理员能够在网络钓鱼模拟中模拟、分配培训和读取派生的见解到用户的联机行为。 该服务提供攻击模拟报告，帮助租户识别安全知识差距，以便可以进一步培训用户以减少对攻击的敏感性。

攻击模拟和培训 API 使租户管理员能够列出启动的模拟练习和培训，并获取有关钓鱼模拟中用户在线[](report-m365defender-reports-overview.md)行为的派生见解的报告。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出模拟](../api/attacksimulationroot-list-simulations.md)|[模拟](../resources/simulation.md) 集合|获取模拟对象 [及其](../resources/simulation.md) 属性的列表。|

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|attackTechnique|[simulationAttackTechnique](#simulationattacktechnique-values)|攻击模拟和培训活动中使用的社交工程技术。 支持 `$filter` 和 `$orderby`。 可取值为：`unknown`、`credentialHarvesting`、`attachmentMalware`、`driveByUrl`、`linkInAttachment`、`linkToMalwareFile` 或 `unknownFutureValue`。 有关社交工程攻击技术类型详细信息，请参阅 [模拟](/microsoft-365/security/office-365-security/attack-simulation-training-get-started?view=o365-worldwide&preserve-view=true#simulations)。|
|attackType|[simulationAttackType](#simulationattacktype-values)|攻击模拟和培训计划的攻击类型。 支持 `$filter` 和 `$orderby`。 可取值为：`unknown`、`social`、`cloud`、`endpoint`、`unknownFutureValue`。|
|automationId|String|攻击模拟自动化的唯一标识符。|
|completionDateTime|DateTimeOffset|攻击模拟和培训市场活动的完成日期和时间。 支持 `$filter` 和 `$orderby`。|
|createdBy|[emailIdentity](../resources/emailidentity.md)|创建攻击模拟和培训活动的用户的身份。|
|createdDateTime|DateTimeOffset|创建攻击模拟和培训市场活动的日期和时间。|
|description|字符串|攻击模拟和培训计划的说明。|
|displayName|字符串|攻击模拟和培训计划的显示名称。 支持 `$filter` 和 `$orderby`。|
|id|String|攻击模拟和培训活动的唯一标识符。|
|isAutomated|Boolean|表示是否从模拟自动化流创建攻击模拟和培训活动的标志。 支持 `$filter` 和 `$orderby`。 |
|lastModifiedBy|[emailIdentity](../resources/emailidentity.md)|最近修改攻击模拟和培训活动的用户的身份。|
|lastModifiedDateTime|DateTimeOffset|最近修改攻击模拟和培训活动的日期和时间。|
|launchDateTime|DateTimeOffset|攻击模拟和培训计划的启动/开始日期和时间。 支持 `$filter` 和 `$orderby`。|
|payloadDeliveryPlatform|payloadDeliveryPlatform|在攻击模拟和培训活动中使用的网络钓鱼有效负载的交付方法。 可取值为：`unknown`、`sms`、`email`、`teams`、`unknownFutureValue`。|
|report|[simulationReport](../resources/simulationreport.md)|攻击模拟和培训计划的报告。|
|状态|[simulationStatus](#simulationstatus-values)|攻击模拟和培训计划的状态。 支持 `$filter` 和 `$orderby`。 可取值为：`unknown`、`draft`、`running`、`scheduled`、`succeeded`、`failed`、`cancelled`、`excluded`、`unknownFutureValue`。|

### <a name="simulationstatus-values"></a>simulationStatus 值

|成员|说明 |
|:---|:---|
|unknown| 未定义模拟状态。 |
|draft| 模拟在草稿模式下。 |
|running| 模拟正在运行。 |
|scheduled| 模拟已计划。 |
|succeeded| 模拟已成功。 |
|failed| 模拟失败。 |
|cancelled| 模拟被取消。 |
|已排除| 模拟将排除。 |
|unknownFutureValue| 可发展枚举 sentinel 值。 请勿使用。 |

### <a name="simulationattacktechnique-values"></a>simulationAttackTechnique 值

|成员|说明 |
|:---|:---|
|unknown| 未定义攻击技术。 |
|credentialHarvesting| 涉及最终用户提供凭据的攻击技术。 |
|attachmentMalware| 涉及最终用户单击附件的攻击技术。 |
|driveByUrl| 涉及最终用户单击网络钓鱼有效负载中的 URL 链接的攻击技术。 |
|linkInAttachment| 涉及最终用户单击附件中的 URL 链接的攻击技术。 |
|linkToMalwareFile| 涉及最终用户单击指向恶意软件文件的 URL 链接的攻击技术。 |
|unknownFutureValue| 可发展枚举 sentinel 值。 请勿使用。 |

### <a name="simulationattacktype-values"></a>simulationAttackType 值

|成员|说明 |
|:---|:---|
|unknown| 攻击类型未标识。 |
|social| 攻击使用社交技能以自我方式处理犯罪，从而产生一种虚假的满足感、紧急感或担心感。 |
|云| 对云环境中主机或用户的攻击，例如拒绝服务攻击。|
|endpoint| 攻击企业网络的终结点，如台式机、笔记本电脑、移动电话、物联网设备。 |
|unknownFutureValue| 可发展枚举 sentinel 值。 请勿使用。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.simulation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulation",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "attackType": "String",
  "attackTechnique": "String",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.emailIdentity"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.emailIdentity"
  },
  "launchDateTime": "String (timestamp)",
  "completionDateTime": "String (timestamp)",
  "isAutomated": "Boolean",
  "automationId": "String",
  "payloadDeliveryPlatform": "String",
  "report": {
    "@odata.type": "microsoft.graph.simulationReport"
  }
}
```


## <a name="see-also"></a>另请参阅
- [模拟网络钓鱼攻击](/microsoft-365/security/office-365-security/attack-simulation-training?view=o365-worldwide&preserve-view=true)
- [开始使用攻击模拟培训](/microsoft-365/security/office-365-security/attack-simulation-training-get-started?view=o365-worldwide&preserve-view=true#simulations)。
