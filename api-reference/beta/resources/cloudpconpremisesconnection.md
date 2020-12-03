---
title: cloudPcOnPremisesConnection 资源类型
description: 表示可用于为云电脑建立本地网络连接的 Azure 资源信息的已定义集合。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 23cf853eac58ed168592da1ab4cbe45dc2028dcd
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563836"
---
# <a name="cloudpconpremisesconnection-resource-type"></a><span data-ttu-id="9debe-103">cloudPcOnPremisesConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="9debe-103">cloudPcOnPremisesConnection resource type</span></span>

<span data-ttu-id="9debe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9debe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9debe-105">表示可用于为云电脑建立本地网络连接的 Azure 资源信息的已定义集合。</span><span class="sxs-lookup"><span data-stu-id="9debe-105">Represents a defined collection of Azure resource information that can be used to establish on-premises network connectivity for cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="9debe-106">方法</span><span class="sxs-lookup"><span data-stu-id="9debe-106">Methods</span></span>

|<span data-ttu-id="9debe-107">方法</span><span class="sxs-lookup"><span data-stu-id="9debe-107">Method</span></span>|<span data-ttu-id="9debe-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9debe-108">Return type</span></span>|<span data-ttu-id="9debe-109">说明</span><span class="sxs-lookup"><span data-stu-id="9debe-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9debe-110">列出 onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="9debe-110">List onPremisesConnections</span></span>](../api/virtualendpoint-list-onpremisesconnections.md)|<span data-ttu-id="9debe-111">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9debe-111">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="9debe-112">列出 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9debe-112">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>|
|[<span data-ttu-id="9debe-113">获取 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="9debe-113">Get cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-get.md)|[<span data-ttu-id="9debe-114">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="9debe-114">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="9debe-115">读取 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9debe-115">Read the properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="9debe-116">创建 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="9debe-116">Create cloudPcOnPremisesConnection</span></span>](../api/virtualendpoint-post-onpremisesconnections.md)|[<span data-ttu-id="9debe-117">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="9debe-117">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="9debe-118">创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9debe-118">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="9debe-119">更新 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="9debe-119">Update cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-update.md)|[<span data-ttu-id="9debe-120">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="9debe-120">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="9debe-121">更新 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9debe-121">Update the properties of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="9debe-122">删除 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="9debe-122">Delete cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-delete.md)|<span data-ttu-id="9debe-123">无</span><span class="sxs-lookup"><span data-stu-id="9debe-123">None</span></span>|<span data-ttu-id="9debe-124">删除 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9debe-124">Delete a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span> <span data-ttu-id="9debe-125">无法删除正在使用的连接。</span><span class="sxs-lookup"><span data-stu-id="9debe-125">You can’t delete an connection that’s in use.</span></span>|
|[<span data-ttu-id="9debe-126">RunHealthChecks of cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="9debe-126">RunHealthChecks of cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-runhealthcheck.md)|<span data-ttu-id="9debe-127">无</span><span class="sxs-lookup"><span data-stu-id="9debe-127">None</span></span>|<span data-ttu-id="9debe-128">对 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)运行运行状况检查。</span><span class="sxs-lookup"><span data-stu-id="9debe-128">Run health checks on the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="9debe-129">属性</span><span class="sxs-lookup"><span data-stu-id="9debe-129">Properties</span></span>

|<span data-ttu-id="9debe-130">属性</span><span class="sxs-lookup"><span data-stu-id="9debe-130">Property</span></span>|<span data-ttu-id="9debe-131">类型</span><span class="sxs-lookup"><span data-stu-id="9debe-131">Type</span></span>|<span data-ttu-id="9debe-132">说明</span><span class="sxs-lookup"><span data-stu-id="9debe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9debe-133">id</span><span class="sxs-lookup"><span data-stu-id="9debe-133">id</span></span>|<span data-ttu-id="9debe-134">String</span><span class="sxs-lookup"><span data-stu-id="9debe-134">String</span></span>|<span data-ttu-id="9debe-135">本地连接的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9debe-135">Unique identifier for the on-premises connection.</span></span> <span data-ttu-id="9debe-136">只读。</span><span class="sxs-lookup"><span data-stu-id="9debe-136">Read-only.</span></span>|
|<span data-ttu-id="9debe-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9debe-137">displayName</span></span>|<span data-ttu-id="9debe-138">String</span><span class="sxs-lookup"><span data-stu-id="9debe-138">String</span></span>|<span data-ttu-id="9debe-139">本地连接的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9debe-139">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="9debe-140">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="9debe-140">subscriptionId</span></span>|<span data-ttu-id="9debe-141">String</span><span class="sxs-lookup"><span data-stu-id="9debe-141">String</span></span>|<span data-ttu-id="9debe-142">与你的租户关联的目标 Azure 订阅的 ID。</span><span class="sxs-lookup"><span data-stu-id="9debe-142">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="9debe-143">subscriptionName</span><span class="sxs-lookup"><span data-stu-id="9debe-143">subscriptionName</span></span>|<span data-ttu-id="9debe-144">String</span><span class="sxs-lookup"><span data-stu-id="9debe-144">String</span></span>|<span data-ttu-id="9debe-145">目标 Azure 订阅的名称。</span><span class="sxs-lookup"><span data-stu-id="9debe-145">The name of the target Azure subscription.</span></span> <span data-ttu-id="9debe-146">只读。</span><span class="sxs-lookup"><span data-stu-id="9debe-146">Read-only.</span></span>|
|<span data-ttu-id="9debe-147">adDomainName</span><span class="sxs-lookup"><span data-stu-id="9debe-147">adDomainName</span></span>|<span data-ttu-id="9debe-148">String</span><span class="sxs-lookup"><span data-stu-id="9debe-148">String</span></span>|<span data-ttu-id="9debe-149">要加入的 Active Directory 域 (FQDN) 的完全限定的域名称。</span><span class="sxs-lookup"><span data-stu-id="9debe-149">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="9debe-150">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="9debe-150">adDomainUsername</span></span>|<span data-ttu-id="9debe-151">String</span><span class="sxs-lookup"><span data-stu-id="9debe-151">String</span></span>|<span data-ttu-id="9debe-152">Active Directory 帐户的用户名 (用户或服务帐户) 具有在 Active Directory 中创建计算机对象的权限。</span><span class="sxs-lookup"><span data-stu-id="9debe-152">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="9debe-153">必需的格式： contoso@microsoft.com。</span><span class="sxs-lookup"><span data-stu-id="9debe-153">Required format: contoso@microsoft.com.</span></span>|
|<span data-ttu-id="9debe-154">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="9debe-154">adDomainPassword</span></span>|<span data-ttu-id="9debe-155">String</span><span class="sxs-lookup"><span data-stu-id="9debe-155">String</span></span>|<span data-ttu-id="9debe-156">与 adDomainUsername 相关联的密码。</span><span class="sxs-lookup"><span data-stu-id="9debe-156">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="9debe-157">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="9debe-157">organizationalUnit</span></span>|<span data-ttu-id="9debe-158">String</span><span class="sxs-lookup"><span data-stu-id="9debe-158">String</span></span>|<span data-ttu-id="9debe-159">在其中创建计算机帐户的组织单位 (OU) 。</span><span class="sxs-lookup"><span data-stu-id="9debe-159">The organizational unit (OU) in which the computer account is created.</span></span> <span data-ttu-id="9debe-160">如果为 null，则在使用 Active Directory 域 (OU) 中) 的已知计算机对象容器中配置为默认 (的 OU。</span><span class="sxs-lookup"><span data-stu-id="9debe-160">If left null, the OU that’s configured as the default (a well-known computer object container) in your Active Directory domain (OU) is used.</span></span> <span data-ttu-id="9debe-161">可选。</span><span class="sxs-lookup"><span data-stu-id="9debe-161">Optional.</span></span>|
|<span data-ttu-id="9debe-162">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="9debe-162">resourceGroupId</span></span>|<span data-ttu-id="9debe-163">String</span><span class="sxs-lookup"><span data-stu-id="9debe-163">String</span></span>|<span data-ttu-id="9debe-164">目标资源组的 ID。</span><span class="sxs-lookup"><span data-stu-id="9debe-164">The ID of the target resource group.</span></span> <span data-ttu-id="9debe-165">必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}"。</span><span class="sxs-lookup"><span data-stu-id="9debe-165">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="9debe-166">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="9debe-166">virtualNetworkId</span></span>|<span data-ttu-id="9debe-167">String</span><span class="sxs-lookup"><span data-stu-id="9debe-167">String</span></span>|<span data-ttu-id="9debe-168">目标虚拟网络的 ID。</span><span class="sxs-lookup"><span data-stu-id="9debe-168">The ID of the target virtual network.</span></span> <span data-ttu-id="9debe-169">必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}"。</span><span class="sxs-lookup"><span data-stu-id="9debe-169">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="9debe-170">subnetId</span><span class="sxs-lookup"><span data-stu-id="9debe-170">subnetId</span></span>|<span data-ttu-id="9debe-171">String</span><span class="sxs-lookup"><span data-stu-id="9debe-171">String</span></span>|<span data-ttu-id="9debe-172">目标子网的 ID。</span><span class="sxs-lookup"><span data-stu-id="9debe-172">The ID of the target subnet.</span></span> <span data-ttu-id="9debe-173">必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}"。</span><span class="sxs-lookup"><span data-stu-id="9debe-173">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|
|<span data-ttu-id="9debe-174">healthCheckStatus</span><span class="sxs-lookup"><span data-stu-id="9debe-174">healthCheckStatus</span></span>|<span data-ttu-id="9debe-175">cloudPcOnPremisesConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="9debe-175">cloudPcOnPremisesConnectionStatus</span></span>|<span data-ttu-id="9debe-176">对本地连接执行的最新运行状况检查的状态。</span><span class="sxs-lookup"><span data-stu-id="9debe-176">The status of the most recent health check done on the on-premises connection.</span></span> <span data-ttu-id="9debe-177">例如，如果状态为 "已传递"，则本地连接已通过该服务运行的所有检查。</span><span class="sxs-lookup"><span data-stu-id="9debe-177">For example, if status is "passed", the on-premises connection has passed all checks run by the service.</span></span> <span data-ttu-id="9debe-178">只读。</span><span class="sxs-lookup"><span data-stu-id="9debe-178">Read-only.</span></span> <span data-ttu-id="9debe-179">可取值为：`Pending`、`Running`、`Passed`、`Failed`、`UnknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="9debe-179">Possible values are: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.</span></span>|
|<span data-ttu-id="9debe-180">healthCheckStatusDetails</span><span class="sxs-lookup"><span data-stu-id="9debe-180">healthCheckStatusDetails</span></span>|[<span data-ttu-id="9debe-181">cloudPcOnPremisesConnectionStatusDetails</span><span class="sxs-lookup"><span data-stu-id="9debe-181">cloudPcOnPremisesConnectionStatusDetails</span></span>](../resources/cloudpconpremisesconnectionstatusdetails.md)|<span data-ttu-id="9debe-182">连接的运行状况检查和相应结果的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9debe-182">The details of the connection's health checks and the corresponding results.</span></span> <span data-ttu-id="9debe-183">仅在 `$select` 上返回。</span><span class="sxs-lookup"><span data-stu-id="9debe-183">Returned only on `$select`.</span></span> <span data-ttu-id="9debe-184">请参阅获取 healthCheckStatusDetails 属性的 [示例](../api/cloudpconpremisesconnection-get.md) 。只读。</span><span class="sxs-lookup"><span data-stu-id="9debe-184">See an [example](../api/cloudpconpremisesconnection-get.md) of getting the healthCheckStatusDetails property.Read-only.</span></span>|
|<span data-ttu-id="9debe-185">inUse</span><span class="sxs-lookup"><span data-stu-id="9debe-185">inUse</span></span>|<span data-ttu-id="9debe-186">布尔值</span><span class="sxs-lookup"><span data-stu-id="9debe-186">Boolean</span></span>|<span data-ttu-id="9debe-187">如果为 true，则使用内部部署连接。</span><span class="sxs-lookup"><span data-stu-id="9debe-187">When true, the on-premises connection is in use.</span></span> <span data-ttu-id="9debe-188">如果为 false，则表示未使用该连接。</span><span class="sxs-lookup"><span data-stu-id="9debe-188">When false, the connection is not in use.</span></span> <span data-ttu-id="9debe-189">无法删除正在使用的连接。</span><span class="sxs-lookup"><span data-stu-id="9debe-189">You cannot delete a connection that’s in use.</span></span> <span data-ttu-id="9debe-190">只读。</span><span class="sxs-lookup"><span data-stu-id="9debe-190">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9debe-191">关系</span><span class="sxs-lookup"><span data-stu-id="9debe-191">Relationships</span></span>

<span data-ttu-id="9debe-192">无。</span><span class="sxs-lookup"><span data-stu-id="9debe-192">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9debe-193">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9debe-193">JSON representation</span></span>

<span data-ttu-id="9debe-194">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9debe-194">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection",
  "baseType": "microsoft.graph.entity",
  "openType": false,
  "optionalProperties": ["healthCheckStatusDetails"]
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
  "id": "String (identifier)",
  "displayName": "String",
  "subscriptionId": "String",
  "subscriptionName": "String",
  "adDomainName": "String",
  "adDomainUsername": "String",
  "adDomainPassword": "String",
  "organizationalUnit": "String",
  "resourceGroupId": "String",
  "virtualNetworkId": "String",
  "subnetId": "String",
  "healthCheckStatus": "string",
  "healthCheckStatusDetails": {
    "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionStatusDetails",
    "startDateTime": "String (timestamp)",
    "endDateTime": "String (timestamp)",
    "healthChecks": [
      {
        "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
        "displayName": "String",
        "status": "String",
        "startDateTime": "String (timestamp)",
        "endDateTime": "String (timestamp)",
        "errorType": "String",
        "recommendedAction": "String",
        "additionalDetails": "String"
      }
    ]
  },
  "inUse": "Boolean"
}
```
