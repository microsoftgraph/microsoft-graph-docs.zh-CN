---
title: riskyUser 资源类型
description: 有风险的用户项
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d54cab6905142282890f60042802c9f8060330bbffb5923505b5bae1a6cd9b45
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235301"
---
# <a name="riskyuser-resource-type"></a>riskyUser 资源类型

命名空间：microsoft.graph

表示处于风险中的 Azure AD 用户。 Azure AD 根据各种信号和机器学习持续评估用户风险。 此 API 为 Azure AD 中所有处于风险中的用户提供编程访问权限。

有关风险事件详细信息，请参阅Azure Active Directory [Identity Protection。](/azure/active-directory/identity-protection/overview-identity-protection)

>**注意：** 使用 riskyUsers API 需要Azure AD Premium P2许可证。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 riskyUsers](../api/riskyuser-list.md)|[riskyUser](../resources/riskyuser.md) 集合|获取 **riskyUser** 对象及其属性的列表。|
|[获取 riskyUser](../api/riskyuser-get.md)|[riskyUser](../resources/riskyuser.md)|读取 **riskyUser** 对象的属性和关系。|
|[消除 riskyUser](../api/riskyuser-dismiss.md)|无|消除一个或多个 **riskyUser 对象** 的风险。 |
|[确认存在已泄露的 riskyUser](../api/riskyuser-confirmcompromised.md)|无|确认一个或多个 **riskyUser** 对象受到威胁。|
|[列表历史记录](../api/riskyuser-list-history.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 集合|从 **历史记录导航属性获取 riskyUserHistoryItems。**|
|[获取历史记录](../api/riskyuser-get-riskyuserhistoryitem.md)|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)|读取 [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 对象的属性和关系。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|处于风险中的用户的唯一 ID。|
|isDeleted|Boolean|指示用户是否被删除。 可取值为：`true`、`false`。|
|isProcessing|Boolean|指示后端是否正在处理用户的风险状态。|
|riskDetail|riskDetail|检测到的风险的详细信息。 可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。|
|riskLastUpdatedDateTime|DateTimeOffset|上次更新有风险用户的日期和时间。  DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`|
|riskLevel|riskLevel|检测到的风险用户级别。 可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。|
|riskState|riskState|用户风险的状态。 可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。|
|userDisplayName|String|有风险的用户显示名称。|
|userPrincipalName|String|有风险的用户主体名称。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|history|[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 集合|   与用户风险级别更改相关的活动|

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
