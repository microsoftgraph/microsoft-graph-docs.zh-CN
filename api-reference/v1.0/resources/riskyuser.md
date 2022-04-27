---
title: riskyUser 资源类型
description: 风险用户项
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 222ff5f10fdb7ddf9ebd80209551d5e3f44ce83b
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060784"
---
# <a name="riskyuser-resource-type"></a>riskyUser 资源类型

命名空间：microsoft.graph

表示Azure AD有风险的用户。 Azure AD根据各种信号和机器学习不断评估用户风险。 此 API 提供对Azure AD中所有有风险用户的编程访问权限。

有关风险事件的详细信息，请[参阅Azure Active Directory标识保护](/azure/active-directory/identity-protection/overview-identity-protection)。

>[!NOTE]
> 1. 使用 riskyUsers API 需要Azure AD Premium P2许可证。
> 2. 风险用户数据的可用性受[Azure AD数据保留策略](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)的控制。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 riskyUsers](../api/riskyuser-list.md)|[riskyUser](../resources/riskyuser.md) 集合|获取 **riskyUser** 对象及其属性的列表。|
|[获取 riskyUser](../api/riskyuser-get.md)|[riskyUser](../resources/riskyuser.md)|读取 **riskyUser** 对象的属性和关系。|
|[关闭 riskyUser](../api/riskyuser-dismiss.md)|无|消除一个或多个 **有风险的User** 对象的风险。 |
|[确认有风险的用户是否已泄露](../api/riskyuser-confirmcompromised.md)|无|确认一个或多个 **有风险的User** 对象已泄露。|
|[列出历史记录](../api/riskyuser-list-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 集合|从历史记录导航属性获取 **riskyUserHistoryItems** 。|
|[获取历史记录](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|读取 [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 对象的属性和关系。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|有风险的用户的唯一 ID。|
|isDeleted|Boolean|指示是否删除用户。 可取值为：`true`、`false`。|
|isProcessing|Boolean|指示后端是否正在处理用户的风险状态。|
|riskDetail|riskDetail|检测到的风险的详细信息。 可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。|
|riskLastUpdatedDateTime|DateTimeOffset|风险用户上次更新的日期和时间。  DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|riskLevel|riskLevel|检测到的风险用户的级别。 可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。|
|riskState|riskState|用户风险的状态。 可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。|
|userDisplayName|String|有风险的用户显示名称。|
|userPrincipalName|String|有风险的用户主体名称。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|历史|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 集合|   与用户风险级别更改相关的活动|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUser",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```
