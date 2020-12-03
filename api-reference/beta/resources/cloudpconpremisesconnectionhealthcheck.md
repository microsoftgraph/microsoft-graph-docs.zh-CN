---
title: cloudPcOnPremisesConnectionHealthCheck 资源类型
description: 云 PC 本地连接运行状况检查的结果。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 16dea9278c9471996e4a5beaf20d5f9ec5c2d5c5
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563833"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a><span data-ttu-id="73c0c-103">cloudPcOnPremisesConnectionHealthCheck 资源类型</span><span class="sxs-lookup"><span data-stu-id="73c0c-103">cloudPcOnPremisesConnectionHealthCheck resource type</span></span>

<span data-ttu-id="73c0c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73c0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73c0c-105">云 PC 本地连接运行状况检查的结果。</span><span class="sxs-lookup"><span data-stu-id="73c0c-105">The result of a cloud PC on-premises connection health check.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="73c0c-106">方法</span><span class="sxs-lookup"><span data-stu-id="73c0c-106">Methods</span></span>

|<span data-ttu-id="73c0c-107">方法</span><span class="sxs-lookup"><span data-stu-id="73c0c-107">Method</span></span>|<span data-ttu-id="73c0c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="73c0c-108">Return type</span></span>|<span data-ttu-id="73c0c-109">说明</span><span class="sxs-lookup"><span data-stu-id="73c0c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="73c0c-110">RunHealthChecks of cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="73c0c-110">RunHealthChecks of cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-runhealthcheck.md)|<span data-ttu-id="73c0c-111">无</span><span class="sxs-lookup"><span data-stu-id="73c0c-111">None</span></span>|<span data-ttu-id="73c0c-112">运行 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)的运行状况检查。</span><span class="sxs-lookup"><span data-stu-id="73c0c-112">Run the health checks of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="73c0c-113">属性</span><span class="sxs-lookup"><span data-stu-id="73c0c-113">Properties</span></span>

|<span data-ttu-id="73c0c-114">属性</span><span class="sxs-lookup"><span data-stu-id="73c0c-114">Property</span></span>|<span data-ttu-id="73c0c-115">类型</span><span class="sxs-lookup"><span data-stu-id="73c0c-115">Type</span></span>|<span data-ttu-id="73c0c-116">说明</span><span class="sxs-lookup"><span data-stu-id="73c0c-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73c0c-117">displayName</span><span class="sxs-lookup"><span data-stu-id="73c0c-117">displayName</span></span>|<span data-ttu-id="73c0c-118">String</span><span class="sxs-lookup"><span data-stu-id="73c0c-118">String</span></span>|<span data-ttu-id="73c0c-119">此运行状况检查项的显示名称。</span><span class="sxs-lookup"><span data-stu-id="73c0c-119">The display name for this health check item.</span></span>|
|<span data-ttu-id="73c0c-120">status</span><span class="sxs-lookup"><span data-stu-id="73c0c-120">status</span></span>|<span data-ttu-id="73c0c-121">cloudPcOnPremisesConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="73c0c-121">cloudPcOnPremisesConnectionStatus</span></span>|<span data-ttu-id="73c0c-122">运行状况检查项的状态。</span><span class="sxs-lookup"><span data-stu-id="73c0c-122">The status of the health check item.</span></span> <span data-ttu-id="73c0c-123">只读。</span><span class="sxs-lookup"><span data-stu-id="73c0c-123">Read-only.</span></span> <span data-ttu-id="73c0c-124">可取值为：`Pending`、`Running`、`Passed`、`Failed`、`UnknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="73c0c-124">Possible values are: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.</span></span>|
|<span data-ttu-id="73c0c-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="73c0c-125">startDateTime</span></span>|<span data-ttu-id="73c0c-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73c0c-126">DateTimeOffset</span></span>|<span data-ttu-id="73c0c-127">运行状况检查项的开始时间。</span><span class="sxs-lookup"><span data-stu-id="73c0c-127">The start time of the health check item.</span></span> <span data-ttu-id="73c0c-128">只读。</span><span class="sxs-lookup"><span data-stu-id="73c0c-128">Read-only.</span></span>|
|<span data-ttu-id="73c0c-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="73c0c-129">endDateTime</span></span>|<span data-ttu-id="73c0c-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73c0c-130">DateTimeOffset</span></span>|<span data-ttu-id="73c0c-131">运行状况检查项的结束时间。</span><span class="sxs-lookup"><span data-stu-id="73c0c-131">The end time of the health check item.</span></span> <span data-ttu-id="73c0c-132">只读。</span><span class="sxs-lookup"><span data-stu-id="73c0c-132">Read-only.</span></span>|
|<span data-ttu-id="73c0c-133">errorType</span><span class="sxs-lookup"><span data-stu-id="73c0c-133">errorType</span></span>|<span data-ttu-id="73c0c-134">cloudPcOnPremisesConnectionHealthCheckErrorType</span><span class="sxs-lookup"><span data-stu-id="73c0c-134">cloudPcOnPremisesConnectionHealthCheckErrorType</span></span>|<span data-ttu-id="73c0c-135">在此运行状况检查过程中发生的错误的类型。</span><span class="sxs-lookup"><span data-stu-id="73c0c-135">The type of error that occurred during this health check.</span></span> <span data-ttu-id="73c0c-136">可取值为：`DnsCheckFqdnNotFound`、`DnsCheckUnknownError`、`AdJoinCheckFqdnNotFound`、`AdJoinCheckIncorrectCredentials`、`AdJoinCheckOrganizationalUnitNotFound`、`AdJoinCheckOrganizationalUnitIncorrectFormat`、`AdJoinCheckUnknownError`、`EndpointConnectivityCheckUrlNotWhitelisted`、`EndpointConnectivityCheckUnknownError`、`AadConnectivityCheckUnknownError`。</span><span class="sxs-lookup"><span data-stu-id="73c0c-136">Possible values are: `DnsCheckFqdnNotFound`, `DnsCheckUnknownError`, `AdJoinCheckFqdnNotFound`, `AdJoinCheckIncorrectCredentials`, `AdJoinCheckOrganizationalUnitNotFound`, `AdJoinCheckOrganizationalUnitIncorrectFormat`, `AdJoinCheckUnknownError`, `EndpointConnectivityCheckUrlNotWhitelisted`, `EndpointConnectivityCheckUnknownError`, `AadConnectivityCheckUnknownError`.</span></span>|
|<span data-ttu-id="73c0c-137">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="73c0c-137">recommendedAction</span></span>|<span data-ttu-id="73c0c-138">String</span><span class="sxs-lookup"><span data-stu-id="73c0c-138">String</span></span>|<span data-ttu-id="73c0c-139">建议用于修复相应错误的操作。</span><span class="sxs-lookup"><span data-stu-id="73c0c-139">The recommended action to fix the corresponding error.</span></span>|
|<span data-ttu-id="73c0c-140">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="73c0c-140">additionalDetails</span></span>|<span data-ttu-id="73c0c-141">String</span><span class="sxs-lookup"><span data-stu-id="73c0c-141">String</span></span>|<span data-ttu-id="73c0c-142">有关运行状况检查或建议操作的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="73c0c-142">Additional details about the health check or the recommended action.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73c0c-143">关系</span><span class="sxs-lookup"><span data-stu-id="73c0c-143">Relationships</span></span>

<span data-ttu-id="73c0c-144">无。</span><span class="sxs-lookup"><span data-stu-id="73c0c-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="73c0c-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73c0c-145">JSON representation</span></span>

<span data-ttu-id="73c0c-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73c0c-146">The following is a JSON representation of the resource.</span></span>
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
