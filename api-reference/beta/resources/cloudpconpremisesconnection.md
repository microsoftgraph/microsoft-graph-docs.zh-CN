---
title: cloudPcOnPremisesConnection 资源类型
description: 表示一个定义的 Azure 资源信息集合，可用于为云电脑建立本地网络连接。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7090679e0f35f182c7966fc9810b4698d090e002
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870645"
---
# <a name="cloudpconpremisesconnection-resource-type"></a><span data-ttu-id="2cdb0-103">cloudPcOnPremisesConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="2cdb0-103">cloudPcOnPremisesConnection resource type</span></span>

<span data-ttu-id="2cdb0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cdb0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cdb0-105">表示一个定义的 Azure 资源信息集合，可用于为云电脑建立本地网络连接。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-105">Represents a defined collection of Azure resource information that can be used to establish on-premises network connectivity for cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="2cdb0-106">方法</span><span class="sxs-lookup"><span data-stu-id="2cdb0-106">Methods</span></span>

|<span data-ttu-id="2cdb0-107">方法</span><span class="sxs-lookup"><span data-stu-id="2cdb0-107">Method</span></span>|<span data-ttu-id="2cdb0-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="2cdb0-108">Return type</span></span>|<span data-ttu-id="2cdb0-109">说明</span><span class="sxs-lookup"><span data-stu-id="2cdb0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2cdb0-110">列出 onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="2cdb0-110">List onPremisesConnections</span></span>](../api/virtualendpoint-list-onpremisesconnections.md)|<span data-ttu-id="2cdb0-111">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2cdb0-111">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="2cdb0-112">列出 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-112">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>|
|[<span data-ttu-id="2cdb0-113">获取 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="2cdb0-113">Get cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-get.md)|[<span data-ttu-id="2cdb0-114">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="2cdb0-114">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="2cdb0-115">读取 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-115">Read the properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="2cdb0-116">创建 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="2cdb0-116">Create cloudPcOnPremisesConnection</span></span>](../api/virtualendpoint-post-onpremisesconnections.md)|[<span data-ttu-id="2cdb0-117">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="2cdb0-117">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="2cdb0-118">创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-118">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="2cdb0-119">更新 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="2cdb0-119">Update cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-update.md)|[<span data-ttu-id="2cdb0-120">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="2cdb0-120">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="2cdb0-121">更新 [cloudPcOnPremisesConnection 对象](../resources/cloudpconpremisesconnection.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-121">Update the properties of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="2cdb0-122">删除 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="2cdb0-122">Delete cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-delete.md)|<span data-ttu-id="2cdb0-123">无</span><span class="sxs-lookup"><span data-stu-id="2cdb0-123">None</span></span>|<span data-ttu-id="2cdb0-124">删除 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-124">Delete a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span> <span data-ttu-id="2cdb0-125">不能删除使用的连接。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-125">You can’t delete an connection that’s in use.</span></span>|
|[<span data-ttu-id="2cdb0-126">cloudPcOnPremisesConnection 的 RunHealthChecks</span><span class="sxs-lookup"><span data-stu-id="2cdb0-126">RunHealthChecks of cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-runhealthcheck.md)|<span data-ttu-id="2cdb0-127">无</span><span class="sxs-lookup"><span data-stu-id="2cdb0-127">None</span></span>|<span data-ttu-id="2cdb0-128">对 [cloudPcOnPremisesConnection 运行运行状况检查](../resources/cloudpconpremisesconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-128">Run health checks on the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>|
|[<span data-ttu-id="2cdb0-129">updateAdDomainPassword</span><span class="sxs-lookup"><span data-stu-id="2cdb0-129">updateAdDomainPassword</span></span>](../api/cloudpconpremisesconnection-updateaddomainpassword.md)|<span data-ttu-id="2cdb0-130">无</span><span class="sxs-lookup"><span data-stu-id="2cdb0-130">None</span></span>|<span data-ttu-id="2cdb0-131">更新成功 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)的 AD 域密码。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-131">Update AD domain password for a successful [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="2cdb0-132">属性</span><span class="sxs-lookup"><span data-stu-id="2cdb0-132">Properties</span></span>

|<span data-ttu-id="2cdb0-133">属性</span><span class="sxs-lookup"><span data-stu-id="2cdb0-133">Property</span></span>|<span data-ttu-id="2cdb0-134">类型</span><span class="sxs-lookup"><span data-stu-id="2cdb0-134">Type</span></span>|<span data-ttu-id="2cdb0-135">说明</span><span class="sxs-lookup"><span data-stu-id="2cdb0-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cdb0-136">id</span><span class="sxs-lookup"><span data-stu-id="2cdb0-136">id</span></span>|<span data-ttu-id="2cdb0-137">String</span><span class="sxs-lookup"><span data-stu-id="2cdb0-137">String</span></span>|<span data-ttu-id="2cdb0-138">本地连接的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-138">Unique identifier for the on-premises connection.</span></span> <span data-ttu-id="2cdb0-139">只读。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-139">Read-only.</span></span>|
|<span data-ttu-id="2cdb0-140">displayName</span><span class="sxs-lookup"><span data-stu-id="2cdb0-140">displayName</span></span>|<span data-ttu-id="2cdb0-141">String</span><span class="sxs-lookup"><span data-stu-id="2cdb0-141">String</span></span>|<span data-ttu-id="2cdb0-142">本地显示名称的基础结构。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-142">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="2cdb0-143">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="2cdb0-143">subscriptionId</span></span>|<span data-ttu-id="2cdb0-144">String</span><span class="sxs-lookup"><span data-stu-id="2cdb0-144">String</span></span>|<span data-ttu-id="2cdb0-145">与租户关联的目标 Azure 订阅的 ID。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-145">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="2cdb0-146">subscriptionName</span><span class="sxs-lookup"><span data-stu-id="2cdb0-146">subscriptionName</span></span>|<span data-ttu-id="2cdb0-147">String</span><span class="sxs-lookup"><span data-stu-id="2cdb0-147">String</span></span>|<span data-ttu-id="2cdb0-148">目标 Azure 订阅的名称。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-148">The name of the target Azure subscription.</span></span> <span data-ttu-id="2cdb0-149">只读。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-149">Read-only.</span></span>|
|<span data-ttu-id="2cdb0-150">adDomainName</span><span class="sxs-lookup"><span data-stu-id="2cdb0-150">adDomainName</span></span>|<span data-ttu-id="2cdb0-151">String</span><span class="sxs-lookup"><span data-stu-id="2cdb0-151">String</span></span>|<span data-ttu-id="2cdb0-152">要加入的 Active Directory (完全限定) FQDN。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-152">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="2cdb0-153">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="2cdb0-153">adDomainUsername</span></span>|<span data-ttu-id="2cdb0-154">String</span><span class="sxs-lookup"><span data-stu-id="2cdb0-154">String</span></span>|<span data-ttu-id="2cdb0-155">Active Directory 帐户的用户名 (拥有在 Active Directory) 创建计算机对象的权限的用户或服务帐户。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-155">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="2cdb0-156">所需格式：admin@contoso.com。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-156">Required format: admin@contoso.com.</span></span>|
|<span data-ttu-id="2cdb0-157">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="2cdb0-157">adDomainPassword</span></span>|<span data-ttu-id="2cdb0-158">String</span><span class="sxs-lookup"><span data-stu-id="2cdb0-158">String</span></span>|<span data-ttu-id="2cdb0-159">与 adDomainUsername 关联的密码。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-159">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="2cdb0-160">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="2cdb0-160">organizationalUnit</span></span>|<span data-ttu-id="2cdb0-161">String</span><span class="sxs-lookup"><span data-stu-id="2cdb0-161">String</span></span>|<span data-ttu-id="2cdb0-162">组织单位 (OU) 创建计算机帐户的组织单位。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-162">The organizational unit (OU) in which the computer account is created.</span></span> <span data-ttu-id="2cdb0-163">如果保留为 null，则使用配置为默认 ou (Active Directory 域) OU (中的已知计算机对象容器) 。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-163">If left null, the OU that’s configured as the default (a well-known computer object container) in your Active Directory domain (OU) is used.</span></span> <span data-ttu-id="2cdb0-164">可选。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-164">Optional.</span></span>|
|<span data-ttu-id="2cdb0-165">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="2cdb0-165">resourceGroupId</span></span>|<span data-ttu-id="2cdb0-166">String</span><span class="sxs-lookup"><span data-stu-id="2cdb0-166">String</span></span>|<span data-ttu-id="2cdb0-167">目标资源组的 ID。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-167">The ID of the target resource group.</span></span> <span data-ttu-id="2cdb0-168">所需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}"。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-168">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="2cdb0-169">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="2cdb0-169">virtualNetworkId</span></span>|<span data-ttu-id="2cdb0-170">String</span><span class="sxs-lookup"><span data-stu-id="2cdb0-170">String</span></span>|<span data-ttu-id="2cdb0-171">目标虚拟网络的 ID。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-171">The ID of the target virtual network.</span></span> <span data-ttu-id="2cdb0-172">所需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}"。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-172">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="2cdb0-173">subnetId</span><span class="sxs-lookup"><span data-stu-id="2cdb0-173">subnetId</span></span>|<span data-ttu-id="2cdb0-174">String</span><span class="sxs-lookup"><span data-stu-id="2cdb0-174">String</span></span>|<span data-ttu-id="2cdb0-175">目标子网的 ID。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-175">The ID of the target subnet.</span></span> <span data-ttu-id="2cdb0-176">所需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}"。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-176">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|
|<span data-ttu-id="2cdb0-177">healthCheckStatus</span><span class="sxs-lookup"><span data-stu-id="2cdb0-177">healthCheckStatus</span></span>|[<span data-ttu-id="2cdb0-178">cloudPcOnPremisesConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="2cdb0-178">cloudPcOnPremisesConnectionStatus</span></span>](#cloudpconpremisesconnectionstatus-values)|<span data-ttu-id="2cdb0-179">在本地连接上完成的最新运行状况检查的状态。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-179">The status of the most recent health check done on the on-premises connection.</span></span> <span data-ttu-id="2cdb0-180">例如，如果状态为"passed"，则本地连接已通过服务运行的所有检查。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-180">For example, if status is "passed", the on-premises connection has passed all checks run by the service.</span></span> <span data-ttu-id="2cdb0-181">可取值为：`pending`、`running`、`passed`、`failed`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-181">Possible values are: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`.</span></span> <span data-ttu-id="2cdb0-182">只读。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-182">Read-only.</span></span>|
|<span data-ttu-id="2cdb0-183">healthCheckStatusDetails</span><span class="sxs-lookup"><span data-stu-id="2cdb0-183">healthCheckStatusDetails</span></span>|[<span data-ttu-id="2cdb0-184">cloudPcOnPremisesConnectionStatusDetails</span><span class="sxs-lookup"><span data-stu-id="2cdb0-184">cloudPcOnPremisesConnectionStatusDetails</span></span>](../resources/cloudpconpremisesconnectionstatusdetails.md)|<span data-ttu-id="2cdb0-185">连接运行状况检查的详细信息和相应结果。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-185">The details of the connection's health checks and the corresponding results.</span></span> <span data-ttu-id="2cdb0-186">仅在 上返回 `$select` 。有关演示如何获取 **inUse** 属性的示例，请参阅示例 2：获取本地连接的选定属性，包括 [healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md)。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-186">Returned only on `$select`.For an example that shows how to get the **inUse** property, see [Example 2: Get the selected properties of an on-premises connection, including healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md).</span></span> <span data-ttu-id="2cdb0-187">只读。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-187">Read-only.</span></span>|
|<span data-ttu-id="2cdb0-188">inUse</span><span class="sxs-lookup"><span data-stu-id="2cdb0-188">inUse</span></span>|<span data-ttu-id="2cdb0-189">布尔</span><span class="sxs-lookup"><span data-stu-id="2cdb0-189">Boolean</span></span>|<span data-ttu-id="2cdb0-190">如果 `true` 为 ，则使用内部部署连接。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-190">When `true`, the on-premises connection is in use.</span></span> <span data-ttu-id="2cdb0-191">如果 `false` 为 ，则不使用连接。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-191">When `false`, the connection is not in use.</span></span> <span data-ttu-id="2cdb0-192">不能删除使用的连接。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-192">You cannot delete a connection that’s in use.</span></span> <span data-ttu-id="2cdb0-193">仅在 `$select` 上返回。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-193">Returned only on `$select`.</span></span> <span data-ttu-id="2cdb0-194">有关演示如何获取 **inUse** 属性的示例，请参阅示例 2：获取本地连接的选定属性，包括 [healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md)。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-194">For an example that shows how to get the **inUse** property, see [Example 2: Get the selected properties of an on-premises connection, including healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md).</span></span> <span data-ttu-id="2cdb0-195">只读。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-195">Read-only.</span></span>|

### <a name="cloudpconpremisesconnectionstatus-values"></a><span data-ttu-id="2cdb0-196">cloudPcOnPremisesConnectionStatus 值</span><span class="sxs-lookup"><span data-stu-id="2cdb0-196">cloudPcOnPremisesConnectionStatus values</span></span>

|<span data-ttu-id="2cdb0-197">成员</span><span class="sxs-lookup"><span data-stu-id="2cdb0-197">Member</span></span>|<span data-ttu-id="2cdb0-198">说明</span><span class="sxs-lookup"><span data-stu-id="2cdb0-198">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2cdb0-199">pending</span><span class="sxs-lookup"><span data-stu-id="2cdb0-199">pending</span></span>|<span data-ttu-id="2cdb0-200">已创建并等待运行状况检查。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-200">Created and waiting for health checks.</span></span>
|<span data-ttu-id="2cdb0-201">running</span><span class="sxs-lookup"><span data-stu-id="2cdb0-201">running</span></span>|<span data-ttu-id="2cdb0-202">运行状况检查正在运行。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-202">Health checks are running.</span></span>|
|<span data-ttu-id="2cdb0-203">passed</span><span class="sxs-lookup"><span data-stu-id="2cdb0-203">passed</span></span>|<span data-ttu-id="2cdb0-204">运行状况检查通过。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-204">Health checks passed.</span></span>|
|<span data-ttu-id="2cdb0-205">failed</span><span class="sxs-lookup"><span data-stu-id="2cdb0-205">failed</span></span>|<span data-ttu-id="2cdb0-206">运行状况检查失败。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-206">Health checks failed.</span></span>|
|<span data-ttu-id="2cdb0-207">警告</span><span class="sxs-lookup"><span data-stu-id="2cdb0-207">warning</span></span>|<span data-ttu-id="2cdb0-208">运行状况检查通过，并发出警告。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-208">Health checks passed with warning.</span></span>|
|<span data-ttu-id="2cdb0-209">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="2cdb0-209">unknownFutureValue</span></span>|<span data-ttu-id="2cdb0-210">未知未来状态 (保留，当前未) 。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-210">Unknown future status (reserved, not used right now).</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cdb0-211">关系</span><span class="sxs-lookup"><span data-stu-id="2cdb0-211">Relationships</span></span>

<span data-ttu-id="2cdb0-212">无。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-212">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cdb0-213">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2cdb0-213">JSON representation</span></span>

<span data-ttu-id="2cdb0-214">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2cdb0-214">The following is a JSON representation of the resource.</span></span>
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
