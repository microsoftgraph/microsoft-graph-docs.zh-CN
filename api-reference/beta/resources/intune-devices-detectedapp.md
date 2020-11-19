---
title: detectedApp 资源类型
description: 托管设备上安装的托管或未托管应用。 未托管应用仅出现在标记为公司所有的设备上。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bfd569086784964a7685ab6b5f174cefd906c2f7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267759"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="3e8d1-104">detectedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e8d1-104">detectedApp resource type</span></span>

<span data-ttu-id="3e8d1-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e8d1-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e8d1-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e8d1-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e8d1-108">托管设备上安装的托管或未托管应用。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-108">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="3e8d1-109">未托管应用仅出现在标记为公司所有的设备上。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-109">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="3e8d1-110">方法</span><span class="sxs-lookup"><span data-stu-id="3e8d1-110">Methods</span></span>
|<span data-ttu-id="3e8d1-111">方法</span><span class="sxs-lookup"><span data-stu-id="3e8d1-111">Method</span></span>|<span data-ttu-id="3e8d1-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="3e8d1-112">Return Type</span></span>|<span data-ttu-id="3e8d1-113">说明</span><span class="sxs-lookup"><span data-stu-id="3e8d1-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3e8d1-114">List detectedApps</span><span class="sxs-lookup"><span data-stu-id="3e8d1-114">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="3e8d1-115">[detectedApp](../resources/intune-devices-detectedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3e8d1-115">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="3e8d1-116">列出 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-116">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="3e8d1-117">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="3e8d1-117">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="3e8d1-118">detectedApp</span><span class="sxs-lookup"><span data-stu-id="3e8d1-118">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="3e8d1-119">读取 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-119">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="3e8d1-120">Create detectedApp</span><span class="sxs-lookup"><span data-stu-id="3e8d1-120">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="3e8d1-121">detectedApp</span><span class="sxs-lookup"><span data-stu-id="3e8d1-121">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="3e8d1-122">创建新的 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-122">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="3e8d1-123">Delete detectedApp</span><span class="sxs-lookup"><span data-stu-id="3e8d1-123">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="3e8d1-124">无</span><span class="sxs-lookup"><span data-stu-id="3e8d1-124">None</span></span>|<span data-ttu-id="3e8d1-125">删除 [detectedApp](../resources/intune-devices-detectedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-125">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="3e8d1-126">Update detectedApp</span><span class="sxs-lookup"><span data-stu-id="3e8d1-126">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="3e8d1-127">detectedApp</span><span class="sxs-lookup"><span data-stu-id="3e8d1-127">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="3e8d1-128">更新 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-128">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3e8d1-129">属性</span><span class="sxs-lookup"><span data-stu-id="3e8d1-129">Properties</span></span>
|<span data-ttu-id="3e8d1-130">属性</span><span class="sxs-lookup"><span data-stu-id="3e8d1-130">Property</span></span>|<span data-ttu-id="3e8d1-131">类型</span><span class="sxs-lookup"><span data-stu-id="3e8d1-131">Type</span></span>|<span data-ttu-id="3e8d1-132">说明</span><span class="sxs-lookup"><span data-stu-id="3e8d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e8d1-133">id</span><span class="sxs-lookup"><span data-stu-id="3e8d1-133">id</span></span>|<span data-ttu-id="3e8d1-134">字符串</span><span class="sxs-lookup"><span data-stu-id="3e8d1-134">String</span></span>|<span data-ttu-id="3e8d1-135">检测到的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="3e8d1-136">创建此应用程序时，Intune 将自动生成它。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="3e8d1-137">只读。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-137">Read-only.</span></span>|
|<span data-ttu-id="3e8d1-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3e8d1-138">displayName</span></span>|<span data-ttu-id="3e8d1-139">字符串</span><span class="sxs-lookup"><span data-stu-id="3e8d1-139">String</span></span>|<span data-ttu-id="3e8d1-140">发现的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-140">Name of the discovered application.</span></span> <span data-ttu-id="3e8d1-141">只读</span><span class="sxs-lookup"><span data-stu-id="3e8d1-141">Read-only</span></span>|
|<span data-ttu-id="3e8d1-142">version</span><span class="sxs-lookup"><span data-stu-id="3e8d1-142">version</span></span>|<span data-ttu-id="3e8d1-143">String</span><span class="sxs-lookup"><span data-stu-id="3e8d1-143">String</span></span>|<span data-ttu-id="3e8d1-144">发现的应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-144">Version of the discovered application.</span></span> <span data-ttu-id="3e8d1-145">只读</span><span class="sxs-lookup"><span data-stu-id="3e8d1-145">Read-only</span></span>|
|<span data-ttu-id="3e8d1-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="3e8d1-146">sizeInByte</span></span>|<span data-ttu-id="3e8d1-147">Int64</span><span class="sxs-lookup"><span data-stu-id="3e8d1-147">Int64</span></span>|<span data-ttu-id="3e8d1-148">发现的应用程序的大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-148">Discovered application size in bytes.</span></span> <span data-ttu-id="3e8d1-149">只读</span><span class="sxs-lookup"><span data-stu-id="3e8d1-149">Read-only</span></span>|
|<span data-ttu-id="3e8d1-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="3e8d1-150">deviceCount</span></span>|<span data-ttu-id="3e8d1-151">Int32</span><span class="sxs-lookup"><span data-stu-id="3e8d1-151">Int32</span></span>|<span data-ttu-id="3e8d1-152">已安装此应用程序的设备数量</span><span class="sxs-lookup"><span data-stu-id="3e8d1-152">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e8d1-153">关系</span><span class="sxs-lookup"><span data-stu-id="3e8d1-153">Relationships</span></span>
|<span data-ttu-id="3e8d1-154">关系</span><span class="sxs-lookup"><span data-stu-id="3e8d1-154">Relationship</span></span>|<span data-ttu-id="3e8d1-155">类型</span><span class="sxs-lookup"><span data-stu-id="3e8d1-155">Type</span></span>|<span data-ttu-id="3e8d1-156">说明</span><span class="sxs-lookup"><span data-stu-id="3e8d1-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e8d1-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="3e8d1-157">managedDevices</span></span>|<span data-ttu-id="3e8d1-158">[managedDevice](../resources/intune-devices-manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3e8d1-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="3e8d1-159">已安装发现的应用程序的设备</span><span class="sxs-lookup"><span data-stu-id="3e8d1-159">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e8d1-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e8d1-160">JSON Representation</span></span>
<span data-ttu-id="3e8d1-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e8d1-161">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```




