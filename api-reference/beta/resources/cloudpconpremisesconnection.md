---
title: cloudPcOnPremisesConnection 资源类型
description: 表示 Azure 资源信息的定义集合，可用于为云电脑建立本地网络连接。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ec7a3dfaee2f1e111b81bc551f427764fce50f1b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159610"
---
# <a name="cloudpconpremisesconnection-resource-type"></a><span data-ttu-id="3b1b4-103">cloudPcOnPremisesConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b1b4-103">cloudPcOnPremisesConnection resource type</span></span>

<span data-ttu-id="3b1b4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b1b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b1b4-105">表示 Azure 资源信息的定义集合，可用于为云电脑建立本地网络连接。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-105">Represents a defined collection of Azure resource information that can be used to establish on-premises network connectivity for cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="3b1b4-106">方法</span><span class="sxs-lookup"><span data-stu-id="3b1b4-106">Methods</span></span>

|<span data-ttu-id="3b1b4-107">方法</span><span class="sxs-lookup"><span data-stu-id="3b1b4-107">Method</span></span>|<span data-ttu-id="3b1b4-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3b1b4-108">Return type</span></span>|<span data-ttu-id="3b1b4-109">说明</span><span class="sxs-lookup"><span data-stu-id="3b1b4-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3b1b4-110">列出 onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="3b1b4-110">List onPremisesConnections</span></span>](../api/virtualendpoint-list-onpremisesconnections.md)|<span data-ttu-id="3b1b4-111">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b1b4-111">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="3b1b4-112">列出 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-112">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>|
|[<span data-ttu-id="3b1b4-113">获取 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="3b1b4-113">Get cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-get.md)|[<span data-ttu-id="3b1b4-114">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="3b1b4-114">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="3b1b4-115">读取 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-115">Read the properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="3b1b4-116">创建 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="3b1b4-116">Create cloudPcOnPremisesConnection</span></span>](../api/virtualendpoint-post-onpremisesconnections.md)|[<span data-ttu-id="3b1b4-117">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="3b1b4-117">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="3b1b4-118">创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-118">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="3b1b4-119">更新 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="3b1b4-119">Update cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-update.md)|[<span data-ttu-id="3b1b4-120">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="3b1b4-120">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="3b1b4-121">更新 [cloudPcOnPremisesConnection 对象](../resources/cloudpconpremisesconnection.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-121">Update the properties of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="3b1b4-122">删除 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="3b1b4-122">Delete cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-delete.md)|<span data-ttu-id="3b1b4-123">无</span><span class="sxs-lookup"><span data-stu-id="3b1b4-123">None</span></span>|<span data-ttu-id="3b1b4-124">删除 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-124">Delete a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span> <span data-ttu-id="3b1b4-125">不能删除使用的连接。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-125">You can’t delete an connection that’s in use.</span></span>|
|[<span data-ttu-id="3b1b4-126">CloudPcOnPremisesConnection 的 RunHealthChecks</span><span class="sxs-lookup"><span data-stu-id="3b1b4-126">RunHealthChecks of cloudPcOnPremisesConnection</span></span>](../api/cloudpconpremisesconnection-runhealthcheck.md)|<span data-ttu-id="3b1b4-127">无</span><span class="sxs-lookup"><span data-stu-id="3b1b4-127">None</span></span>|<span data-ttu-id="3b1b4-128">对 [cloudPcOnPremisesConnection 运行运行状况检查](../resources/cloudpconpremisesconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-128">Run health checks on the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>|
|[<span data-ttu-id="3b1b4-129">updateAdDomainPassword</span><span class="sxs-lookup"><span data-stu-id="3b1b4-129">updateAdDomainPassword</span></span>](../api/cloudpconpremisesconnection-updateaddomainpassword.md)|<span data-ttu-id="3b1b4-130">无</span><span class="sxs-lookup"><span data-stu-id="3b1b4-130">None</span></span>|<span data-ttu-id="3b1b4-131">更新成功 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)的 AD 域密码。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-131">Update AD domain password for a successful [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="3b1b4-132">属性</span><span class="sxs-lookup"><span data-stu-id="3b1b4-132">Properties</span></span>

|<span data-ttu-id="3b1b4-133">属性</span><span class="sxs-lookup"><span data-stu-id="3b1b4-133">Property</span></span>|<span data-ttu-id="3b1b4-134">类型</span><span class="sxs-lookup"><span data-stu-id="3b1b4-134">Type</span></span>|<span data-ttu-id="3b1b4-135">说明</span><span class="sxs-lookup"><span data-stu-id="3b1b4-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b1b4-136">id</span><span class="sxs-lookup"><span data-stu-id="3b1b4-136">id</span></span>|<span data-ttu-id="3b1b4-137">String</span><span class="sxs-lookup"><span data-stu-id="3b1b4-137">String</span></span>|<span data-ttu-id="3b1b4-138">本地连接的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-138">Unique identifier for the on-premises connection.</span></span> <span data-ttu-id="3b1b4-139">只读。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-139">Read-only.</span></span>|
|<span data-ttu-id="3b1b4-140">displayName</span><span class="sxs-lookup"><span data-stu-id="3b1b4-140">displayName</span></span>|<span data-ttu-id="3b1b4-141">String</span><span class="sxs-lookup"><span data-stu-id="3b1b4-141">String</span></span>|<span data-ttu-id="3b1b4-142">本地显示名称的基础结构。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-142">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="3b1b4-143">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="3b1b4-143">subscriptionId</span></span>|<span data-ttu-id="3b1b4-144">String</span><span class="sxs-lookup"><span data-stu-id="3b1b4-144">String</span></span>|<span data-ttu-id="3b1b4-145">与租户关联的目标 Azure 订阅的 ID。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-145">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="3b1b4-146">subscriptionName</span><span class="sxs-lookup"><span data-stu-id="3b1b4-146">subscriptionName</span></span>|<span data-ttu-id="3b1b4-147">String</span><span class="sxs-lookup"><span data-stu-id="3b1b4-147">String</span></span>|<span data-ttu-id="3b1b4-148">目标 Azure 订阅的名称。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-148">The name of the target Azure subscription.</span></span> <span data-ttu-id="3b1b4-149">只读。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-149">Read-only.</span></span>|
|<span data-ttu-id="3b1b4-150">adDomainName</span><span class="sxs-lookup"><span data-stu-id="3b1b4-150">adDomainName</span></span>|<span data-ttu-id="3b1b4-151">String</span><span class="sxs-lookup"><span data-stu-id="3b1b4-151">String</span></span>|<span data-ttu-id="3b1b4-152">要加入的 Active Directory (的 FQDN) 完全限定域名。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-152">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="3b1b4-153">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="3b1b4-153">adDomainUsername</span></span>|<span data-ttu-id="3b1b4-154">String</span><span class="sxs-lookup"><span data-stu-id="3b1b4-154">String</span></span>|<span data-ttu-id="3b1b4-155">Active Directory 帐户的用户名 (拥有在 Active Directory) 创建计算机对象的权限的用户或服务帐户。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-155">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="3b1b4-156">所需格式：admin@contoso.com。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-156">Required format: admin@contoso.com.</span></span>|
|<span data-ttu-id="3b1b4-157">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="3b1b4-157">adDomainPassword</span></span>|<span data-ttu-id="3b1b4-158">String</span><span class="sxs-lookup"><span data-stu-id="3b1b4-158">String</span></span>|<span data-ttu-id="3b1b4-159">与 adDomainUsername 关联的密码。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-159">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="3b1b4-160">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="3b1b4-160">organizationalUnit</span></span>|<span data-ttu-id="3b1b4-161">String</span><span class="sxs-lookup"><span data-stu-id="3b1b4-161">String</span></span>|<span data-ttu-id="3b1b4-162">创建计算机 (OU) 组织单位。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-162">The organizational unit (OU) in which the computer account is created.</span></span> <span data-ttu-id="3b1b4-163">如果留空，则使用配置为默认的 OU (Active Directory 域) OU (中配置) 计算机对象容器。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-163">If left null, the OU that’s configured as the default (a well-known computer object container) in your Active Directory domain (OU) is used.</span></span> <span data-ttu-id="3b1b4-164">可选。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-164">Optional.</span></span>|
|<span data-ttu-id="3b1b4-165">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="3b1b4-165">resourceGroupId</span></span>|<span data-ttu-id="3b1b4-166">String</span><span class="sxs-lookup"><span data-stu-id="3b1b4-166">String</span></span>|<span data-ttu-id="3b1b4-167">目标资源组的 ID。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-167">The ID of the target resource group.</span></span> <span data-ttu-id="3b1b4-168">必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}"。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-168">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="3b1b4-169">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="3b1b4-169">virtualNetworkId</span></span>|<span data-ttu-id="3b1b4-170">String</span><span class="sxs-lookup"><span data-stu-id="3b1b4-170">String</span></span>|<span data-ttu-id="3b1b4-171">目标虚拟网络的 ID。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-171">The ID of the target virtual network.</span></span> <span data-ttu-id="3b1b4-172">必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}"。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-172">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="3b1b4-173">subnetId</span><span class="sxs-lookup"><span data-stu-id="3b1b4-173">subnetId</span></span>|<span data-ttu-id="3b1b4-174">String</span><span class="sxs-lookup"><span data-stu-id="3b1b4-174">String</span></span>|<span data-ttu-id="3b1b4-175">目标子网的 ID。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-175">The ID of the target subnet.</span></span> <span data-ttu-id="3b1b4-176">必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}"。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-176">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|
|<span data-ttu-id="3b1b4-177">healthCheckStatus</span><span class="sxs-lookup"><span data-stu-id="3b1b4-177">healthCheckStatus</span></span>|[<span data-ttu-id="3b1b4-178">cloudPcOnPremisesConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="3b1b4-178">cloudPcOnPremisesConnectionStatus</span></span>](#cloudpconpremisesconnectionstatus-values)|<span data-ttu-id="3b1b4-179">在本地连接上完成的最新运行状况检查的状态。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-179">The status of the most recent health check done on the on-premises connection.</span></span> <span data-ttu-id="3b1b4-180">例如，如果状态为"passed"，则本地连接已通过服务运行的所有检查。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-180">For example, if status is "passed", the on-premises connection has passed all checks run by the service.</span></span> <span data-ttu-id="3b1b4-181">可取值为：`pending`、`running`、`passed`、`failed`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-181">Possible values are: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`.</span></span> <span data-ttu-id="3b1b4-182">只读。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-182">Read-only.</span></span>|
|<span data-ttu-id="3b1b4-183">healthCheckStatusDetails</span><span class="sxs-lookup"><span data-stu-id="3b1b4-183">healthCheckStatusDetails</span></span>|[<span data-ttu-id="3b1b4-184">cloudPcOnPremisesConnectionStatusDetails</span><span class="sxs-lookup"><span data-stu-id="3b1b4-184">cloudPcOnPremisesConnectionStatusDetails</span></span>](../resources/cloudpconpremisesconnectionstatusdetails.md)|<span data-ttu-id="3b1b4-185">连接运行状况检查的详细信息和相应的结果。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-185">The details of the connection's health checks and the corresponding results.</span></span> <span data-ttu-id="3b1b4-186">仅返回 `$select` 。有关演示如何获取 **inUse** 属性的示例，请参阅示例 2：获取本地连接的选定属性，包括 [healthCheckStatusDetails。](../api/cloudpconpremisesconnection-get.md)</span><span class="sxs-lookup"><span data-stu-id="3b1b4-186">Returned only on `$select`.For an example that shows how to get the **inUse** property, see [Example 2: Get the selected properties of an on-premises connection, including healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md).</span></span> <span data-ttu-id="3b1b4-187">只读。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-187">Read-only.</span></span>|
|<span data-ttu-id="3b1b4-188">inUse</span><span class="sxs-lookup"><span data-stu-id="3b1b4-188">inUse</span></span>|<span data-ttu-id="3b1b4-189">布尔</span><span class="sxs-lookup"><span data-stu-id="3b1b4-189">Boolean</span></span>|<span data-ttu-id="3b1b4-190">When `true` ， the on-premises connection is in use.</span><span class="sxs-lookup"><span data-stu-id="3b1b4-190">When `true`, the on-premises connection is in use.</span></span> <span data-ttu-id="3b1b4-191">When `false` ， the connection is not in use.</span><span class="sxs-lookup"><span data-stu-id="3b1b4-191">When `false`, the connection is not in use.</span></span> <span data-ttu-id="3b1b4-192">不能删除使用的连接。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-192">You cannot delete a connection that’s in use.</span></span> <span data-ttu-id="3b1b4-193">仅在 `$select` 上返回。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-193">Returned only on `$select`.</span></span> <span data-ttu-id="3b1b4-194">有关演示如何获取 **inUse** 属性的示例，请参阅示例 2：获取本地连接的选定属性，包括 [healthCheckStatusDetails。](../api/cloudpconpremisesconnection-get.md)</span><span class="sxs-lookup"><span data-stu-id="3b1b4-194">For an example that shows how to get the **inUse** property, see [Example 2: Get the selected properties of an on-premises connection, including healthCheckStatusDetails](../api/cloudpconpremisesconnection-get.md).</span></span> <span data-ttu-id="3b1b4-195">只读。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-195">Read-only.</span></span>|

### <a name="cloudpconpremisesconnectionstatus-values"></a><span data-ttu-id="3b1b4-196">cloudPcOnPremisesConnectionStatus 值</span><span class="sxs-lookup"><span data-stu-id="3b1b4-196">cloudPcOnPremisesConnectionStatus values</span></span>

|<span data-ttu-id="3b1b4-197">成员</span><span class="sxs-lookup"><span data-stu-id="3b1b4-197">Member</span></span>|<span data-ttu-id="3b1b4-198">说明</span><span class="sxs-lookup"><span data-stu-id="3b1b4-198">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3b1b4-199">挂起</span><span class="sxs-lookup"><span data-stu-id="3b1b4-199">pending</span></span>|<span data-ttu-id="3b1b4-200">已创建并等待运行状况检查。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-200">Created and waiting for health checks.</span></span>
|<span data-ttu-id="3b1b4-201">running</span><span class="sxs-lookup"><span data-stu-id="3b1b4-201">running</span></span>|<span data-ttu-id="3b1b4-202">运行状况检查正在运行。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-202">Health checks are running.</span></span>|
|<span data-ttu-id="3b1b4-203">passed</span><span class="sxs-lookup"><span data-stu-id="3b1b4-203">passed</span></span>|<span data-ttu-id="3b1b4-204">运行状况检查通过。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-204">Health checks passed.</span></span>|
|<span data-ttu-id="3b1b4-205">failed</span><span class="sxs-lookup"><span data-stu-id="3b1b4-205">failed</span></span>|<span data-ttu-id="3b1b4-206">运行状况检查失败。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-206">Health checks failed.</span></span>|
|<span data-ttu-id="3b1b4-207">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="3b1b4-207">unknownFutureValue</span></span>|<span data-ttu-id="3b1b4-208">保留的 (未知状态，当前未) 。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-208">Unknown future status (reserved, not used right now).</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b1b4-209">关系</span><span class="sxs-lookup"><span data-stu-id="3b1b4-209">Relationships</span></span>

<span data-ttu-id="3b1b4-210">无。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-210">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b1b4-211">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b1b4-211">JSON representation</span></span>

<span data-ttu-id="3b1b4-212">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b1b4-212">The following is a JSON representation of the resource.</span></span>
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
