---
title: virtualEndpoint 资源类型
description: virtualEndpoint 资源表示云电脑管理功能的容器。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ea76f9267bc9be33c88a4d6a615f2fe881a3b193
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156677"
---
# <a name="virtualendpoint-resource-type"></a><span data-ttu-id="72fd1-103">virtualEndpoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="72fd1-103">virtualEndpoint resource type</span></span>

<span data-ttu-id="72fd1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72fd1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72fd1-105">virtualEndpoint 资源表示 API 用于管理云电脑的容器。</span><span class="sxs-lookup"><span data-stu-id="72fd1-105">The virtualEndpoint resource represents a container for APIs to manage cloud PC.</span></span>

<span data-ttu-id="72fd1-106">使用云电脑 API 为组织的员工预配和管理虚拟桌面。</span><span class="sxs-lookup"><span data-stu-id="72fd1-106">Use the cloud PC API to provision and manage virtual desktops for employees in an organization.</span></span> <span data-ttu-id="72fd1-107">将它与 [Intune API](../resources/intune-graph-overview.md) 结合使用，以管理物理和虚拟终结点。</span><span class="sxs-lookup"><span data-stu-id="72fd1-107">Use it in conjunction with the [Intune API](../resources/intune-graph-overview.md) to manage physical and virtual endpoints.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="methods"></a><span data-ttu-id="72fd1-108">方法</span><span class="sxs-lookup"><span data-stu-id="72fd1-108">Methods</span></span>

|<span data-ttu-id="72fd1-109">方法</span><span class="sxs-lookup"><span data-stu-id="72fd1-109">Method</span></span>|<span data-ttu-id="72fd1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="72fd1-110">Return type</span></span>|<span data-ttu-id="72fd1-111">说明</span><span class="sxs-lookup"><span data-stu-id="72fd1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="72fd1-112">获取有效权限</span><span class="sxs-lookup"><span data-stu-id="72fd1-112">Get effective permissions</span></span>](../api/virtualendpoint-geteffectivepermissions.md)|<span data-ttu-id="72fd1-113">字符串集合</span><span class="sxs-lookup"><span data-stu-id="72fd1-113">String collection</span></span>|<span data-ttu-id="72fd1-114">查看当前经过身份验证的用户的有效权限。</span><span class="sxs-lookup"><span data-stu-id="72fd1-114">View the effective permissions of the currently authenticated user.</span></span>|
|[<span data-ttu-id="72fd1-115">列出 cloudPCs</span><span class="sxs-lookup"><span data-stu-id="72fd1-115">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="72fd1-116">[cloudPC](../resources/cloudpc.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72fd1-116">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="72fd1-117">列出 cloudPC 对象 [的属性和](../resources/cloudpc.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="72fd1-117">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="72fd1-118">列出 deviceImages</span><span class="sxs-lookup"><span data-stu-id="72fd1-118">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="72fd1-119">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72fd1-119">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="72fd1-120">列出 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="72fd1-120">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="72fd1-121">创建 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="72fd1-121">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="72fd1-122">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="72fd1-122">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="72fd1-123">创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72fd1-123">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="72fd1-124">列出 onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="72fd1-124">List onPremisesConnections</span></span>](../api/virtualendpoint-list-onpremisesconnections.md)|<span data-ttu-id="72fd1-125">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72fd1-125">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="72fd1-126">列出 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="72fd1-126">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>|
|[<span data-ttu-id="72fd1-127">创建 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="72fd1-127">Create cloudPcOnPremisesConnection</span></span>](../api/virtualendpoint-post-onpremisesconnections.md)|[<span data-ttu-id="72fd1-128">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="72fd1-128">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="72fd1-129">创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72fd1-129">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="72fd1-130">列出 provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="72fd1-130">List provisioningPolicies</span></span>](../api/virtualendpoint-list-provisioningpolicies.md)|<span data-ttu-id="72fd1-131">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72fd1-131">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="72fd1-132">列出 [cloudPcProvisioningPolicy 对象的属性和](../resources/cloudpcprovisioningpolicy.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="72fd1-132">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>|
|[<span data-ttu-id="72fd1-133">创建 cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="72fd1-133">Create cloudPcProvisioningPolicy</span></span>](../api/virtualendpoint-post-provisioningpolicies.md)|[<span data-ttu-id="72fd1-134">cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="72fd1-134">cloudPcProvisioningPolicy</span></span>](../resources/cloudpcprovisioningpolicy.md)|<span data-ttu-id="72fd1-135">创建新的 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72fd1-135">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="72fd1-136">属性</span><span class="sxs-lookup"><span data-stu-id="72fd1-136">Properties</span></span>

|<span data-ttu-id="72fd1-137">属性</span><span class="sxs-lookup"><span data-stu-id="72fd1-137">Property</span></span>|<span data-ttu-id="72fd1-138">类型</span><span class="sxs-lookup"><span data-stu-id="72fd1-138">Type</span></span>|<span data-ttu-id="72fd1-139">说明</span><span class="sxs-lookup"><span data-stu-id="72fd1-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72fd1-140">id</span><span class="sxs-lookup"><span data-stu-id="72fd1-140">id</span></span>|<span data-ttu-id="72fd1-141">String</span><span class="sxs-lookup"><span data-stu-id="72fd1-141">String</span></span>|<span data-ttu-id="72fd1-142">虚拟终结点 ID 的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="72fd1-142">The unique identifier for the virtual endpoint id. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72fd1-143">关系</span><span class="sxs-lookup"><span data-stu-id="72fd1-143">Relationships</span></span>

|<span data-ttu-id="72fd1-144">关系</span><span class="sxs-lookup"><span data-stu-id="72fd1-144">Relationship</span></span>|<span data-ttu-id="72fd1-145">类型</span><span class="sxs-lookup"><span data-stu-id="72fd1-145">Type</span></span>|<span data-ttu-id="72fd1-146">说明</span><span class="sxs-lookup"><span data-stu-id="72fd1-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72fd1-147">cloudPCs</span><span class="sxs-lookup"><span data-stu-id="72fd1-147">cloudPCs</span></span>|<span data-ttu-id="72fd1-148">[cloudPC](../resources/cloudpc.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72fd1-148">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="72fd1-149">云托管虚拟桌面。</span><span class="sxs-lookup"><span data-stu-id="72fd1-149">Cloud managed virtual desktops.</span></span>|
|<span data-ttu-id="72fd1-150">deviceImages</span><span class="sxs-lookup"><span data-stu-id="72fd1-150">deviceImages</span></span>|<span data-ttu-id="72fd1-151">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72fd1-151">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="72fd1-152">云电脑上的图像资源。</span><span class="sxs-lookup"><span data-stu-id="72fd1-152">The image resource on cloud PC.</span></span>|
|<span data-ttu-id="72fd1-153">onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="72fd1-153">onPremisesConnections</span></span>|<span data-ttu-id="72fd1-154">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72fd1-154">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="72fd1-155">Azure 资源信息的定义集合，可用于为云电脑建立本地网络连接。</span><span class="sxs-lookup"><span data-stu-id="72fd1-155">A defined collection of Azure resource information that can be used to establish on-premises network connectivity for cloud PCs.</span></span>|
|<span data-ttu-id="72fd1-156">provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="72fd1-156">provisioningPolicies</span></span>|<span data-ttu-id="72fd1-157">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72fd1-157">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="72fd1-158">云电脑预配策略。</span><span class="sxs-lookup"><span data-stu-id="72fd1-158">cloud PC provisioning policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72fd1-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72fd1-159">JSON representation</span></span>

<span data-ttu-id="72fd1-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72fd1-160">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.virtualEndpoint",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.virtualEndpoint",
  "id": "string"
}
```
