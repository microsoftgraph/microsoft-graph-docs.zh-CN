---
title: managedTenant 资源类型
description: 表示与多租户管理平台交互的可用操作。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 4518a6b4f3b05e237e4a44c06bed12901369879b
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094156"
---
# <a name="managedtenant-resource-type"></a>managedTenant 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

作为 Microsoft 365 Lighthouse API 的根资源，**managedTenant** 表示托管服务提供商 (MSP) 可用的功能，以便缩放其客户租户的远程管理，以帮助其进入正常且安全的状态。

Microsoft 365 Lighthouse API 是在 OData 子名空间中定义的。 `microsoft.graph.managedTenants`

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|aggregatedPolicyCompliances|[microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) 集合|跨托管租户的设备符合性策略的聚合视图。|
|auditEvents|[microsoft.graph.managedTenants.auditEvent](../resources/managedtenants-auditevent.md) 集合|跨托管租户的审核事件集合。|
|cloudPcConnections|[microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) 集合|跨托管租户的云电脑连接集合。|
|cloudPcDevices|[microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) 集合|跨托管租户的云电脑设备集合。|
|cloudPcsOverview|[microsoft.graph.managedTenants.cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) 集合|跨托管租户的云电脑信息概述。|
|conditionalAccessPolicyCoverages|[microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) 集合|跨托管租户的条件访问策略覆盖范围的聚合视图。|
|credentialUserRegistrationsSummaries|[microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) 集合|有关跨托管租户进行多重身份验证和自助密码重置的用户注册的摘要信息。|
|deviceCompliancePolicySettingStateSummaries|[microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) 集合|有关跨托管租户的设备符合性策略设置状态的摘要信息。|
|managedDeviceCompliances|[microsoft.graph.managedTenants.managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) 集合|托管设备跨托管租户的符合性集合。|
|managedDeviceComplianceTrends|[microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) 集合|跨托管租户实现设备符合性的趋势见解。|
|managementActions|[microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md) 集合|跨托管租户的基线管理操作的集合。|
|managementActionTenantDeploymentStatuses|[microsoft.graph.managedTenants.managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) 集合|跨托管租户的管理操作的租户级别状态。|
|managementIntents|[microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md) 集合|跨托管租户的基线管理意向的集合。|
|managementTemplates|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) 集合|跨托管租户的基线管理模板的集合。|
|myRoles|[microsoft.graph.managedTenants.myRole](../resources/managedtenants-myrole.md) 集合|托管租户的已登录用户的角色分配集合。|
|tenantGroups|[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) 集合|多租户管理平台使用的托管租户逻辑分组的集合。|
|租户|[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md) 集合|与管理实体关联的租户的集合。|
|tenantsCustomizedInformation|[microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) 集合|跨托管租户的租户级别自定义信息的集合。|
|tenantsDetailedInformation|[microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) 集合|集合租户级别跨托管租户的详细信息。|
|tenantTags|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md) 集合|跨托管租户的租户标记的集合。|
|tenantUsage|[microsoft.graph.managedTenants.tenantUsage](../resources/managedtenants-tenantusage.md) 集合|跨托管租户的租户使用情况集合。|
|windowsDeviceMalwareStates|[microsoft.graph.managedTenants.windowsDeviceMalwareState](../resources/managedtenants-windowsdevicemalwarestate.md) 集合|在托管租户中注册到Microsoft Endpoint Manager的Windows设备的恶意软件状态。|
|windowsProtectionStates|[microsoft.graph.managedTenants.windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) 集合|在托管租户中注册了Microsoft Endpoint Manager的Windows设备的保护状态。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managedTenant",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenant",
  "id": "String (identifier)"
}
```
