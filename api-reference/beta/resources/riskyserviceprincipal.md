---
title: riskyServicePrincipal 资源类型
description: '表示Azure AD工作负荷标识，包括应用程序、服务主体和托管标识的风险。 '
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ad89892a3cb33bb182a7df1a2e12d9355c2178b0
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723737"
---
# <a name="riskyserviceprincipal-resource-type"></a>riskyServicePrincipal 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Azure AD风险的服务主体。 Azure AD根据各种信号和机器学习持续评估服务主体风险。 此 API 提供对租户中所有处于风险中的服务主体的Azure AD访问权限。

继承自 [entity](../resources/entity.md)。

>**注意：** 使用 riskyServicePrincipal API 需要一个Azure AD Premium P2许可证。

## <a name="methods"></a>方法

| 方法                                                                                      | 返回类型                                                                        | 说明                                                     |
| :------------------------------------------------------------------------------------------ | :--------------------------------------------------------------------------------- | :-------------------------------------------------------------- |
| [列出 riskyServicePrincipals](../api/identityprotectionroot-list-riskyserviceprincipals.md) | [riskyServicePrincipal](../resources/riskyserviceprincipal.md) 集合          | 列出风险服务主体及其风险属性。        |
| [获取 riskyServicePrincipal](../api/riskyserviceprincipal-get.md)                            | [riskyServicePrincipal](../resources/riskyserviceprincipal.md)                     | 获取特定的风险服务主体及其风险属性。 |
| [dismiss](../api/riskyserviceprincipal-dismiss.md)                                          | 无                                                                               | 消除风险服务主体的风险。                  |
| [confirmComprom一](../api/riskyserviceprincipal-confirmcompromised.md)                    | 无                                                                               | 确认存在风险的服务主体受到威胁。               |
| [列表历史记录](../api/riskyserviceprincipal-list-history.md)                                | [riskyServicePrincipalHistoryItem](riskyserviceprincipalhistoryitem.md) 集合 | 获取服务主体Azure AD历史记录。          |

## <a name="properties"></a>属性

| 属性                | 类型           | 说明                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| :---------------------- | :------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| accountEnabled          | Boolean        | 如果已启用服务主体帐户，则为 `true`；否则，为 `false`。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| appId                   | String         | 关联的应用程序的全局唯一标识符 (**其 appId**) （如果有）。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| displayName             | String         | 服务主体的显示名称。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| id                      | String         | 分配给处于风险中的服务主体的唯一标识符。 继承自 [entity](../resources/entity.md)。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| isProcessing            | Boolean        | 指示Azure AD当前是否正在处理服务主体的风险状态。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| riskDetail              | riskDetail     | 检测到的风险的详细信息。 <br>**注意：** 此属性的详细信息仅适用于 Azure AD Premium P2 客户。 将返回 P1 客户 `hidden`。 <br/>可能的值是：、`none``adminGeneratedTemporaryPassword``userPerformedSecuredPasswordReset``userPerformedSecuredPasswordChange`、、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、 。 `adminConfirmedSigninCompromised``hidden``adminConfirmedUserCompromised``unknownFutureValue``adminConfirmedServicePrincipalCompromised``adminDismissedAllRiskForServicePrincipal` 请注意，必须使用此可`Prefer: include-unknown-enum-members`变化枚举 (请求) 获取以下[值：](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)`adminConfirmedServicePrincipalCompromised`、 `adminDismissedAllRiskForServicePrincipal`。 |
| riskLastUpdatedDateTime | DateTimeOffset | 上次更新风险状态的日期与时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2021 年 1 月 1 日午夜 UTC 为 `2021-01-01T00:00:00Z`。 支持 `$filter`（`eq`）。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| riskLevel               | riskLevel      | 检测到的风险工作负荷标识的级别。 可能的值包括 `low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。 支持 `$filter`（`eq`）。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| riskState               | riskState      | 服务主体的风险状态。 可取值包括：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| servicePrincipalType    | String         | 标识服务主体是表示 `Application`、、 `ManagedIdentity`或旧版应用程序 () `socialIdp` 。 这由内部Azure AD并继承自 [servicePrincipal](../resources/servicePrincipal.md)。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |

## <a name="relationships"></a>关系

| 关系 | 类型                                                                               | 说明                                                 |
| :----------- | :--------------------------------------------------------------------------------- | :---------------------------------------------------------- |
| history      | [riskyServicePrincipalHistoryItem](riskyserviceprincipalhistoryitem.md) 集合 | 表示服务主体Azure AD历史记录。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyServicePrincipal",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.riskyServicePrincipal",
  "id": "String (identifier)",
  "accountEnabled": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "displayName": "String",
  "appId": "String",
  "servicePrincipalType": "String"
}
```
