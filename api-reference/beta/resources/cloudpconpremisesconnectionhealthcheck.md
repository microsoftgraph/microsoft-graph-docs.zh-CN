---
title: cloudPcOnPremisesConnectionHealthCheck 资源类型
description: 云电脑本地连接运行状况检查的结果。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: b1b1010c22bed8de73b5d3fa2caf680f26091d00
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351088"
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
|displayName|字符串|此显示名称检查项目的详细信息。|
|状态|[cloudPcOnPremisesConnectionStatus](../resources/cloudpconpremisesconnection.md#cloudpconpremisesconnectionstatus-values)|运行状况检查项目的状态。 可取值为：`pending`、`running`、`passed`、`failed`、`unknownFutureValue`。 只读。|
|startDateTime|DateTimeOffset|运行状况检查项目的开始时间。 只读。|
|endDateTime|DateTimeOffset|运行状况检查项目的结束时间。 只读。|
|errorType|[cloudPcOnPremisesConnectionHealthCheckErrorType](#cloudpconpremisesconnectionhealthcheckerrortype-values)|此运行状况检查期间发生的错误类型。|
|recommendedAction|字符串|修复相应错误的推荐操作。|
|additionalDetails|字符串|有关运行状况检查或建议操作的其他详细信息。|

### <a name="cloudpconpremisesconnectionhealthcheckerrortype-values"></a>cloudPcOnPremisesConnectionHealthCheckErrorType 值

|成员|说明|
|:---|:---|
|dnsCheckFqdnNotFound|域名的 DNS 解析失败。 可能的错误原因：1. 指定的 Azure vNet DNS 服务器无法解析域名。 请使用相应的 DNS 服务器更新 vNet;2. 提供的域名不存在或不正确。 请使用正确的域名更新本地网络连接。 请确保本地网络连接中定义的 vNet 可以解析域名。|
|dnsCheckUnknownError|域名的 DNS 解析失败。 可能的错误原因：1. 指定的 Azure vNet DNS 服务器无法解析域名。 请使用相应的 DNS 服务器更新 vNet;2. 提供的域名不存在或不正确。 请使用正确的域名更新本地网络连接。 请确保本地网络连接中定义的 vNet 可以解析域名。|
|adJoinCheckFqdnNotFound|域加入检查失败，因为找不到域名。 请确保域名的域控制器可通过本地网络连接中定义的 vNet 联系。|
|adJoinCheckIncorrectCredentials|域加入检查失败，因为为域提供的凭据不正确。 请使用正确的凭据更新本地网络连接。|
|adJoinCheckOrganizationalUnitNotFound|域加入检查失败，因为找不到 (OU) 组织单位。 请在域中提供 OU。 OU 必须采用可分辨名称格式。 示例格式："OU=OU1，OU=OU2，OU=OU3，DC=DC1"。|
|adJoinCheckOrganizationalUnitIncorrectFormat|域加入检查失败，因为找不到 (OU) 组织单位。 请在域中提供 OU。 OU 必须采用可分辨名称格式。 示例格式："OU=OU1，OU=OU2，OU=OU3，DC=DC1"。|
|adJoinCheckComputerObjectAlreadyExists|在本地网络连接中提供 (OU) 找不到计算机帐户，但域中已存在计算机名称。 这通常发生在计算机对象从内部部署网络连接中配置的 OU 中移出之后。 请将计算机对象移回目标 OU。|
|adJoinCheckAccessDenied|域加入检查失败，因为提供的用户帐户没有足够的权限加入域。 请确保提供的帐户具有足够的权限或更改在本地网络连接属性中定义的用户帐户。 所需的权限：*创建计算机对象和**删除计算机对象*。|
|adJoinCheckUnknownError|由于未知错误，域加入检查失败。 请确保本地网络连接可以使用提供的详细信息成功加入域。|
|endpointConnectivityCheckCloudPcUrlNotAllowListed|预配期间，无法联系一个或多个所需的 URL。 请确保所有所需的 URL 都可以通过防火墙和代理。|
|endpointConnectivityCheckWVDUrlNotAllowListed|预配期间，无法联系一个或多个所需的 WVD URL。 请确保所有所需的 URL 都可以通过防火墙和代理。|
|endpointConnectivityCheckIntuneUrlNotAllowListed|预配期间，无法联系一个或多个所需的 Intune URL。 请确保所有所需的 URL 都可以通过防火墙和代理。|
|endpointConnectivityCheckUnknownError|预配期间，无法联系一个或多个所需的 URL。 请确保所有所需的 URL 都可以通过防火墙和代理。|
|azureAdDeviceSyncCheckDeviceNotFound|在 Azure AD Azure Active Directory (找不到云电脑) 。 请确保 Azure AD 连接频繁工作并同步，以便云电脑计算机对象同步到 Azure AD。 必须最近 60 分钟内启用和同步 Azure AD 设备同步。|
|azureAdDeviceSyncCheckLongSyncCircle|检查云电脑计算机对象是否已同步到 Azure AD Azure Active Directory (已) 已退出。请确保 Azure AD 连接频繁工作并同步，以便云电脑计算机对象同步到 Azure AD。 必须最近 60 分钟内启用和同步 Azure AD 设备同步。|
|azureAdDeviceSyncCheckUnknownError|混合Azure Active Directory (Azure AD) 连接检查失败。 请确保 Azure AD 连接频繁工作并同步，以便云电脑计算机对象同步到 Azure AD。 必须最近 60 分钟内启用和同步 Azure AD 设备同步。|
|resourceAvailabilityCheckNoSubnetIP|提供的子网没有可用的 IP 地址。 请确保本地网络连接中提供的子网具有足够的可用 IP 地址。 请展开当前选定的子网或选择要用于设置的不同子网。|
|resourceAvailabilityCheckSubscriptionDisabled|提供的 Azure 订阅已禁用。 请确保 Azure 订阅已启用且可用于预配。|
|resourceAvailabilityCheckAzurePolicyViolation|找不到提供的 Azure 订阅。 请确保 Azure 订阅可用于预配。|
|resourceAvailabilityCheckUnsupportedVNetRegion|所选 vNet 位于不受支持的区域。 请确保所选 vNet 位于受支持的区域。|
|resourceAvailabilityCheckUnknownError|由于未知错误，Azure 资源的资源可用性检查失败。 请确保所有 Azure 资源都满足先决条件。|
|permissionCheckNoSubscriptionReaderRole|云电脑服务主体对 Azure 订阅的权限不足。 请确保云电脑服务主体对订阅具有 *读者* 权限。|
|permissionCheckNoResourceGroupOwnerRole|云电脑服务主体对 Azure 资源组的权限不足。 请确保云电脑服务主体对资源组具有所有者权限。 |
|permissionCheckNoVNetContributorRole|云电脑服务主体在 Azure vNet 上没有足够的权限。 请确保云电脑服务在 vNet 上具有网络参与者权限。|
|permissionCheckUnknownError|云电脑服务主体没有足够的权限。 请确保向云电脑服务主体授予了足够的 Azure 权限。|
|internalServerErrorDeploymentCanceled|部署已取消。 请稍后重试。 如果问题仍然存在，请联系支持人员。|
|internalServerErrorAllocateResourceFailed|资源分配失败。 请稍后重试。 如果问题仍然存在，请联系支持人员。|
|internalServerErrorVMDeploymentTimeout|虚拟机部署已过。请稍后重试。 如果问题仍然存在，请联系支持人员。|
|internalServerErrorUnableToRunDscScript|预配期间，某些 PowerShell DSC 脚本在云电脑上执行。 无法在运行状况检查期间下载或执行这些 DSC 脚本。 请确保 vNet 可以不受限制地访问所需的终结点，并且不会在环境或组策略中阻止 PowerShell。|
|internalServerUnknownError|由于内部错误，设置失败。 请联系客户支持。|

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
