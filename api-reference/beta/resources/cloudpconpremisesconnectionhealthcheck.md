---
title: cloudPcOnPremisesConnectionHealthCheck 资源类型
description: 云电脑本地连接运行状况检查的结果。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: e79f73bbe1a493e581a35db5fec396d752ff08d1
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844604"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a><span data-ttu-id="7c7bf-103">cloudPcOnPremisesConnectionHealthCheck 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c7bf-103">cloudPcOnPremisesConnectionHealthCheck resource type</span></span>

<span data-ttu-id="7c7bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c7bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c7bf-105">云电脑本地连接运行状况检查的结果。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-105">The result of a cloud PC on-premises connection health check.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="7c7bf-106">方法</span><span class="sxs-lookup"><span data-stu-id="7c7bf-106">Methods</span></span>

|<span data-ttu-id="7c7bf-107">方法</span><span class="sxs-lookup"><span data-stu-id="7c7bf-107">Method</span></span>|<span data-ttu-id="7c7bf-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="7c7bf-108">Return type</span></span>|<span data-ttu-id="7c7bf-109">说明</span><span class="sxs-lookup"><span data-stu-id="7c7bf-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7c7bf-110">CloudPcOnPremisesConnection 的 RunHealthChecks</span><span class="sxs-lookup"><span data-stu-id="7c7bf-110">RunHealthChecks of cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-runhealthcheck.md)|<span data-ttu-id="7c7bf-111">无</span><span class="sxs-lookup"><span data-stu-id="7c7bf-111">None</span></span>|<span data-ttu-id="7c7bf-112">运行 [cloudPcOnPremisesConnection 的运行状况检查](../resources/cloudpconpremisesconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-112">Run the health checks of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="7c7bf-113">属性</span><span class="sxs-lookup"><span data-stu-id="7c7bf-113">Properties</span></span>

|<span data-ttu-id="7c7bf-114">属性</span><span class="sxs-lookup"><span data-stu-id="7c7bf-114">Property</span></span>|<span data-ttu-id="7c7bf-115">类型</span><span class="sxs-lookup"><span data-stu-id="7c7bf-115">Type</span></span>|<span data-ttu-id="7c7bf-116">说明</span><span class="sxs-lookup"><span data-stu-id="7c7bf-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c7bf-117">displayName</span><span class="sxs-lookup"><span data-stu-id="7c7bf-117">displayName</span></span>|<span data-ttu-id="7c7bf-118">String</span><span class="sxs-lookup"><span data-stu-id="7c7bf-118">String</span></span>|<span data-ttu-id="7c7bf-119">此显示名称检查项目的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-119">The display name for this health check item.</span></span>|
|<span data-ttu-id="7c7bf-120">status</span><span class="sxs-lookup"><span data-stu-id="7c7bf-120">status</span></span>|<span data-ttu-id="7c7bf-121">cloudPcOnPremisesConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="7c7bf-121">cloudPcOnPremisesConnectionStatus</span></span>|<span data-ttu-id="7c7bf-122">运行状况检查项目的状态。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-122">The status of the health check item.</span></span> <span data-ttu-id="7c7bf-123">只读。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-123">Read-only.</span></span> <span data-ttu-id="7c7bf-124">可取值为：`Pending`、`Running`、`Passed`、`Failed`、`UnknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-124">Possible values are: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.</span></span>|
|<span data-ttu-id="7c7bf-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7c7bf-125">startDateTime</span></span>|<span data-ttu-id="7c7bf-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c7bf-126">DateTimeOffset</span></span>|<span data-ttu-id="7c7bf-127">运行状况检查项目的开始时间。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-127">The start time of the health check item.</span></span> <span data-ttu-id="7c7bf-128">只读。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-128">Read-only.</span></span>|
|<span data-ttu-id="7c7bf-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7c7bf-129">endDateTime</span></span>|<span data-ttu-id="7c7bf-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c7bf-130">DateTimeOffset</span></span>|<span data-ttu-id="7c7bf-131">运行状况检查项目的结束时间。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-131">The end time of the health check item.</span></span> <span data-ttu-id="7c7bf-132">只读。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-132">Read-only.</span></span>|
|<span data-ttu-id="7c7bf-133">errorType</span><span class="sxs-lookup"><span data-stu-id="7c7bf-133">errorType</span></span>|<span data-ttu-id="7c7bf-134">cloudPcOnPremisesConnectionHealthCheckErrorType</span><span class="sxs-lookup"><span data-stu-id="7c7bf-134">cloudPcOnPremisesConnectionHealthCheckErrorType</span></span>|<span data-ttu-id="7c7bf-135">在此运行状况检查期间发生的错误类型。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-135">The type of error that occurred during this health check.</span></span> <span data-ttu-id="7c7bf-136">可能的值是： `DnsCheckFqdnNotFound` ， `DnsCheckUnknownError` `AdJoinCheckFqdnNotFound` `AdJoinCheckIncorrectCredentials` `AdJoinCheckOrganizationalUnitNotFound` `AdJoinCheckOrganizationalUnitIncorrectFormat` `AdJoinCheckUnknownError` `EndpointConnectivityCheckUrlNotWhitelisted` `EndpointConnectivityCheckUnknownError` `AadConnectivityCheckUnknownError` `ResourceAvailabilityCheckNoSubnetIP` `resourceAvailabilityCheckSubscriptionDisabled` `resourceAvailabilityCheckUnknownError` `permissionCheckNoSubscriptionReaderRole` `permissionCheckNoResourceGroupOwnerRole` `permissionCheckNoVNetContributorRole` `permissionCheckUnknownError` `internalServerUnknownError` 。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-136">Possible values are: `DnsCheckFqdnNotFound`, `DnsCheckUnknownError`, `AdJoinCheckFqdnNotFound`, `AdJoinCheckIncorrectCredentials`, `AdJoinCheckOrganizationalUnitNotFound`, `AdJoinCheckOrganizationalUnitIncorrectFormat`, `AdJoinCheckUnknownError`, `EndpointConnectivityCheckUrlNotWhitelisted`, `EndpointConnectivityCheckUnknownError`, `AadConnectivityCheckUnknownError`, `ResourceAvailabilityCheckNoSubnetIP`, `resourceAvailabilityCheckSubscriptionDisabled`, `resourceAvailabilityCheckUnknownError`,`permissionCheckNoSubscriptionReaderRole`, `permissionCheckNoResourceGroupOwnerRole`, `permissionCheckNoVNetContributorRole`, `permissionCheckUnknownError`, `internalServerUnknownError`.</span></span>|
|<span data-ttu-id="7c7bf-137">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="7c7bf-137">recommendedAction</span></span>|<span data-ttu-id="7c7bf-138">String</span><span class="sxs-lookup"><span data-stu-id="7c7bf-138">String</span></span>|<span data-ttu-id="7c7bf-139">修复相应错误的建议操作。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-139">The recommended action to fix the corresponding error.</span></span>|
|<span data-ttu-id="7c7bf-140">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="7c7bf-140">additionalDetails</span></span>|<span data-ttu-id="7c7bf-141">String</span><span class="sxs-lookup"><span data-stu-id="7c7bf-141">String</span></span>|<span data-ttu-id="7c7bf-142">有关运行状况检查或建议操作的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-142">Additional details about the health check or the recommended action.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c7bf-143">关系</span><span class="sxs-lookup"><span data-stu-id="7c7bf-143">Relationships</span></span>

<span data-ttu-id="7c7bf-144">无。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c7bf-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c7bf-145">JSON representation</span></span>

<span data-ttu-id="7c7bf-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c7bf-146">The following is a JSON representation of the resource.</span></span>
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
