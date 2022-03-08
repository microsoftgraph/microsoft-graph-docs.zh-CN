---
title: managedTenant 资源类型
description: 表示与多租户管理平台交互的可用操作。
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: c072c5b127a4e7b22022d03b674e8a3a8bdacd19
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337024"
---
# <a name="managedtenant-resource-type"></a>managedTenant 资源类型

命名空间：microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

作为 Microsoft 365 Lighthouse API 的根资源，**managedTenant** 表示可供托管服务提供商 (MSP) 使用的功能，以扩展其客户租户的远程管理，以帮助其进入正常和安全状态。

该Microsoft 365 Lighthouse API 在 OData 子名称空间中定义`microsoft.graph.managedTenants`。

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|aggregatedPolicyCompliances|[microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) 集合|跨托管租户的设备合规性策略聚合视图。|
|auditEvents|[microsoft.graph.managedTenants.auditEvent](../resources/managedtenants-auditevent.md) 集合|跨托管租户的审核事件集合。|
|cloudPcConnections|[microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) 集合|跨托管租户的云电脑连接的集合。|
|cloudPcDevices|[microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) 集合|跨托管租户的云电脑设备的集合。|
|cloudPcsOverview|[microsoft.graph.managedTenants.cloudPcOverview](../resources/managedtenants-cloudpcoverview.md) 集合|跨托管租户的云电脑信息概述。|
|conditionalAccessPolicyCoverages|[microsoft.graph.managedTenants.conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) 集合|跨托管租户的条件访问策略覆盖的聚合视图。|
|credentialUserRegistrationsSummaries|[microsoft.graph.managedTenants.credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) 集合|跨托管租户进行多重身份验证和自助服务密码重置的用户注册的摘要信息。|
|deviceCompliancePolicySettingStateSummaries|[microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) 集合|跨托管租户的设备合规性策略设置状态摘要信息。|
|managedDeviceCompliances|[microsoft.graph.managedTenants.managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) 集合|跨托管租户的托管设备的合规性集合。|
|managedDeviceComplianceTrends|[microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) 集合|跨托管租户的设备合规性趋势见解。|
|managementActions|[microsoft.graph.managedTenants.managementAction](../resources/managedtenants-managementaction.md) 集合|跨托管租户的基线管理操作的集合。|
|managementActionTenantDeploymentStatuses|[microsoft.graph.managedTenants.managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) 集合|跨托管租户的管理操作租户级别状态。|
|managementIntents|[microsoft.graph.managedTenants.managementIntent](../resources/managedtenants-managementintent.md) 集合|跨托管租户的基线管理意图的集合。|
|managementTemplates|[microsoft.graph.managedTenants.managementTemplate](../resources/managedtenants-managementtemplate.md) 集合|跨托管租户的基线管理模板的集合。|
|tenantGroups|[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) 集合|多租户管理平台使用的托管租户的逻辑分组的集合。|
|tenants|[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md) 集合|与管理实体关联的租户集合。|
|tenantsCustomizedInformation|[microsoft.graph.managedTenants.tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) 集合|跨托管租户的租户级别自定义信息的集合。|
|tenantsDetailedInformation|[microsoft.graph.managedTenants.tenantDetailedInformation](../resources/managedtenants-tenantdetailedinformation.md) 集合|跨托管租户的集合租户级别详细信息。|
|tenantTags|[microsoft.graph.managedTenants.tenantTag](../resources/managedtenants-tenanttag.md) 集合|跨托管租户的租户标记集合。|
|windowsDeviceMalwareStates|[microsoft.graph.managedTenants.windowsDeviceMalwareState](../resources/managedtenants-windowsdevicemalwarestate.md) 集合|跨托管租户向 Windows注册Microsoft Endpoint Manager恶意软件的状态。|
|windowsProtectionStates|[microsoft.graph.managedTenants.windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) 集合|跨托管租户Windows注册的设备Microsoft Endpoint Manager保护状态。|

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
