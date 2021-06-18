---
title: cloudPcOnPremisesConnectionHealthCheck 资源类型
description: 云电脑本地连接运行状况检查的结果。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 0323ee64056df1019cc2a8f6e2bd004ffec223b7
ms.sourcegitcommit: 2d0daa446c7b37ced1d214e0c6e18e2b8243bb09
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2021
ms.locfileid: "53010197"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>cloudPcOnPremisesConnectionHealthCheck 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

云电脑本地连接运行状况检查的结果。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[cloudPcOnPremisesConnection 的 RunHealthChecks](../api/cloudpconpremisesconnection-runhealthcheck.md)|无|运行 [cloudPcOnPremisesConnection 的运行状况检查](../resources/cloudpconpremisesconnection.md)。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|此显示名称检查项目的详细信息。|
|状态|[cloudPcOnPremisesConnectionStatus](../resources/cloudpconpremisesconnection.md#cloudpconpremisesconnectionstatus-values)|运行状况检查项目的状态。 可取值为：`pending`、`running`、`passed`、`failed`、`unknownFutureValue`。 只读。|
|startDateTime|DateTimeOffset|运行状况检查项目的开始时间。 只读。|
|endDateTime|DateTimeOffset|运行状况检查项目的结束时间。 只读。|
|errorType|[cloudPcOnPremisesConnectionHealthCheckErrorType](#cloudpconpremisesconnectionhealthcheckerrortype-values)|此运行状况检查期间发生的错误类型。|
|recommendedAction|String|修复相应错误的推荐操作。|
|additionalDetails|String|有关运行状况检查或建议操作的其他详细信息。|

### <a name="cloudpconpremisesconnectionhealthcheckerrortype-values"></a>cloudPcOnPremisesConnectionHealthCheckErrorType 值

|成员|说明|
|:---|:---|
|dnsCheckFqdnNotFound|DNS 检查失败，因为找不到完全限定的域名。 请重新输入完全限定的域名。|
|dnsCheckUnknownError|DNS 检查由于未知错误失败。 请联系客户支持。|
|adJoinCheckFqdnNotFound|活动域加入检查失败，因为找不到完全限定的域名。 请重新输入完全限定的域名。|
|adJoinCheckIncorrectCredentials|活动域加入检查失败，因为域凭据不正确。 请更新用户名和密码。|
|adJoinCheckOrganizationalUnitNotFound|活动域加入检查失败，因为找不到指定的组织单位。 请重新输入组织单位。|
|adJoinCheckOrganizationalUnitIncorrectFormat|活动域加入检查失败，因为指定的组织单位的格式不正确。 示例格式："OU=OU1，OU=OU2，OU=OU3，DC=DC1"。|
|adJoinCheckAccessDenied|活动域加入检查失败，因为当委派了控制权的非管理员用户尝试将计算机对象加入域控制器时，访问被拒绝。 请为客户分配正确的权限，以将计算机对象加入域。 所需的权限：创建计算机对象、删除计算机对象。|
|adJoinCheckUnknownError|由于未知错误，活动域加入检查失败。 请联系客户支持。|
|endpointConnectivityCheckCloudPcUrlNotAllowListed|终结点连接检查失败，因为 CPC 设置脚本存储 URL 不在网络防火墙设置中的允许列表中。 请将 URL 添加到允许的网络防火墙设置列表中。 可以在其他信息中找到 URL。|
|endpointConnectivityCheckWVDUrlNotAllowListed|终结点连接检查失败，因为 WVD URL 不在网络防火墙设置中的允许列表中。 请将 URL 添加到允许的网络防火墙设置列表中。|
|endpointConnectivityCheckIntuneUrlNotAllowListed|终结点连接检查失败，因为 Intune URL 不在网络防火墙设置中的允许列表上。 请将 URL 添加到允许的网络防火墙设置列表中。|
|endpointConnectivityCheckUnknownError|由于未知错误，终结点连接检查失败。 请联系客户支持。|
|aadConnectivityCheckUnknownError|由于Azure Active Directory未知，连接检查失败。 请联系客户支持。|
|resourceAvailabilityCheckNoSubnetIP|资源可用性检查失败，因为子网中没有任何可用的 IP 地址。 请释放部分或更改为其他子网，然后重试。|
|resourceAvailabilityCheckSubscriptionDisabled|由于已禁用 Azure 订阅，资源可用性检查失败。 请重新启用订阅。|
|resourceAvailabilityCheckAzurePolicyViolation|创建所需的 Azure 资源失败，因为组织的 Azure 策略阻止了该操作。 请更新 Azure 策略以允许创建此资源。|
|resourceAvailabilityCheckUnsupportedVNetRegion|所选 vNet 不在受支持的 Azure 区域。|
|resourceAvailabilityCheckUnknownError|由于未知错误，资源可用性检查失败。 请联系客户支持。|
|permissionCheckNoSubscriptionReaderRole|云电脑服务主体对指定的 Azure 订阅没有读者权限。 请与订阅所有者合作，在角色分配 Azure 订阅上添加读卡器。|
|permissionCheckNoResourceGroupOwnerRole|云电脑服务主体对指定的资源组没有所有者权限。 Please work with the subscription owner to add owner 角色分配 on the resource group for the Cloud PC service principal.|
|permissionCheckNoVNetContributorRole|云电脑服务主体对指定的虚拟网络没有网络参与者权限。 请与订阅所有者合作，为云电脑角色分配添加网络参与者。 |
|permissionCheckUnknownError|由于未知错误，权限检查失败。 请联系客户支持。|
|internalServerErrorDeploymentCanceled|部署已取消。 请稍后重试。 如果问题仍然存在，请联系支持人员。|
|internalServerErrorAllocateResourceFailed|资源分配失败。 请重试，或联系支持人员了解更多详细信息。|
|internalServerErrorVMDeploymentTimeout|虚拟机部署已过。再试一次。 如果问题仍然存在，请联系支持人员。|
|internalServerErrorUnableToRunDscScript|无法在运行状况检查期间运行 DSC 脚本。 该服务需要访问 WinRM 才能成功预配云电脑。 请确保没有任何组策略或相关配置阻止使用 PowerShell/DSC。|
|internalServerUnknownError|由于内部服务器错误未知，运行状况检查失败。 请联系客户支持。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
  "displayName": "String",
  "status": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "errorType": "String",
  "recommendedAction": "String",
  "additionalDetails": "String"
}
```
