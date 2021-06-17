---
title: virtualEndpoint 资源类型
description: virtualEndpoint 资源表示云电脑管理功能的容器。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 33730be63a02a383063738e681297a9b97ffdcf1
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993248"
---
# <a name="virtualendpoint-resource-type"></a><span data-ttu-id="7b23a-103">virtualEndpoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b23a-103">virtualEndpoint resource type</span></span>

<span data-ttu-id="7b23a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b23a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b23a-105">virtualEndpoint 资源表示 API 用于管理云电脑的容器。</span><span class="sxs-lookup"><span data-stu-id="7b23a-105">The virtualEndpoint resource represents a container for APIs to manage cloud PC.</span></span>

<span data-ttu-id="7b23a-106">使用云电脑 API 为组织的员工预配和管理虚拟桌面。</span><span class="sxs-lookup"><span data-stu-id="7b23a-106">Use the cloud PC API to provision and manage virtual desktops for employees in an organization.</span></span> <span data-ttu-id="7b23a-107">将它与 [Intune API](../resources/intune-graph-overview.md) 结合使用，以管理物理和虚拟终结点。</span><span class="sxs-lookup"><span data-stu-id="7b23a-107">Use it in conjunction with the [Intune API](../resources/intune-graph-overview.md) to manage physical and virtual endpoints.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="methods"></a><span data-ttu-id="7b23a-108">方法</span><span class="sxs-lookup"><span data-stu-id="7b23a-108">Methods</span></span>

|<span data-ttu-id="7b23a-109">方法</span><span class="sxs-lookup"><span data-stu-id="7b23a-109">Method</span></span>|<span data-ttu-id="7b23a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7b23a-110">Return type</span></span>|<span data-ttu-id="7b23a-111">说明</span><span class="sxs-lookup"><span data-stu-id="7b23a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7b23a-112">获取有效权限</span><span class="sxs-lookup"><span data-stu-id="7b23a-112">Get effective permissions</span></span>](../api/virtualendpoint-geteffectivepermissions.md)|<span data-ttu-id="7b23a-113">字符串集合</span><span class="sxs-lookup"><span data-stu-id="7b23a-113">String collection</span></span>|<span data-ttu-id="7b23a-114">查看当前经过身份验证的用户的有效权限。</span><span class="sxs-lookup"><span data-stu-id="7b23a-114">View the effective permissions of the currently authenticated user.</span></span>|
|[<span data-ttu-id="7b23a-115">列出 cloudPCs</span><span class="sxs-lookup"><span data-stu-id="7b23a-115">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="7b23a-116">[cloudPC](../resources/cloudpc.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b23a-116">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="7b23a-117">列出 [cloudPC 对象的属性和](../resources/cloudpc.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="7b23a-117">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="7b23a-118">列出 deviceImages</span><span class="sxs-lookup"><span data-stu-id="7b23a-118">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="7b23a-119">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b23a-119">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="7b23a-120">列出 [cloudPcDeviceImage 对象的属性和](../resources/cloudpcdeviceimage.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="7b23a-120">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="7b23a-121">创建 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="7b23a-121">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="7b23a-122">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="7b23a-122">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="7b23a-123">创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b23a-123">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="7b23a-124">列出 onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="7b23a-124">List onPremisesConnections</span></span>](../api/virtualendpoint-list-onpremisesconnections.md)|<span data-ttu-id="7b23a-125">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b23a-125">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="7b23a-126">列出 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7b23a-126">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>|
|[<span data-ttu-id="7b23a-127">创建 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="7b23a-127">Create cloudPcOnPremisesConnection</span></span>](../api/virtualendpoint-post-onpremisesconnections.md)|[<span data-ttu-id="7b23a-128">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="7b23a-128">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="7b23a-129">创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b23a-129">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="7b23a-130">列出 provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="7b23a-130">List provisioningPolicies</span></span>](../api/virtualendpoint-list-provisioningpolicies.md)|<span data-ttu-id="7b23a-131">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b23a-131">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="7b23a-132">列出 [cloudPcProvisioningPolicy 对象的属性和](../resources/cloudpcprovisioningpolicy.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="7b23a-132">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>|
|[<span data-ttu-id="7b23a-133">创建 cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="7b23a-133">Create cloudPcProvisioningPolicy</span></span>](../api/virtualendpoint-post-provisioningpolicies.md)|[<span data-ttu-id="7b23a-134">cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="7b23a-134">cloudPcProvisioningPolicy</span></span>](../resources/cloudpcprovisioningpolicy.md)|<span data-ttu-id="7b23a-135">创建新的 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7b23a-135">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>|
|[<span data-ttu-id="7b23a-136">列出 userSettings</span><span class="sxs-lookup"><span data-stu-id="7b23a-136">List userSettings</span></span>](../api/virtualendpoint-list-usersettings.md)|<span data-ttu-id="7b23a-137">[cloudPcUserSetting](../resources/cloudpcusersetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b23a-137">[cloudPcUserSetting](../resources/cloudpcusersetting.md) collection</span></span>|<span data-ttu-id="7b23a-138">从 userSettings 导航属性获取 cloudPcUserSetting 资源。</span><span class="sxs-lookup"><span data-stu-id="7b23a-138">Get the cloudPcUserSetting resources from the userSettings navigation property.</span></span>|
|[<span data-ttu-id="7b23a-139">创建 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="7b23a-139">Create cloudPcUserSetting</span></span>](../api/virtualendpoint-post-usersettings.md)|[<span data-ttu-id="7b23a-140">cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="7b23a-140">cloudPcUserSetting</span></span>](../resources/cloudpcusersetting.md)|<span data-ttu-id="7b23a-141">创建新的 cloudPcUserSetting 对象。</span><span class="sxs-lookup"><span data-stu-id="7b23a-141">Create a new cloudPcUserSetting object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b23a-142">属性</span><span class="sxs-lookup"><span data-stu-id="7b23a-142">Properties</span></span>

|<span data-ttu-id="7b23a-143">属性</span><span class="sxs-lookup"><span data-stu-id="7b23a-143">Property</span></span>|<span data-ttu-id="7b23a-144">类型</span><span class="sxs-lookup"><span data-stu-id="7b23a-144">Type</span></span>|<span data-ttu-id="7b23a-145">说明</span><span class="sxs-lookup"><span data-stu-id="7b23a-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b23a-146">id</span><span class="sxs-lookup"><span data-stu-id="7b23a-146">id</span></span>|<span data-ttu-id="7b23a-147">String</span><span class="sxs-lookup"><span data-stu-id="7b23a-147">String</span></span>|<span data-ttu-id="7b23a-148">虚拟终结点 ID 的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="7b23a-148">The unique identifier for the virtual endpoint id. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b23a-149">关系</span><span class="sxs-lookup"><span data-stu-id="7b23a-149">Relationships</span></span>

|<span data-ttu-id="7b23a-150">关系</span><span class="sxs-lookup"><span data-stu-id="7b23a-150">Relationship</span></span>|<span data-ttu-id="7b23a-151">类型</span><span class="sxs-lookup"><span data-stu-id="7b23a-151">Type</span></span>|<span data-ttu-id="7b23a-152">说明</span><span class="sxs-lookup"><span data-stu-id="7b23a-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b23a-153">cloudPCs</span><span class="sxs-lookup"><span data-stu-id="7b23a-153">cloudPCs</span></span>|<span data-ttu-id="7b23a-154">[cloudPC](../resources/cloudpc.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b23a-154">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="7b23a-155">云托管虚拟桌面。</span><span class="sxs-lookup"><span data-stu-id="7b23a-155">Cloud managed virtual desktops.</span></span>|
|<span data-ttu-id="7b23a-156">deviceImages</span><span class="sxs-lookup"><span data-stu-id="7b23a-156">deviceImages</span></span>|<span data-ttu-id="7b23a-157">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b23a-157">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="7b23a-158">云电脑上的图像资源。</span><span class="sxs-lookup"><span data-stu-id="7b23a-158">The image resource on cloud PC.</span></span>|
|<span data-ttu-id="7b23a-159">onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="7b23a-159">onPremisesConnections</span></span>|<span data-ttu-id="7b23a-160">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b23a-160">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="7b23a-161">一组已定义的 Azure 资源信息，可用于为云电脑建立本地网络连接。</span><span class="sxs-lookup"><span data-stu-id="7b23a-161">A defined collection of Azure resource information that can be used to establish on-premises network connectivity for cloud PCs.</span></span>|
|<span data-ttu-id="7b23a-162">provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="7b23a-162">provisioningPolicies</span></span>|<span data-ttu-id="7b23a-163">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b23a-163">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="7b23a-164">云电脑预配策略。</span><span class="sxs-lookup"><span data-stu-id="7b23a-164">Cloud PC provisioning policy.</span></span>|
|<span data-ttu-id="7b23a-165">userSettings</span><span class="sxs-lookup"><span data-stu-id="7b23a-165">userSettings</span></span>|<span data-ttu-id="7b23a-166">[cloudPcUserSetting](../resources/cloudpcusersetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b23a-166">[cloudPcUserSetting](../resources/cloudpcusersetting.md) collection</span></span>|<span data-ttu-id="7b23a-167">云电脑用户设置。</span><span class="sxs-lookup"><span data-stu-id="7b23a-167">Cloud PC user settings.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7b23a-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b23a-168">JSON representation</span></span>

<span data-ttu-id="7b23a-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b23a-169">The following is a JSON representation of the resource.</span></span>
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
