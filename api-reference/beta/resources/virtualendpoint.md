---
title: virtualEndpoint 资源类型
description: VirtualEndpoint 资源表示云 PC 管理功能的容器。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7e29e59658914e0f07af7635979e1b8938b99491
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563945"
---
# <a name="virtualendpoint-resource-type"></a><span data-ttu-id="16976-103">virtualEndpoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="16976-103">virtualEndpoint resource type</span></span>

<span data-ttu-id="16976-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16976-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16976-105">VirtualEndpoint 资源表示用于管理云电脑的 Api 容器。</span><span class="sxs-lookup"><span data-stu-id="16976-105">The virtualEndpoint resource represents a container for APIs to manage cloud PC.</span></span>

<span data-ttu-id="16976-106">使用云 PC API 为组织中的员工设置和管理虚拟桌面。</span><span class="sxs-lookup"><span data-stu-id="16976-106">Use the cloud PC API to provision and manage virtual desktops for employees in an organization.</span></span> <span data-ttu-id="16976-107">将其与 [INTUNE API](../resources/intune-graph-overview.md) 结合使用，以管理物理终结点和虚拟终结点。</span><span class="sxs-lookup"><span data-stu-id="16976-107">Use it in conjunction with the [Intune API](../resources/intune-graph-overview.md) to manage physical and virtual endpoints.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="methods"></a><span data-ttu-id="16976-108">方法</span><span class="sxs-lookup"><span data-stu-id="16976-108">Methods</span></span>

|<span data-ttu-id="16976-109">方法</span><span class="sxs-lookup"><span data-stu-id="16976-109">Method</span></span>|<span data-ttu-id="16976-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="16976-110">Return type</span></span>|<span data-ttu-id="16976-111">说明</span><span class="sxs-lookup"><span data-stu-id="16976-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="16976-112">获取有效权限</span><span class="sxs-lookup"><span data-stu-id="16976-112">Get effective permissions</span></span>](../api/virtualendpoint-geteffectivepermissions.md)|<span data-ttu-id="16976-113">字符串集合</span><span class="sxs-lookup"><span data-stu-id="16976-113">String collection</span></span>|<span data-ttu-id="16976-114">查看当前经过身份验证的用户的有效权限。</span><span class="sxs-lookup"><span data-stu-id="16976-114">View the effective permissions of the currently authenticated user.</span></span>|
|[<span data-ttu-id="16976-115">列出 cloudPCs</span><span class="sxs-lookup"><span data-stu-id="16976-115">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="16976-116">[cloudPC](../resources/cloudpc.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16976-116">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="16976-117">列出 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="16976-117">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="16976-118">列出 deviceImages</span><span class="sxs-lookup"><span data-stu-id="16976-118">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="16976-119">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16976-119">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="16976-120">列出 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="16976-120">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="16976-121">创建 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="16976-121">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="16976-122">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="16976-122">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="16976-123">创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="16976-123">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="16976-124">列出 onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="16976-124">List onPremisesConnections</span></span>](../api/virtualendpoint-list-onpremisesconnections.md)|<span data-ttu-id="16976-125">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16976-125">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="16976-126">列出 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="16976-126">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>|
|[<span data-ttu-id="16976-127">创建 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="16976-127">Create cloudPcOnPremisesConnection</span></span>](../api/virtualendpoint-post-onpremisesconnections.md)|[<span data-ttu-id="16976-128">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="16976-128">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="16976-129">创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="16976-129">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="16976-130">列出 provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="16976-130">List provisioningPolicies</span></span>](../api/virtualendpoint-list-provisioningpolicies.md)|<span data-ttu-id="16976-131">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16976-131">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="16976-132">列出 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="16976-132">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>|
|[<span data-ttu-id="16976-133">创建 cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="16976-133">Create cloudPcProvisioningPolicy</span></span>](../api/virtualendpoint-post-provisioningpolicies.md)|[<span data-ttu-id="16976-134">cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="16976-134">cloudPcProvisioningPolicy</span></span>](../resources/cloudpcprovisioningpolicy.md)|<span data-ttu-id="16976-135">创建新的 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="16976-135">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="16976-136">属性</span><span class="sxs-lookup"><span data-stu-id="16976-136">Properties</span></span>

|<span data-ttu-id="16976-137">属性</span><span class="sxs-lookup"><span data-stu-id="16976-137">Property</span></span>|<span data-ttu-id="16976-138">类型</span><span class="sxs-lookup"><span data-stu-id="16976-138">Type</span></span>|<span data-ttu-id="16976-139">说明</span><span class="sxs-lookup"><span data-stu-id="16976-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16976-140">id</span><span class="sxs-lookup"><span data-stu-id="16976-140">id</span></span>|<span data-ttu-id="16976-141">String</span><span class="sxs-lookup"><span data-stu-id="16976-141">String</span></span>|<span data-ttu-id="16976-142">虚拟终结点 id 的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="16976-142">The unique identifier for the virtual endpoint id. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16976-143">关系</span><span class="sxs-lookup"><span data-stu-id="16976-143">Relationships</span></span>

|<span data-ttu-id="16976-144">关系</span><span class="sxs-lookup"><span data-stu-id="16976-144">Relationship</span></span>|<span data-ttu-id="16976-145">类型</span><span class="sxs-lookup"><span data-stu-id="16976-145">Type</span></span>|<span data-ttu-id="16976-146">说明</span><span class="sxs-lookup"><span data-stu-id="16976-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16976-147">cloudPCs</span><span class="sxs-lookup"><span data-stu-id="16976-147">cloudPCs</span></span>|<span data-ttu-id="16976-148">[cloudPC](../resources/cloudpc.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16976-148">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="16976-149">云托管虚拟桌面。</span><span class="sxs-lookup"><span data-stu-id="16976-149">Cloud managed virtual desktops.</span></span>|
|<span data-ttu-id="16976-150">deviceImages</span><span class="sxs-lookup"><span data-stu-id="16976-150">deviceImages</span></span>|<span data-ttu-id="16976-151">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16976-151">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="16976-152">云电脑上的图像资源。</span><span class="sxs-lookup"><span data-stu-id="16976-152">The image resource on cloud PC.</span></span>|
|<span data-ttu-id="16976-153">onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="16976-153">onPremisesConnections</span></span>|<span data-ttu-id="16976-154">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16976-154">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="16976-155">可用于为云电脑建立本地网络连接的 Azure 资源信息的已定义集合。</span><span class="sxs-lookup"><span data-stu-id="16976-155">A defined collection of Azure resource information that can be used to establish on-premises network connectivity for cloud PCs.</span></span>|
|<span data-ttu-id="16976-156">provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="16976-156">provisioningPolicies</span></span>|<span data-ttu-id="16976-157">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="16976-157">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="16976-158">云电脑预配策略。</span><span class="sxs-lookup"><span data-stu-id="16976-158">cloud PC provisioning policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16976-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16976-159">JSON representation</span></span>

<span data-ttu-id="16976-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16976-160">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.virtualEndpoint",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.virtualEndpoint",
  "id": "string"
}
```
