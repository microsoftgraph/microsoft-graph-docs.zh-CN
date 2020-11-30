---
title: cloudPcOnPremisesConnectionHealthCheck 资源类型
description: 云 PC 本地连接运行状况检查的结果。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 188d9db2dbef3b3e731e0c95a48f6637e3e00101
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378286"
---
# <a name="cloudpconpremisesconnectionhealthcheck-resource-type"></a><span data-ttu-id="c2bbb-103">cloudPcOnPremisesConnectionHealthCheck 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2bbb-103">cloudPcOnPremisesConnectionHealthCheck resource type</span></span>

<span data-ttu-id="c2bbb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2bbb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c2bbb-105">云 PC 本地连接运行状况检查的结果。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-105">The result of a cloud PC on-premises connection health check.</span></span>

## <a name="methods"></a><span data-ttu-id="c2bbb-106">Methods</span><span class="sxs-lookup"><span data-stu-id="c2bbb-106">Methods</span></span>

|<span data-ttu-id="c2bbb-107">方法</span><span class="sxs-lookup"><span data-stu-id="c2bbb-107">Method</span></span>|<span data-ttu-id="c2bbb-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c2bbb-108">Return type</span></span>|<span data-ttu-id="c2bbb-109">说明</span><span class="sxs-lookup"><span data-stu-id="c2bbb-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c2bbb-110">RunHealthChecks of cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="c2bbb-110">RunHealthChecks of cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-runhealthcheck.md)|<span data-ttu-id="c2bbb-111">无</span><span class="sxs-lookup"><span data-stu-id="c2bbb-111">None</span></span>|<span data-ttu-id="c2bbb-112">运行 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)的运行状况检查。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-112">Run the health checks of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="c2bbb-113">属性</span><span class="sxs-lookup"><span data-stu-id="c2bbb-113">Properties</span></span>

|<span data-ttu-id="c2bbb-114">属性</span><span class="sxs-lookup"><span data-stu-id="c2bbb-114">Property</span></span>|<span data-ttu-id="c2bbb-115">类型</span><span class="sxs-lookup"><span data-stu-id="c2bbb-115">Type</span></span>|<span data-ttu-id="c2bbb-116">说明</span><span class="sxs-lookup"><span data-stu-id="c2bbb-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2bbb-117">displayName</span><span class="sxs-lookup"><span data-stu-id="c2bbb-117">displayName</span></span>|<span data-ttu-id="c2bbb-118">字符串</span><span class="sxs-lookup"><span data-stu-id="c2bbb-118">String</span></span>|<span data-ttu-id="c2bbb-119">此运行状况检查项的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-119">The display name for this health check item.</span></span>|
|<span data-ttu-id="c2bbb-120">status</span><span class="sxs-lookup"><span data-stu-id="c2bbb-120">status</span></span>|<span data-ttu-id="c2bbb-121">cloudPcOnPremisesConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="c2bbb-121">cloudPcOnPremisesConnectionStatus</span></span>|<span data-ttu-id="c2bbb-122">运行状况检查项的状态。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-122">The status of the health check item.</span></span> <span data-ttu-id="c2bbb-123">只读。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-123">Read-only.</span></span> <span data-ttu-id="c2bbb-124">可取值为：`Pending`、`Running`、`Passed`、`Failed`、`UnknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-124">Possible values are: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.</span></span>|
|<span data-ttu-id="c2bbb-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c2bbb-125">startDateTime</span></span>|<span data-ttu-id="c2bbb-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2bbb-126">DateTimeOffset</span></span>|<span data-ttu-id="c2bbb-127">运行状况检查项的开始时间。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-127">The start time of the health check item.</span></span> <span data-ttu-id="c2bbb-128">只读。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-128">Read-only.</span></span>|
|<span data-ttu-id="c2bbb-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c2bbb-129">endDateTime</span></span>|<span data-ttu-id="c2bbb-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2bbb-130">DateTimeOffset</span></span>|<span data-ttu-id="c2bbb-131">运行状况检查项的结束时间。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-131">The end time of the health check item.</span></span> <span data-ttu-id="c2bbb-132">只读。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-132">Read-only.</span></span>|
|<span data-ttu-id="c2bbb-133">errorType</span><span class="sxs-lookup"><span data-stu-id="c2bbb-133">errorType</span></span>|<span data-ttu-id="c2bbb-134">cloudPcOnPremisesConnectionHealthCheckErrorType</span><span class="sxs-lookup"><span data-stu-id="c2bbb-134">cloudPcOnPremisesConnectionHealthCheckErrorType</span></span>|<span data-ttu-id="c2bbb-135">在此运行状况检查过程中发生的错误的类型。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-135">The type of error that occurred during this health check.</span></span> <span data-ttu-id="c2bbb-136">可取值为：`DnsCheckFqdnNotFound`、`DnsCheckUnknownError`、`AdJoinCheckFqdnNotFound`、`AdJoinCheckIncorrectCredentials`、`AdJoinCheckOrganizationalUnitNotFound`、`AdJoinCheckOrganizationalUnitIncorrectFormat`、`AdJoinCheckUnknownError`、`EndpointConnectivityCheckUrlNotWhitelisted`、`EndpointConnectivityCheckUnknownError`、`AadConnectivityCheckUnknownError`。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-136">Possible values are: `DnsCheckFqdnNotFound`, `DnsCheckUnknownError`, `AdJoinCheckFqdnNotFound`, `AdJoinCheckIncorrectCredentials`, `AdJoinCheckOrganizationalUnitNotFound`, `AdJoinCheckOrganizationalUnitIncorrectFormat`, `AdJoinCheckUnknownError`, `EndpointConnectivityCheckUrlNotWhitelisted`, `EndpointConnectivityCheckUnknownError`, `AadConnectivityCheckUnknownError`.</span></span>|
|<span data-ttu-id="c2bbb-137">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="c2bbb-137">recommendedAction</span></span>|<span data-ttu-id="c2bbb-138">字符串</span><span class="sxs-lookup"><span data-stu-id="c2bbb-138">String</span></span>|<span data-ttu-id="c2bbb-139">建议用于修复相应错误的操作。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-139">The recommended action to fix the corresponding error.</span></span>|
|<span data-ttu-id="c2bbb-140">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="c2bbb-140">additionalDetails</span></span>|<span data-ttu-id="c2bbb-141">字符串</span><span class="sxs-lookup"><span data-stu-id="c2bbb-141">String</span></span>|<span data-ttu-id="c2bbb-142">有关运行状况检查或建议操作的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-142">Additional details about the health check or the recommended action.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2bbb-143">关系</span><span class="sxs-lookup"><span data-stu-id="c2bbb-143">Relationships</span></span>

<span data-ttu-id="c2bbb-144">无。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2bbb-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2bbb-145">JSON representation</span></span>

<span data-ttu-id="c2bbb-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2bbb-146">The following is a JSON representation of the resource.</span></span>
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
