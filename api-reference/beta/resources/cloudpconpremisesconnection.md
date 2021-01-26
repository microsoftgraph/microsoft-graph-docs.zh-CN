---
title: cloudPcOnPremisesConnection 资源类型
description: 表示 Azure 资源信息的定义集合，可用于为云电脑建立本地网络连接。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 88143f58c070f7a359fab7bb0674fa6a39477d91
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982731"
---
# <a name="cloudpconpremisesconnection-resource-type"></a><span data-ttu-id="c282b-103">cloudPcOnPremisesConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="c282b-103">cloudPcOnPremisesConnection resource type</span></span>

<span data-ttu-id="c282b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c282b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c282b-105">表示 Azure 资源信息的定义集合，可用于为云电脑建立本地网络连接。</span><span class="sxs-lookup"><span data-stu-id="c282b-105">Represents a defined collection of Azure resource information that can be used to establish on-premises network connectivity for cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="c282b-106">方法</span><span class="sxs-lookup"><span data-stu-id="c282b-106">Methods</span></span>

|<span data-ttu-id="c282b-107">方法</span><span class="sxs-lookup"><span data-stu-id="c282b-107">Method</span></span>|<span data-ttu-id="c282b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c282b-108">Return type</span></span>|<span data-ttu-id="c282b-109">说明</span><span class="sxs-lookup"><span data-stu-id="c282b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c282b-110">列出 onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="c282b-110">List onPremisesConnections</span></span>](../api/virtualendpoint-list-onpremisesconnections.md)|<span data-ttu-id="c282b-111">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c282b-111">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="c282b-112">列出 [cloudPcOnPremisesConnection 对象的属性和](../resources/cloudpconpremisesconnection.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="c282b-112">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>|
|[<span data-ttu-id="c282b-113">获取 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="c282b-113">Get cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-get.md)|[<span data-ttu-id="c282b-114">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="c282b-114">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="c282b-115">读取 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c282b-115">Read the properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="c282b-116">创建 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="c282b-116">Create cloudPcOnPremisesConnection</span></span>](../api/virtualendpoint-post-onpremisesconnections.md)|[<span data-ttu-id="c282b-117">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="c282b-117">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="c282b-118">创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c282b-118">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="c282b-119">更新 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="c282b-119">Update cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-update.md)|[<span data-ttu-id="c282b-120">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="c282b-120">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="c282b-121">更新 [cloudPcOnPremisesConnection 对象](../resources/cloudpconpremisesconnection.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="c282b-121">Update the properties of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="c282b-122">删除 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="c282b-122">Delete cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-delete.md)|<span data-ttu-id="c282b-123">无</span><span class="sxs-lookup"><span data-stu-id="c282b-123">None</span></span>|<span data-ttu-id="c282b-124">删除 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c282b-124">Delete a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span> <span data-ttu-id="c282b-125">不能删除使用的连接。</span><span class="sxs-lookup"><span data-stu-id="c282b-125">You can’t delete an connection that’s in use.</span></span>|
|[<span data-ttu-id="c282b-126">CloudPcOnPremisesConnection 的 RunHealthChecks</span><span class="sxs-lookup"><span data-stu-id="c282b-126">RunHealthChecks of cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-runhealthcheck.md)|<span data-ttu-id="c282b-127">无</span><span class="sxs-lookup"><span data-stu-id="c282b-127">None</span></span>|<span data-ttu-id="c282b-128">对 [cloudPcOnPremisesConnection 运行运行状况检查](../resources/cloudpconpremisesconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="c282b-128">Run health checks on the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>|
|[<span data-ttu-id="c282b-129">updateAdDomainPassword</span><span class="sxs-lookup"><span data-stu-id="c282b-129">updateAdDomainPassword</span></span>](../api/cloudpconpremisesconnection-updateaddomainpassword.md)|<span data-ttu-id="c282b-130">无</span><span class="sxs-lookup"><span data-stu-id="c282b-130">None</span></span>|<span data-ttu-id="c282b-131">更新成功 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)的 AD 域密码。</span><span class="sxs-lookup"><span data-stu-id="c282b-131">Update AD domain password for a successful [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="c282b-132">属性</span><span class="sxs-lookup"><span data-stu-id="c282b-132">Properties</span></span>

|<span data-ttu-id="c282b-133">属性</span><span class="sxs-lookup"><span data-stu-id="c282b-133">Property</span></span>|<span data-ttu-id="c282b-134">类型</span><span class="sxs-lookup"><span data-stu-id="c282b-134">Type</span></span>|<span data-ttu-id="c282b-135">说明</span><span class="sxs-lookup"><span data-stu-id="c282b-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c282b-136">id</span><span class="sxs-lookup"><span data-stu-id="c282b-136">id</span></span>|<span data-ttu-id="c282b-137">String</span><span class="sxs-lookup"><span data-stu-id="c282b-137">String</span></span>|<span data-ttu-id="c282b-138">本地连接的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c282b-138">Unique identifier for the on-premises connection.</span></span> <span data-ttu-id="c282b-139">只读。</span><span class="sxs-lookup"><span data-stu-id="c282b-139">Read-only.</span></span>|
|<span data-ttu-id="c282b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="c282b-140">displayName</span></span>|<span data-ttu-id="c282b-141">String</span><span class="sxs-lookup"><span data-stu-id="c282b-141">String</span></span>|<span data-ttu-id="c282b-142">本地显示名称的基础结构。</span><span class="sxs-lookup"><span data-stu-id="c282b-142">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="c282b-143">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="c282b-143">subscriptionId</span></span>|<span data-ttu-id="c282b-144">String</span><span class="sxs-lookup"><span data-stu-id="c282b-144">String</span></span>|<span data-ttu-id="c282b-145">与租户关联的目标 Azure 订阅的 ID。</span><span class="sxs-lookup"><span data-stu-id="c282b-145">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="c282b-146">subscriptionName</span><span class="sxs-lookup"><span data-stu-id="c282b-146">subscriptionName</span></span>|<span data-ttu-id="c282b-147">String</span><span class="sxs-lookup"><span data-stu-id="c282b-147">String</span></span>|<span data-ttu-id="c282b-148">目标 Azure 订阅的名称。</span><span class="sxs-lookup"><span data-stu-id="c282b-148">The name of the target Azure subscription.</span></span> <span data-ttu-id="c282b-149">只读。</span><span class="sxs-lookup"><span data-stu-id="c282b-149">Read-only.</span></span>|
|<span data-ttu-id="c282b-150">adDomainName</span><span class="sxs-lookup"><span data-stu-id="c282b-150">adDomainName</span></span>|<span data-ttu-id="c282b-151">String</span><span class="sxs-lookup"><span data-stu-id="c282b-151">String</span></span>|<span data-ttu-id="c282b-152">要加入的 Active Directory (的 FQDN) 完全限定域名。</span><span class="sxs-lookup"><span data-stu-id="c282b-152">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="c282b-153">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="c282b-153">adDomainUsername</span></span>|<span data-ttu-id="c282b-154">String</span><span class="sxs-lookup"><span data-stu-id="c282b-154">String</span></span>|<span data-ttu-id="c282b-155">Active Directory 帐户的用户名 (拥有在 Active Directory) 创建计算机对象的权限的用户或服务帐户。</span><span class="sxs-lookup"><span data-stu-id="c282b-155">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="c282b-156">所需格式：admin@contoso.com。</span><span class="sxs-lookup"><span data-stu-id="c282b-156">Required format: admin@contoso.com.</span></span>|
|<span data-ttu-id="c282b-157">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="c282b-157">adDomainPassword</span></span>|<span data-ttu-id="c282b-158">String</span><span class="sxs-lookup"><span data-stu-id="c282b-158">String</span></span>|<span data-ttu-id="c282b-159">与 adDomainUsername 关联的密码。</span><span class="sxs-lookup"><span data-stu-id="c282b-159">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="c282b-160">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="c282b-160">organizationalUnit</span></span>|<span data-ttu-id="c282b-161">String</span><span class="sxs-lookup"><span data-stu-id="c282b-161">String</span></span>|<span data-ttu-id="c282b-162">创建计算机 (OU) 组织单位。</span><span class="sxs-lookup"><span data-stu-id="c282b-162">The organizational unit (OU) in which the computer account is created.</span></span> <span data-ttu-id="c282b-163">如果留空，则使用配置为默认 ou (Active Directory 域) OU (中的已知计算机对象容器) OU。</span><span class="sxs-lookup"><span data-stu-id="c282b-163">If left null, the OU that’s configured as the default (a well-known computer object container) in your Active Directory domain (OU) is used.</span></span> <span data-ttu-id="c282b-164">可选。</span><span class="sxs-lookup"><span data-stu-id="c282b-164">Optional.</span></span>|
|<span data-ttu-id="c282b-165">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="c282b-165">resourceGroupId</span></span>|<span data-ttu-id="c282b-166">String</span><span class="sxs-lookup"><span data-stu-id="c282b-166">String</span></span>|<span data-ttu-id="c282b-167">目标资源组的 ID。</span><span class="sxs-lookup"><span data-stu-id="c282b-167">The ID of the target resource group.</span></span> <span data-ttu-id="c282b-168">必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}"。</span><span class="sxs-lookup"><span data-stu-id="c282b-168">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="c282b-169">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="c282b-169">virtualNetworkId</span></span>|<span data-ttu-id="c282b-170">String</span><span class="sxs-lookup"><span data-stu-id="c282b-170">String</span></span>|<span data-ttu-id="c282b-171">目标虚拟网络的 ID。</span><span class="sxs-lookup"><span data-stu-id="c282b-171">The ID of the target virtual network.</span></span> <span data-ttu-id="c282b-172">必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}"。</span><span class="sxs-lookup"><span data-stu-id="c282b-172">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="c282b-173">subnetId</span><span class="sxs-lookup"><span data-stu-id="c282b-173">subnetId</span></span>|<span data-ttu-id="c282b-174">String</span><span class="sxs-lookup"><span data-stu-id="c282b-174">String</span></span>|<span data-ttu-id="c282b-175">目标子网的 ID。</span><span class="sxs-lookup"><span data-stu-id="c282b-175">The ID of the target subnet.</span></span> <span data-ttu-id="c282b-176">必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}"。</span><span class="sxs-lookup"><span data-stu-id="c282b-176">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|
|<span data-ttu-id="c282b-177">healthCheckStatus</span><span class="sxs-lookup"><span data-stu-id="c282b-177">healthCheckStatus</span></span>|<span data-ttu-id="c282b-178">cloudPcOnPremisesConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="c282b-178">cloudPcOnPremisesConnectionStatus</span></span>|<span data-ttu-id="c282b-179">在本地连接上完成的最新运行状况检查的状态。</span><span class="sxs-lookup"><span data-stu-id="c282b-179">The status of the most recent health check done on the on-premises connection.</span></span> <span data-ttu-id="c282b-180">例如，如果状态为"passed"，则本地连接已通过服务运行的所有检查。</span><span class="sxs-lookup"><span data-stu-id="c282b-180">For example, if status is "passed", the on-premises connection has passed all checks run by the service.</span></span> <span data-ttu-id="c282b-181">只读。</span><span class="sxs-lookup"><span data-stu-id="c282b-181">Read-only.</span></span> <span data-ttu-id="c282b-182">可取值为：`Pending`、`Running`、`Passed`、`Failed`、`UnknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c282b-182">Possible values are: `Pending`, `Running`, `Passed`, `Failed`, `UnknownFutureValue`.</span></span>|
|<span data-ttu-id="c282b-183">healthCheckStatusDetails</span><span class="sxs-lookup"><span data-stu-id="c282b-183">healthCheckStatusDetails</span></span>|[<span data-ttu-id="c282b-184">cloudPcOnPremisesConnectionStatusDetails</span><span class="sxs-lookup"><span data-stu-id="c282b-184">cloudPcOnPremisesConnectionStatusDetails</span></span>](../resources/cloudpconpremisesconnectionstatusdetails.md)|<span data-ttu-id="c282b-185">连接运行状况检查的详细信息和相应的结果。</span><span class="sxs-lookup"><span data-stu-id="c282b-185">The details of the connection's health checks and the corresponding results.</span></span> <span data-ttu-id="c282b-186">仅在 `$select` 上返回。</span><span class="sxs-lookup"><span data-stu-id="c282b-186">Returned only on `$select`.</span></span> <span data-ttu-id="c282b-187">请参阅 [获取](../api/cloudpconpremisesconnection-get.md) healthCheckStatusDetails 属性的示例。只读。</span><span class="sxs-lookup"><span data-stu-id="c282b-187">See an [example](../api/cloudpconpremisesconnection-get.md) of getting the healthCheckStatusDetails property.Read-only.</span></span>|
|<span data-ttu-id="c282b-188">inUse</span><span class="sxs-lookup"><span data-stu-id="c282b-188">inUse</span></span>|<span data-ttu-id="c282b-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="c282b-189">Boolean</span></span>|<span data-ttu-id="c282b-190">如果为 true，则使用本地连接。</span><span class="sxs-lookup"><span data-stu-id="c282b-190">When true, the on-premises connection is in use.</span></span> <span data-ttu-id="c282b-191">如果为 false，则不使用连接。</span><span class="sxs-lookup"><span data-stu-id="c282b-191">When false, the connection is not in use.</span></span> <span data-ttu-id="c282b-192">不能删除使用的连接。</span><span class="sxs-lookup"><span data-stu-id="c282b-192">You cannot delete a connection that’s in use.</span></span> <span data-ttu-id="c282b-193">只读。</span><span class="sxs-lookup"><span data-stu-id="c282b-193">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c282b-194">关系</span><span class="sxs-lookup"><span data-stu-id="c282b-194">Relationships</span></span>

<span data-ttu-id="c282b-195">无。</span><span class="sxs-lookup"><span data-stu-id="c282b-195">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c282b-196">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c282b-196">JSON representation</span></span>

<span data-ttu-id="c282b-197">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c282b-197">The following is a JSON representation of the resource.</span></span>
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
