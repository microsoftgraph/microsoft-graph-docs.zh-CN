---
title: azureADDevice 资源类型
description: 表示 Azure AD Azure Active Directory (注册) Azure AD 服务中的设备。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a9d7b68257895674530acfbafcd0fb6b6c9c7b02
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067871"
---
# <a name="azureaddevice-resource-type"></a><span data-ttu-id="d559a-103">azureADDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="d559a-103">azureADDevice resource type</span></span>

<span data-ttu-id="d559a-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="d559a-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d559a-105">表示 Azure AD Azure Active Directory (注册) Azure AD 服务中的设备。</span><span class="sxs-lookup"><span data-stu-id="d559a-105">Represents a device in Azure Active Directory (Azure AD) that is registered with the deployment service.</span></span>

<span data-ttu-id="d559a-106">Azure AD 设备通过以下方法之一自动创建：</span><span class="sxs-lookup"><span data-stu-id="d559a-106">An Azure AD device is automatically created through one of the following methods:</span></span>
* [<span data-ttu-id="d559a-107">updatableAsset： enrollAssets</span><span class="sxs-lookup"><span data-stu-id="d559a-107">updatableAsset: enrollAssets</span></span>](../api/windowsupdates-updatableasset-enrollassets.md)
* [<span data-ttu-id="d559a-108">updatableAsset： enrollAssetsById</span><span class="sxs-lookup"><span data-stu-id="d559a-108">updatableAsset: enrollAssetsById</span></span>](../api/windowsupdates-updatableasset-enrollassetsbyid.md)
* [<span data-ttu-id="d559a-109">deploymentAudience：updateAudience</span><span class="sxs-lookup"><span data-stu-id="d559a-109">deploymentAudience: updateAudience</span></span>](../api/windowsupdates-deploymentaudience-updateaudience.md)
* [<span data-ttu-id="d559a-110">deploymentAudience：updateAudienceById</span><span class="sxs-lookup"><span data-stu-id="d559a-110">deploymentAudience: updateAudienceById</span></span>](../api/windowsupdates-deploymentaudience-updateaudiencebyid.md)
* [<span data-ttu-id="d559a-111">updatableAssetGroup：addMembers</span><span class="sxs-lookup"><span data-stu-id="d559a-111">updatableAssetGroup: addMembers</span></span>](../api/windowsupdates-updatableassetgroup-addmembers.md)
* [<span data-ttu-id="d559a-112">updatableAssetGroup：addMembersById</span><span class="sxs-lookup"><span data-stu-id="d559a-112">updatableAssetGroup: addMembersById</span></span>](../api/windowsupdates-updatableassetgroup-addmembersbyid.md)

<span data-ttu-id="d559a-113">继承自 [updatableAsset](../resources/windowsupdates-updatableasset.md)。</span><span class="sxs-lookup"><span data-stu-id="d559a-113">Inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d559a-114">方法</span><span class="sxs-lookup"><span data-stu-id="d559a-114">Methods</span></span>
|<span data-ttu-id="d559a-115">方法</span><span class="sxs-lookup"><span data-stu-id="d559a-115">Method</span></span>|<span data-ttu-id="d559a-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="d559a-116">Return type</span></span>|<span data-ttu-id="d559a-117">说明</span><span class="sxs-lookup"><span data-stu-id="d559a-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d559a-118">列出 azureADDevice 资源</span><span class="sxs-lookup"><span data-stu-id="d559a-118">List azureADDevice resources</span></span>](../api/windowsupdates-updates-list-updatableassets-azureaddevice.md)|<span data-ttu-id="d559a-119">[microsoft.graph.windowsUpdates.azureADDevice](../resources/windowsupdates-azureaddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d559a-119">[microsoft.graph.windowsUpdates.azureADDevice](../resources/windowsupdates-azureaddevice.md) collection</span></span>|<span data-ttu-id="d559a-120">获取 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="d559a-120">Get a list of the [azureADDevice](../resources/windowsupdates-azureaddevice.md) objects and their properties.</span></span>|
|[<span data-ttu-id="d559a-121">获取 azureADDevice</span><span class="sxs-lookup"><span data-stu-id="d559a-121">Get azureADDevice</span></span>](../api/windowsupdates-azureaddevice-get.md)|[<span data-ttu-id="d559a-122">microsoft.graph.windowsUpdates.azureADDevice</span><span class="sxs-lookup"><span data-stu-id="d559a-122">microsoft.graph.windowsUpdates.azureADDevice</span></span>](../resources/windowsupdates-azureaddevice.md)|<span data-ttu-id="d559a-123">读取 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d559a-123">Read the properties and relationships of an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object.</span></span>|
|[<span data-ttu-id="d559a-124">删除 azureADDevice</span><span class="sxs-lookup"><span data-stu-id="d559a-124">Delete azureADDevice</span></span>](../api/windowsupdates-azureaddevice-delete.md)|<span data-ttu-id="d559a-125">无</span><span class="sxs-lookup"><span data-stu-id="d559a-125">None</span></span>|<span data-ttu-id="d559a-126">删除 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d559a-126">Delete an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object.</span></span>|
|[<span data-ttu-id="d559a-127">在管理中注册 azureADDevice 资源</span><span class="sxs-lookup"><span data-stu-id="d559a-127">Enroll azureADDevice resources in management</span></span>](../api/windowsupdates-updatableasset-enrollassets.md)|<span data-ttu-id="d559a-128">无</span><span class="sxs-lookup"><span data-stu-id="d559a-128">None</span></span>|<span data-ttu-id="d559a-129">在 [部署服务更新管理中注册 azureADDevice](../resources/windowsupdates-azureaddevice.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="d559a-129">Enroll [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources in update management by the deployment service.</span></span>|
|[<span data-ttu-id="d559a-130">按 ID 管理中心注册 azureADDevice (azureADDevice) </span><span class="sxs-lookup"><span data-stu-id="d559a-130">Enroll azureADDevice resources in management (by ID)</span></span>](../api/windowsupdates-updatableasset-enrollassetsbyid.md)|<span data-ttu-id="d559a-131">无</span><span class="sxs-lookup"><span data-stu-id="d559a-131">None</span></span>|<span data-ttu-id="d559a-132">在 [部署服务更新管理中注册 azureADDevice](../resources/windowsupdates-azureaddevice.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="d559a-132">Enroll [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources in update management by the deployment service.</span></span>|
|[<span data-ttu-id="d559a-133">从管理中注销 azureADDevice 资源</span><span class="sxs-lookup"><span data-stu-id="d559a-133">Unenroll azureADDevice resources from management</span></span>](../api/windowsupdates-updatableasset-unenrollassets.md)|<span data-ttu-id="d559a-134">无</span><span class="sxs-lookup"><span data-stu-id="d559a-134">None</span></span>|<span data-ttu-id="d559a-135">从部署服务的更新管理中注销 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="d559a-135">Unenroll [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources from update management by the deployment service.</span></span>|
|[<span data-ttu-id="d559a-136">取消注册按 ID 管理 (azureADDevice) </span><span class="sxs-lookup"><span data-stu-id="d559a-136">Unenroll azureADDevice resources from management (by ID)</span></span>](../api/windowsupdates-updatableasset-unenrollassetsbyid.md)|<span data-ttu-id="d559a-137">无</span><span class="sxs-lookup"><span data-stu-id="d559a-137">None</span></span>|<span data-ttu-id="d559a-138">从部署服务的更新管理中注销 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="d559a-138">Unenroll [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources from update management by the deployment service.</span></span>|

## <a name="properties"></a><span data-ttu-id="d559a-139">属性</span><span class="sxs-lookup"><span data-stu-id="d559a-139">Properties</span></span>
|<span data-ttu-id="d559a-140">属性</span><span class="sxs-lookup"><span data-stu-id="d559a-140">Property</span></span>|<span data-ttu-id="d559a-141">类型</span><span class="sxs-lookup"><span data-stu-id="d559a-141">Type</span></span>|<span data-ttu-id="d559a-142">说明</span><span class="sxs-lookup"><span data-stu-id="d559a-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d559a-143">enrollments</span><span class="sxs-lookup"><span data-stu-id="d559a-143">enrollments</span></span>|<span data-ttu-id="d559a-144">[microsoft.graph.windowsUpdates.updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d559a-144">[microsoft.graph.windowsUpdates.updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md) collection</span></span>|<span data-ttu-id="d559a-145">指定设备注册的服务区域。</span><span class="sxs-lookup"><span data-stu-id="d559a-145">Specifies areas of the service in which the device is enrolled.</span></span> <span data-ttu-id="d559a-146">只读。</span><span class="sxs-lookup"><span data-stu-id="d559a-146">Read-only.</span></span> <span data-ttu-id="d559a-147">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="d559a-147">Returned by default.</span></span>|
|<span data-ttu-id="d559a-148">错误</span><span class="sxs-lookup"><span data-stu-id="d559a-148">errors</span></span>|<span data-ttu-id="d559a-149">[microsoft.graph.windowsUpdates.updatableAssetError](../resources/windowsupdates-updatableasseterror.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d559a-149">[microsoft.graph.windowsUpdates.updatableAssetError](../resources/windowsupdates-updatableasseterror.md) collection</span></span>|<span data-ttu-id="d559a-150">指定阻止设备注册更新管理或重新记录已部署内容的任何错误。</span><span class="sxs-lookup"><span data-stu-id="d559a-150">Specifies any errors that prevent the device from being enrolled in update management or receving deployed content.</span></span> <span data-ttu-id="d559a-151">只读。</span><span class="sxs-lookup"><span data-stu-id="d559a-151">Read-only.</span></span> <span data-ttu-id="d559a-152">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="d559a-152">Returned by default.</span></span>|
|<span data-ttu-id="d559a-153">id</span><span class="sxs-lookup"><span data-stu-id="d559a-153">id</span></span>|<span data-ttu-id="d559a-154">String</span><span class="sxs-lookup"><span data-stu-id="d559a-154">String</span></span>|<span data-ttu-id="d559a-155">设备的标识符。</span><span class="sxs-lookup"><span data-stu-id="d559a-155">An identifier for the device.</span></span> <span data-ttu-id="d559a-156">键。</span><span class="sxs-lookup"><span data-stu-id="d559a-156">Key.</span></span> <span data-ttu-id="d559a-157">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="d559a-157">Not nullable.</span></span> <span data-ttu-id="d559a-158">只读。</span><span class="sxs-lookup"><span data-stu-id="d559a-158">Read-only.</span></span> <span data-ttu-id="d559a-159">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="d559a-159">Returned by default.</span></span> <span data-ttu-id="d559a-160">继承自 [updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="d559a-160">Inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d559a-161">关系</span><span class="sxs-lookup"><span data-stu-id="d559a-161">Relationships</span></span>
<span data-ttu-id="d559a-162">无。</span><span class="sxs-lookup"><span data-stu-id="d559a-162">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d559a-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d559a-163">JSON representation</span></span>
<span data-ttu-id="d559a-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d559a-164">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.azureADDevice",
  "baseType": "microsoft.graph.windowsUpdates.updatableAsset",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
  "id": "String (identifier)",
  "errors": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
    }
  ],
  "enrollments": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
    }
  ]
}
```

