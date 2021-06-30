---
title: virtualEndpoint 资源类型
description: virtualEndpoint 资源表示云电脑管理功能的容器。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 215179905a9affc9d9c31770511ebbdf22d865ba
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208188"
---
# <a name="virtualendpoint-resource-type"></a><span data-ttu-id="e0889-103">virtualEndpoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0889-103">virtualEndpoint resource type</span></span>

<span data-ttu-id="e0889-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0889-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0889-105">表示 API 用于管理云电脑的容器。</span><span class="sxs-lookup"><span data-stu-id="e0889-105">Represents a container for APIs to manage cloud PC.</span></span>

<span data-ttu-id="e0889-106">使用云电脑 API 为组织的员工预配和管理虚拟桌面。</span><span class="sxs-lookup"><span data-stu-id="e0889-106">Use the cloud PC API to provision and manage virtual desktops for employees in an organization.</span></span> <span data-ttu-id="e0889-107">将它与 [Intune API](../resources/intune-graph-overview.md) 结合使用，以管理物理和虚拟终结点。</span><span class="sxs-lookup"><span data-stu-id="e0889-107">Use it in conjunction with the [Intune API](../resources/intune-graph-overview.md) to manage physical and virtual endpoints.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="methods"></a><span data-ttu-id="e0889-108">方法</span><span class="sxs-lookup"><span data-stu-id="e0889-108">Methods</span></span>

|<span data-ttu-id="e0889-109">方法</span><span class="sxs-lookup"><span data-stu-id="e0889-109">Method</span></span>|<span data-ttu-id="e0889-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e0889-110">Return type</span></span>|<span data-ttu-id="e0889-111">说明</span><span class="sxs-lookup"><span data-stu-id="e0889-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e0889-112">获取有效权限</span><span class="sxs-lookup"><span data-stu-id="e0889-112">Get effective permissions</span></span>](../api/virtualendpoint-geteffectivepermissions.md)|<span data-ttu-id="e0889-113">String collection</span><span class="sxs-lookup"><span data-stu-id="e0889-113">String collection</span></span>|<span data-ttu-id="e0889-114">查看当前经过身份验证的用户的有效权限。</span><span class="sxs-lookup"><span data-stu-id="e0889-114">View the effective permissions of the currently authenticated user.</span></span>|
|[<span data-ttu-id="e0889-115">列出 cloudPCs</span><span class="sxs-lookup"><span data-stu-id="e0889-115">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="e0889-116">[cloudPC](../resources/cloudpc.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0889-116">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="e0889-117">列出 [cloudPC 对象的属性和](../resources/cloudpc.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="e0889-117">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="e0889-118">列出 deviceImages</span><span class="sxs-lookup"><span data-stu-id="e0889-118">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="e0889-119">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0889-119">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="e0889-120">列出 [cloudPcDeviceImage 对象的属性和](../resources/cloudpcdeviceimage.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="e0889-120">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="e0889-121">创建 cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="e0889-121">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="e0889-122">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="e0889-122">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="e0889-123">创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0889-123">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="e0889-124">列出 onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="e0889-124">List onPremisesConnections</span></span>](../api/virtualendpoint-list-onpremisesconnections.md)|<span data-ttu-id="e0889-125">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0889-125">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="e0889-126">列出 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e0889-126">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>|
|[<span data-ttu-id="e0889-127">创建 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="e0889-127">Create cloudPcOnPremisesConnection</span></span>](../api/virtualendpoint-post-onpremisesconnections.md)|[<span data-ttu-id="e0889-128">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="e0889-128">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="e0889-129">创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0889-129">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="e0889-130">列出 provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="e0889-130">List provisioningPolicies</span></span>](../api/virtualendpoint-list-provisioningpolicies.md)|<span data-ttu-id="e0889-131">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0889-131">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="e0889-132">列出 [cloudPcProvisioningPolicy 对象的属性和](../resources/cloudpcprovisioningpolicy.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="e0889-132">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>|
|[<span data-ttu-id="e0889-133">创建 cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="e0889-133">Create cloudPcProvisioningPolicy</span></span>](../api/virtualendpoint-post-provisioningpolicies.md)|[<span data-ttu-id="e0889-134">cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="e0889-134">cloudPcProvisioningPolicy</span></span>](../resources/cloudpcprovisioningpolicy.md)|<span data-ttu-id="e0889-135">创建新的 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0889-135">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>|
|[<span data-ttu-id="e0889-136">列出 userSettings</span><span class="sxs-lookup"><span data-stu-id="e0889-136">List userSettings</span></span>](../api/virtualendpoint-list-usersettings.md)|<span data-ttu-id="e0889-137">[cloudPcUserSetting](../resources/cloudpcusersetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0889-137">[cloudPcUserSetting](../resources/cloudpcusersetting.md) collection</span></span>|<span data-ttu-id="e0889-138">从 userSettings 导航属性获取 cloudPcUserSetting 资源。</span><span class="sxs-lookup"><span data-stu-id="e0889-138">Get the cloudPcUserSetting resources from the userSettings navigation property.</span></span>|
|[<span data-ttu-id="e0889-139">创建 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="e0889-139">Create cloudPcUserSetting</span></span>](../api/virtualendpoint-post-usersettings.md)|[<span data-ttu-id="e0889-140">cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="e0889-140">cloudPcUserSetting</span></span>](../resources/cloudpcusersetting.md)|<span data-ttu-id="e0889-141">创建新的 cloudPcUserSetting 对象。</span><span class="sxs-lookup"><span data-stu-id="e0889-141">Create a new cloudPcUserSetting object.</span></span>|
|[<span data-ttu-id="e0889-142">列出 auditEvents</span><span class="sxs-lookup"><span data-stu-id="e0889-142">List auditEvents</span></span>](../api/virtualendpoint-list-auditevents.md)|<span data-ttu-id="e0889-143">[cloudPcAuditEvent](../resources/cloudpcauditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0889-143">[cloudPcAuditEvent](../resources/cloudpcauditevent.md) collection</span></span>|<span data-ttu-id="e0889-144">列出 [cloudPcAuditEvent 对象的属性和](../resources/cloudpcauditevent.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="e0889-144">List properties and relationships of the [cloudPcAuditEvent](../resources/cloudpcauditevent.md) objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="e0889-145">属性</span><span class="sxs-lookup"><span data-stu-id="e0889-145">Properties</span></span>

|<span data-ttu-id="e0889-146">属性</span><span class="sxs-lookup"><span data-stu-id="e0889-146">Property</span></span>|<span data-ttu-id="e0889-147">类型</span><span class="sxs-lookup"><span data-stu-id="e0889-147">Type</span></span>|<span data-ttu-id="e0889-148">说明</span><span class="sxs-lookup"><span data-stu-id="e0889-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0889-149">id</span><span class="sxs-lookup"><span data-stu-id="e0889-149">id</span></span>|<span data-ttu-id="e0889-150">String</span><span class="sxs-lookup"><span data-stu-id="e0889-150">String</span></span>|<span data-ttu-id="e0889-151">虚拟终结点 ID 的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="e0889-151">The unique identifier for the virtual endpoint id. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0889-152">关系</span><span class="sxs-lookup"><span data-stu-id="e0889-152">Relationships</span></span>

|<span data-ttu-id="e0889-153">关系</span><span class="sxs-lookup"><span data-stu-id="e0889-153">Relationship</span></span>|<span data-ttu-id="e0889-154">类型</span><span class="sxs-lookup"><span data-stu-id="e0889-154">Type</span></span>|<span data-ttu-id="e0889-155">说明</span><span class="sxs-lookup"><span data-stu-id="e0889-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0889-156">cloudPCs</span><span class="sxs-lookup"><span data-stu-id="e0889-156">cloudPCs</span></span>|<span data-ttu-id="e0889-157">[cloudPC](../resources/cloudpc.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0889-157">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="e0889-158">云托管虚拟桌面。</span><span class="sxs-lookup"><span data-stu-id="e0889-158">Cloud managed virtual desktops.</span></span>|
|<span data-ttu-id="e0889-159">deviceImages</span><span class="sxs-lookup"><span data-stu-id="e0889-159">deviceImages</span></span>|<span data-ttu-id="e0889-160">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0889-160">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="e0889-161">云电脑上的图像资源。</span><span class="sxs-lookup"><span data-stu-id="e0889-161">The image resource on cloud PC.</span></span>|
|<span data-ttu-id="e0889-162">onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="e0889-162">onPremisesConnections</span></span>|<span data-ttu-id="e0889-163">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0889-163">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="e0889-164">一组已定义的 Azure 资源信息，可用于为云电脑建立本地网络连接。</span><span class="sxs-lookup"><span data-stu-id="e0889-164">A defined collection of Azure resource information that can be used to establish on-premises network connectivity for cloud PCs.</span></span>|
|<span data-ttu-id="e0889-165">provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="e0889-165">provisioningPolicies</span></span>|<span data-ttu-id="e0889-166">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0889-166">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="e0889-167">云电脑预配策略。</span><span class="sxs-lookup"><span data-stu-id="e0889-167">Cloud PC provisioning policy.</span></span>|
|<span data-ttu-id="e0889-168">userSettings</span><span class="sxs-lookup"><span data-stu-id="e0889-168">userSettings</span></span>|<span data-ttu-id="e0889-169">[cloudPcUserSetting](../resources/cloudpcusersetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0889-169">[cloudPcUserSetting](../resources/cloudpcusersetting.md) collection</span></span>|<span data-ttu-id="e0889-170">云电脑用户设置。</span><span class="sxs-lookup"><span data-stu-id="e0889-170">Cloud PC user settings.</span></span> |
|<span data-ttu-id="e0889-171">auditEvents</span><span class="sxs-lookup"><span data-stu-id="e0889-171">auditEvents</span></span>|<span data-ttu-id="e0889-172">[cloudPcAuditEvent](../resources/cloudpcauditevent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0889-172">[cloudPcAuditEvent](../resources/cloudpcauditevent.md) collection</span></span>|<span data-ttu-id="e0889-173">云电脑审核事件。</span><span class="sxs-lookup"><span data-stu-id="e0889-173">Cloud PC audit event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e0889-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0889-174">JSON representation</span></span>

<span data-ttu-id="e0889-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0889-175">The following is a JSON representation of the resource.</span></span>
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
