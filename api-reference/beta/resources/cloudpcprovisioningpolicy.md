---
title: cloudPcProvisioningPolicy 资源类型
description: 表示云电脑预配策略。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: b1f5a447c373e64b747fc77ec93c54d8adc09c60
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082074"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a><span data-ttu-id="1c801-103">cloudPcProvisioningPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c801-103">cloudPcProvisioningPolicy resource type</span></span>

<span data-ttu-id="1c801-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c801-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c801-105">表示云电脑预配策略。</span><span class="sxs-lookup"><span data-stu-id="1c801-105">Represents a cloud PC provisioning policy.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="1c801-106">方法</span><span class="sxs-lookup"><span data-stu-id="1c801-106">Methods</span></span>

|<span data-ttu-id="1c801-107">方法</span><span class="sxs-lookup"><span data-stu-id="1c801-107">Method</span></span>|<span data-ttu-id="1c801-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1c801-108">Return type</span></span>|<span data-ttu-id="1c801-109">说明</span><span class="sxs-lookup"><span data-stu-id="1c801-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1c801-110">列出 provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="1c801-110">List provisioningPolicies</span></span>](../api/virtualendpoint-list-provisioningpolicies.md)|<span data-ttu-id="1c801-111">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c801-111">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="1c801-112">列出 [cloudPcProvisioningPolicy 对象的属性和](../resources/cloudpcprovisioningpolicy.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="1c801-112">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>|
|[<span data-ttu-id="1c801-113">获取 cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="1c801-113">Get cloudPcProvisioningPolicy</span></span>](../api/cloudpcprovisioningpolicy-get.md)|[<span data-ttu-id="1c801-114">cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="1c801-114">cloudPcProvisioningPolicy</span></span>](../resources/cloudpcprovisioningpolicy.md)|<span data-ttu-id="1c801-115">读取 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1c801-115">Read the properties and relationships of a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>|
|[<span data-ttu-id="1c801-116">创建 cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="1c801-116">Create cloudPcProvisioningPolicy</span></span>](../api/virtualendpoint-post-provisioningpolicies.md)|[<span data-ttu-id="1c801-117">cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="1c801-117">cloudPcProvisioningPolicy</span></span>](../resources/cloudpcprovisioningpolicy.md)|<span data-ttu-id="1c801-118">创建新的 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1c801-118">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>|
|[<span data-ttu-id="1c801-119">更新 cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="1c801-119">Update cloudPcProvisioningPolicy</span></span>](../api/cloudpcprovisioningpolicy-update.md)|[<span data-ttu-id="1c801-120">cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="1c801-120">cloudPcProvisioningPolicy</span></span>](../resources/cloudpcprovisioningpolicy.md)|<span data-ttu-id="1c801-121">更新 [cloudPcProvisioningPolicy 对象](../resources/cloudpcprovisioningpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="1c801-121">Update the properties of a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>|
|[<span data-ttu-id="1c801-122">删除 cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="1c801-122">Delete cloudPcProvisioningPolicy</span></span>](../api/cloudpcprovisioningpolicy-delete.md)|<span data-ttu-id="1c801-123">无</span><span class="sxs-lookup"><span data-stu-id="1c801-123">None</span></span>|<span data-ttu-id="1c801-124">删除 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1c801-124">Delete a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>|
|[<span data-ttu-id="1c801-125">分配 cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="1c801-125">Assign cloudPcProvisioningPolicy</span></span>](../api/cloudpcprovisioningpolicy-assign.md)|<span data-ttu-id="1c801-126">无</span><span class="sxs-lookup"><span data-stu-id="1c801-126">None</span></span> |<span data-ttu-id="1c801-127">将 [cloudPcProvisioningPolicy 分配给](../resources/cloudpcprovisioningpolicy.md) 用户组。</span><span class="sxs-lookup"><span data-stu-id="1c801-127">Assign a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) to user groups.</span></span>|

## <a name="properties"></a><span data-ttu-id="1c801-128">属性</span><span class="sxs-lookup"><span data-stu-id="1c801-128">Properties</span></span>

|<span data-ttu-id="1c801-129">属性</span><span class="sxs-lookup"><span data-stu-id="1c801-129">Property</span></span>|<span data-ttu-id="1c801-130">类型</span><span class="sxs-lookup"><span data-stu-id="1c801-130">Type</span></span>|<span data-ttu-id="1c801-131">说明</span><span class="sxs-lookup"><span data-stu-id="1c801-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c801-132">id</span><span class="sxs-lookup"><span data-stu-id="1c801-132">id</span></span>|<span data-ttu-id="1c801-133">String</span><span class="sxs-lookup"><span data-stu-id="1c801-133">String</span></span>|<span data-ttu-id="1c801-134">云电脑预配策略的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1c801-134">Unique identifier for the cloud PC provisioning policy.</span></span> <span data-ttu-id="1c801-135">只读。</span><span class="sxs-lookup"><span data-stu-id="1c801-135">Read-only.</span></span>|
|<span data-ttu-id="1c801-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1c801-136">displayName</span></span>|<span data-ttu-id="1c801-137">String</span><span class="sxs-lookup"><span data-stu-id="1c801-137">String</span></span>|<span data-ttu-id="1c801-138">设置显示名称策略的项。</span><span class="sxs-lookup"><span data-stu-id="1c801-138">The display name for the provisioning policy.</span></span>|
|<span data-ttu-id="1c801-139">description</span><span class="sxs-lookup"><span data-stu-id="1c801-139">description</span></span>|<span data-ttu-id="1c801-140">String</span><span class="sxs-lookup"><span data-stu-id="1c801-140">String</span></span>|<span data-ttu-id="1c801-141">设置策略说明。</span><span class="sxs-lookup"><span data-stu-id="1c801-141">The provisioning policy description.</span></span>|
|<span data-ttu-id="1c801-142">onPremisesConnectionId</span><span class="sxs-lookup"><span data-stu-id="1c801-142">onPremisesConnectionId</span></span>|<span data-ttu-id="1c801-143">String</span><span class="sxs-lookup"><span data-stu-id="1c801-143">String</span></span>|<span data-ttu-id="1c801-144">cloudPcOnPremisesConnection 的 ID。</span><span class="sxs-lookup"><span data-stu-id="1c801-144">The ID of the cloudPcOnPremisesConnection.</span></span> <span data-ttu-id="1c801-145">若要确保云电脑具有网络连接并且它们已加入域，请选择与通过云电脑服务验证的虚拟网络的连接。</span><span class="sxs-lookup"><span data-stu-id="1c801-145">To ensure that cloud PCs have network connectivity and that they domain join, choose a connection with a virtual network that’s validated by the cloud PC service.</span></span>|
|<span data-ttu-id="1c801-146">imageId</span><span class="sxs-lookup"><span data-stu-id="1c801-146">imageId</span></span>|<span data-ttu-id="1c801-147">String</span><span class="sxs-lookup"><span data-stu-id="1c801-147">String</span></span>|<span data-ttu-id="1c801-148">你想要在云电脑中预配的操作系统映像的 ID。</span><span class="sxs-lookup"><span data-stu-id="1c801-148">The ID of the OS image you want to provision on cloud PCs.</span></span> <span data-ttu-id="1c801-149">库类型图像的格式为：{publisher_offer_sku}。</span><span class="sxs-lookup"><span data-stu-id="1c801-149">The format for a gallery type image is: {publisher_offer_sku}.</span></span>|
|<span data-ttu-id="1c801-150">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="1c801-150">imageDisplayName</span></span>|<span data-ttu-id="1c801-151">String</span><span class="sxs-lookup"><span data-stu-id="1c801-151">String</span></span>|<span data-ttu-id="1c801-152">要显示名称的操作系统映像的映像的映像。</span><span class="sxs-lookup"><span data-stu-id="1c801-152">The display name for the OS image you’re provisioning.</span></span>|
|<span data-ttu-id="1c801-153">imageType</span><span class="sxs-lookup"><span data-stu-id="1c801-153">imageType</span></span>|<span data-ttu-id="1c801-154">cloudPcProvisioningPolicyImageType</span><span class="sxs-lookup"><span data-stu-id="1c801-154">cloudPcProvisioningPolicyImageType</span></span>|<span data-ttu-id="1c801-155">你想要在云 (预配的操作系统映像) 库类型。</span><span class="sxs-lookup"><span data-stu-id="1c801-155">The type of OS image (custom or gallery) you want to provision on cloud PCs.</span></span> <span data-ttu-id="1c801-156">可取值为：`gallery`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="1c801-156">Possible values are: `gallery`, `custom`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c801-157">关系</span><span class="sxs-lookup"><span data-stu-id="1c801-157">Relationships</span></span>

|<span data-ttu-id="1c801-158">关系</span><span class="sxs-lookup"><span data-stu-id="1c801-158">Relationship</span></span>|<span data-ttu-id="1c801-159">类型</span><span class="sxs-lookup"><span data-stu-id="1c801-159">Type</span></span>|<span data-ttu-id="1c801-160">说明</span><span class="sxs-lookup"><span data-stu-id="1c801-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c801-161">assignments</span><span class="sxs-lookup"><span data-stu-id="1c801-161">assignments</span></span>|<span data-ttu-id="1c801-162">[cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c801-162">[cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) collection</span></span>|<span data-ttu-id="1c801-163">已定义的设置策略分配集合。</span><span class="sxs-lookup"><span data-stu-id="1c801-163">A defined collection of provisioning policy assignments.</span></span> <span data-ttu-id="1c801-164">表示已分配Microsoft 365 Azure AD 中的组和安全组集。</span><span class="sxs-lookup"><span data-stu-id="1c801-164">Represents the set of Microsoft 365 groups and security groups in Azure AD that have provisioning policy assigned.</span></span> <span data-ttu-id="1c801-165">仅在 `$expand` 上返回。</span><span class="sxs-lookup"><span data-stu-id="1c801-165">Returned only on `$expand`.</span></span> <span data-ttu-id="1c801-166">请参阅 [获取](../api/cloudpcprovisioningpolicy-get.md) 分配关系的示例。</span><span class="sxs-lookup"><span data-stu-id="1c801-166">See an [example](../api/cloudpcprovisioningpolicy-get.md) of getting the assignments relationship.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1c801-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c801-167">JSON representation</span></span>

<span data-ttu-id="1c801-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c801-168">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "onPremisesConnectionId": "String",
  "imageId": "String",
  "imageDisplayName": "String",
  "imageType": "String"
}
```
