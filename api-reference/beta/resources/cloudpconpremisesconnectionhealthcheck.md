---
title: cloudPcOnPremisesConnectionHealthCheck 资源类型
description: 云电脑本地连接运行状况检查的结果。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c322d0af4e255d9438c651d81328c887da1b19a5
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870638"
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
|adJoinCheckOrganizationalUnitIncorrectFormat|由于指定组织单位的格式不正确，活动域加入检查失败。 示例格式："OU=OU1，OU=OU2，OU=OU3，DC=DC1"。|
|adJoinCheckAccessDenied|活动域加入检查失败，因为当委派了控制权的非管理员用户尝试将计算机对象加入域控制器时，访问被拒绝。 请为客户分配正确的权限，以将计算机对象加入域。 所需的权限：创建计算机对象、删除计算机对象。|
|adJoinCheckUnknownError|由于未知错误，活动域加入检查失败。 请联系客户支持。|
|endpointConnectivityCheckCloudPcUrlNotAllowListed|终结点连接检查失败，因为 CPC 设置脚本存储 URL 不在网络防火墙设置中的允许列表中。 请将 URL 添加到允许的网络防火墙设置列表中。 可以在其他信息中找到 URL。|
|endpointConnectivityCheckWVDUrlNotAllowListed|终结点连接检查失败，因为 WVD URL 不在网络防火墙设置中的允许列表中。 请将 URL 添加到允许的网络防火墙设置列表中。|
|endpointConnectivityCheckIntuneUrlNotAllowListed|终结点连接检查失败，因为 Intune URL 不在网络防火墙设置中的允许列表上。 请将 URL 添加到允许的网络防火墙设置列表中。|
|endpointConnectivityCheckUnknownError|由于未知错误，终结点连接检查失败。 请联系客户支持。|
|aadConnectivityCheckUnknownError|由于Azure Active Directory未知，连接检查失败。 请联系客户支持。|
|resourceAvailabilityCheckNoSubnetIP|资源可用性检查失败，因为子网中没有任何可用的 IP 地址。 请释放部分或更改为其他子网，然后重试。|
|resourceAvailabilityCheckSubscriptionDisabled|由于已禁用 Azure 订阅，资源可用性检查失败。 请重新启用订阅。|
|resourceAvailabilityCheckUnsupportedVNetRegion|所选 vNet 不在受支持的 Azure 区域。|
|resourceAvailabilityCheckUnknownError|由于未知错误，资源可用性检查失败。 请联系客户支持。|
|permissionCheckNoSubscriptionReaderRole|Cloud PC服务主体对指定的 Azure 订阅没有读者权限。 请与订阅所有者合作，在 azure 角色分配服务主体的 Azure 订阅Cloud PC读者。|
|permissionCheckNoResourceGroupOwnerRole|Cloud PC服务主体对指定的资源组没有所有者权限。 Please work with the subscription owner to add owner 角色分配 on the resource group for the Cloud PC service principal.|
|permissionCheckNoVNetContributorRole|Cloud PC服务主体对指定的虚拟网络没有网络参与者权限。 请与订阅所有者合作，为服务主体角色分配网络Cloud PC参与者。 |
|permissionCheckUnknownError|由于未知错误，权限检查失败。 请联系客户支持。|
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
