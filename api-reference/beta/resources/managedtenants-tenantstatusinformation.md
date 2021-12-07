---
title: tenantStatusInformation 资源类型
description: 表示托管租户的载入状态信息。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 4d5cf90ebcb1567a84c4d7e0f00547f0e946598d
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61321965"
---
# <a name="tenantstatusinformation-resource-type"></a>tenantStatusInformation 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示托管租户的载入状态信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|delegatedPrivilegeStatus|delegatedPrivilegeStatus|管理实体与托管租户之间的委派管理员权限关系的状态。 可取值为：`none`、`delegatedAdminPrivileges`、`unknownFutureValue`。 可选。 只读。|
|lastDelegatedPrivilegeRefreshDateTime|DateTimeOffset|已更新委派管理员权限状态的日期和时间。 可选。 只读。|
|offboardedByUserId|String|从托管租户上注销的帐户的标识符。 可选。 只读。|
|offboardedDateTime|DateTimeOffset|托管租户从外载的日期和时间。 可选。 只读。|
|onboardedByUserId|String|已载入托管租户的帐户的标识符。 可选。 只读。|
|onboardedDateTime|DateTimeOffset|托管租户载入的日期和时间。 可选。 只读。|
|onboardingStatus|tenantOnboardingStatus|托管租户的载入状态。 可取值为：`ineligible`、`inProcess`、`active`、`inactive`、`unknownFutureValue`。 可选。 只读。|
|tenantOnboardingEligibilityReason|tenantOnboardingEligibilityReason|组织中加入资格Microsoft 365 Lighthouse。 可能的值是 `none` `contractType` `delegatedAdminPrivileges` ：、、、 `usersCount` `license` 和 `unknownFutureValue` 。 可选。 只读。|
|workloadStatuses|[microsoft.graph.managedTenants.workloadStatus](../resources/managedtenants-workloadstatus.md) 集合|托管租户的工作负荷集合。 可选。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantStatusInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantStatusInformation",
  "onboardingStatus": "String",
  "onboardedDateTime": "String (timestamp)",
  "onboardedByUserId": "String",
  "offboardedDateTime": "String (timestamp)",
  "offboardedByUserId": "String",
  "delegatedPrivilegeStatus": "String",
  "lastDelegatedPrivilegeRefreshDateTime": "String (timestamp)",
  "workloadStatuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadStatus"
    }
  ]
}
```
