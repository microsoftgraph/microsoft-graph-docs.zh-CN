---
title: 事件资源类型
description: Microsoft 365 Defender事件是反映攻击事件的关联警报和关联元数据的集合。
ms.date: 09/09/2021
author: BenAlfasi
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e1bef3d9d62fc91cee2fe1883d564bd27eaba638
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220832"
---
# <a name="incident-resource-type"></a>事件资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft 365 Defender事件是反映租户中攻击事件的关联警报和关联元数据的集合。

Microsoft 365服务和应用在检测到可疑或恶意事件或活动时创建警报。 个别警报提供有关已完成或持续攻击的有价值的线索。 但是，攻击通常对不同类型的实体（如设备、用户和邮箱）使用各种技术。 结果是租户中多个实体收到多个警报。
由于将各个警报分组在一起以深入了解攻击可能非常困难且耗时，Microsoft 365 Defender自动将警报及其相关信息聚合到事件中。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出事件](../api/security-list-incidents.md)|[事件](../resources/incident.md) 集合|获取事件对象 [及其](../resources/incident.md) 属性的列表。|
|[获取事件](../api/incident-get.md)|[incident](../resources/incident.md)|读取事件对象的属性 [和](../resources/incident.md) 关系。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|assignedTo|String|事件的所有者;如果没有分配所有者，则为空。 可编辑文本自由。|
|classification|[m365AlertClassification](#m365alertclassification-values)|事件的规范。 可取值为：`unknown`、`falsePositive`、`truePositive`、`benignPositive`、`unknownFutureValue`。|
|comments|[m365AlertComment](../resources/m365alertcomment.md) 集合|管理事件时，由 SecOps (安全) 创建的评论数组。|
|createdDateTime|DateTimeOffset|首次创建事件的时间。|
|确定|[m365AlertDetermination](#m365alertdetermination-values)|指定事件的确定。 可取值为：`unknown`、`apt`、`malware`、`securityPersonnel`、`securityTesting`、`unwantedSoftware`、`other`、`multiStagedAttack`、`compromisedUser`、`phishing`、`maliciousUserActivity`、`clean`、`insufficientData`、`confirmedUserActivity`、`lineOfBusinessApplication`、`unknownFutureValue`。|
|displayName|String|事件名称。|
|id|String|表示事件的唯一标识符。|
|incidentWebUrl|String|事件门户中事件Microsoft 365 Defender URL。|
|lastUpdateDateTime|DateTimeOffset|上次更新事件的时间。|
|redirectIncidentId|String|只有在将事件与另一个事件分组在一起时填充，作为处理事件的逻辑的一部分。|
|severity|[m365AlertSeverity](#m365alertseverity-values )|指示对资产可能的影响。 严重性越高，影响越大。 通常，严重性级别较高的项目需要最直接的关注。 可取值为：`unknown`、`informational`、`low`、`medium`、`high`、`unknownFutureValue`。|
|status|[incidentStatus](#incidentstatus-values)|事件的状态。 可能的值是：`active`、`resolved`、`redirected`、`unknownFutureValue`。|
|标记|字符串集合|与事件关联的自定义标记数组。|


### <a name="incidentstatus-values"></a>incidentStatus 值 

| 成员              | 说明                                                                                                           |
| :-------------------| :-------------------------------------------------------------------------------------------------------------------- |
| active              | 事件为活动状态。                                                                                      |
| 已解决            | 事件已解决。                                                                                    |
| redirected          | 事件与另一个事件合并。 目标事件 ID 将显示在 **redirectIncidentId** 属性中。 |
| unknownFutureValue  | 可发展枚举 sentinel 值。 请勿使用。                                                                     |

### <a name="m365alertclassification-values"></a>m365AlertClassification 值 

| 成员              | 说明                                                                                                                         |
| :-------------------| :---------------------------------------------------------------------------------------------------------------------------------- |
| unknown             | 警报尚未分类。                                                                                                     |
| falsePositive       | 警报为误报，未检测到恶意活动。                                                                 |
| truePositive        | 警报为真正的正，检测到恶意活动。                                                                         |
| 将positive      | 该警报是良好的正，检测到受信任/内部用户存在潜在的恶意活动，例如安全测试。 |
| unknownFutureValue  | 可发展枚举 sentinel 值。 请勿使用。                                                                                   |

### <a name="m365alertdetermination-values"></a>m365AlertDetermination 值 

| 成员                     | 说明                                                                                                                  |
| :--------------------------| :--------------------------------------------------------------------------------------------------------------------------- |
| unknown                    | 尚未设置确定值。                                                                                          |
| apt                        | 检测到高级永久性威胁的真正正警报。                                                           |
| 恶意软件 (malware)                    | 检测到恶意软件的真正正警报。                                                                      |
| securityPersonnel          | 真正的正警报，检测到客户安全团队中某人执行的有效可疑活动。 |
| securityTesting            | 警报检测到作为已知安全测试的一部分执行的有效可疑活动。                         |
| unwantedSoftware           | 警报检测到不需要的软件。                                                                                        |
| multiStagedAttack          | 检测到多个击杀链攻击阶段的真正的正警报。                                                       |
| compromisedUser            | 一个真正的正警报，检测到预期用户的凭据被泄露或被盗。                         |
| 仿冒                   | 检测到网络钓鱼电子邮件的真正正警报。                                                                        |
| maliciousUserActivity      | 真正的正警报，检测到已登录用户执行恶意活动。                                   |
| clean                      | 假警报，无可疑活动。                                                                                       |
| insufficientData           | 假警报，没有足够信息可以证明其他情况。                                                                |
| confirmedUserActivity      | 警报捕获了真正的可疑活动，该活动被视为正常，因为它是已知用户活动。                       |
| lineOfBusinessApplication  | 警报捕获了真正的可疑活动，该活动被视为正常，因为它是已知的经确认的内部应用程序。  |
| other                      | 其他确定。                                                                                                         |
| unknownFutureValue         | 可发展枚举 sentinel 值。 请勿使用。                                                                            |

### <a name="m365alertseverity-values"></a>m365AlertSeverity 值 

| 成员                     | 说明                                                                                                                  |
| :--------------------------| :--------------------------------------------------------------------------------------------------------------------------- |
| unknown            | 未知严重性。       |
| informational      | 可能不可操作或被视为对网络有害的警报，但可以提升组织对潜在安全问题的安全意识。     |
| low                | 与流行恶意软件相关的威胁警报。 例如，黑客工具、非恶意软件黑客工具（如运行探索命令和清除日志）通常不会指示面向组织的高级威胁。 它还可能来自由组织中用户测试的隔离安全工具。  |
| 中等             | 由检测与响应泄露后行为生成的警报，这些行为可能是 APT 高级永久性威胁 (一) 。 这包括观察到的攻击阶段的典型行为、异常注册表更改、执行可疑文件等。 虽然其中一些可能是由于内部安全测试，但是它们是有效的检测，需要调查，因为它们可能是高级攻击的一部分。 |
| high               | 通常看到的与 APT 高级永久性威胁 (警报) 。 这些警报表明存在高风险，因为它们可能危害资产的严重性。 例如：凭据盗窃工具活动、未与任何组关联的勒索软件活动、篡改安全传感器或任何恶意活动，这些活动会指示人类对手。 |
| unknownFutureValue | 可发展枚举 sentinel 值。 请勿使用。 |



## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.incident",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.incident",
  "id": "String (identifier)",
  "incidentWebUrl": "String",
  "redirectIncidentId": "String",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "lastUpdateDateTime": "String (timestamp)",
  "assignedTo": "String",
  "classification": "String",
  "determination": "String",
  "status": "String",
  "severity": "String",
  "tags": [
    "String"
  ],
  "comments": [
    {
      "@odata.type": "microsoft.graph.m365AlertComment"
    }
  ]
}
```
