---
title: cloudPcOnPremisesConnectionHealthCheck 资源类型
description: 云电脑本地连接运行状况检查的结果。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 32b57750400e1fb71dc8cc173b364fba76cd36ec
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033979"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a>cloudPcOnPremisesConnectionHealthCheck 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

云电脑本地连接运行状况检查的结果。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[CloudPcOnPremisesConnection 的 RunHealthChecks](../api/cloudpconpremisesconnection-runhealthcheck.md)|无|运行 [cloudPcOnPremisesConnection 的运行状况检查](../resources/cloudpconpremisesconnection.md)。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|此显示名称检查项目的详细信息。|
|状态|[cloudPcOnPremisesConnectionStatus](../resources/cloudpconpremisesconnection.md#cloudpconpremisesconnectionstatus-values)|运行状况检查项目的状态。 可取值为：`pending`、`running`、`passed`、`failed`、`unknownFutureValue`。 只读。|
|startDateTime|DateTimeOffset|运行状况检查项目的开始时间。 只读。|
|endDateTime|DateTimeOffset|运行状况检查项目的结束时间。 只读。|
|errorType|[cloudPcOnPremisesConnectionHealthCheckErrorType](#cloudpconpremisesconnectionhealthcheckerrortype-values)|在此运行状况检查期间发生的错误类型。|
|recommendedAction|String|修复相应错误的建议操作。|
|additionalDetails|String|有关运行状况检查或建议操作的其他详细信息。|

### <a name="cloudpconpremisesconnectionhealthcheckerrortype-values"></a>cloudPcOnPremisesConnectionHealthCheckErrorType 值

|成员|说明|
|:---|:---|
|dnsCheckFqdnNotFound|DNS 检查失败，因为找不到完全限定的域名。 请重新输入完全限定的域名。|
|dnsCheckUnknownError|由于未知错误，DNS 检查失败。 请联系客户支持人员。|
|adJoinCheckFqdnNotFound|活动域加入检查失败，因为找不到完全限定的域名。 请重新输入完全限定的域名。|
|adJoinCheckIncorrectCredentials|活动域加入检查失败，因为域凭据不正确。 请更新用户名和密码。|
|adJoinCheckOrganizationalUnitNotFound|活动域加入检查失败，因为找不到指定的组织单位。 请重新输入组织单位。|
|adJoinCheckOrganizationalUnitIncorrectFormat|由于指定组织单位的格式不正确，活动域加入检查失败。 示例格式："OU=OU1，OU=OU2，OU=OU3，DC=DC1"。|
|adJoinCheckUnknownError|由于未知错误，活动域加入检查失败。 请联系客户支持人员。|
|endpointConnectivityCheckUrlNotWhitelisted|终结点连接检查失败，因为 URL 不在网络防火墙设置中的允许列表上。 请将 URL 添加到网络防火墙设置的允许列表。 有关 [URL 信息，请参阅](/azure/virtual-desktop/safe-url-list) 所需的 URL 列表。|
|endpointConnectivityCheckUnknownError|由于未知错误，终结点连接检查失败。 请联系客户支持人员。|
|aadConnectivityCheckUnknownError|由于未知错误，Azure Active Directory 连接检查失败。 请联系客户支持人员。|
|resourceAvailabilityCheckNoSubnetIP|资源可用性检查失败，因为子网中没有任何可用的 IP 地址。 请释放部分或更改为其他子网，然后重试。|
|resourceAvailabilityCheckSubscriptionDisabled|由于已禁用 Azure 订阅，资源可用性检查失败。 请重新启用订阅。|
|resourceAvailabilityCheckUnknownError|由于未知错误，资源可用性检查失败。 请联系客户支持人员。|
|permissionCheckNoSubscriptionReaderRole|云电脑服务主体对指定的 Azure 订阅没有读者权限。 Please work with subscription owner to add reader 角色分配 on the Azure subscription for the Cloud PC service principal.|
|permissionCheckNoResourceGroupOwnerRole|云电脑服务主体对指定的资源组没有所有者权限。 请与订阅所有者合作，将所有者角色分配云电脑服务主体的资源组。|
|permissionCheckNoVNetContributorRole|云电脑服务主体对指定的虚拟网络没有网络参与者权限。 请与订阅所有者合作，为云角色分配添加网络参与者。 |
|permissionCheckUnknownError|由于未知错误，权限检查失败。 请联系客户支持人员。|
|internalServerUnknownError|由于未知内部服务器错误，运行状况检查失败。 请联系客户支持人员。|

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
