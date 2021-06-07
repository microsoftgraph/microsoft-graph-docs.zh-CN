---
title: detectedApp 资源类型
description: 托管设备上安装的托管或未托管应用。 未托管应用仅出现在标记为公司所有的设备上。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a6e1d5f6ec6bab9b9506cf6ddcab625ff3d04b74
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758755"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="8faef-104">detectedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="8faef-104">detectedApp resource type</span></span>

<span data-ttu-id="8faef-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8faef-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8faef-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8faef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8faef-107">托管设备上安装的托管或未托管应用。</span><span class="sxs-lookup"><span data-stu-id="8faef-107">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="8faef-108">未托管应用仅出现在标记为公司所有的设备上。</span><span class="sxs-lookup"><span data-stu-id="8faef-108">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="8faef-109">方法</span><span class="sxs-lookup"><span data-stu-id="8faef-109">Methods</span></span>
|<span data-ttu-id="8faef-110">方法</span><span class="sxs-lookup"><span data-stu-id="8faef-110">Method</span></span>|<span data-ttu-id="8faef-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="8faef-111">Return Type</span></span>|<span data-ttu-id="8faef-112">说明</span><span class="sxs-lookup"><span data-stu-id="8faef-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8faef-113">List detectedApps</span><span class="sxs-lookup"><span data-stu-id="8faef-113">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="8faef-114">[detectedApp](../resources/intune-devices-detectedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8faef-114">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="8faef-115">列出 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8faef-115">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="8faef-116">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="8faef-116">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="8faef-117">detectedApp</span><span class="sxs-lookup"><span data-stu-id="8faef-117">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="8faef-118">读取 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8faef-118">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="8faef-119">Create detectedApp</span><span class="sxs-lookup"><span data-stu-id="8faef-119">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="8faef-120">detectedApp</span><span class="sxs-lookup"><span data-stu-id="8faef-120">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="8faef-121">创建新的 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8faef-121">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="8faef-122">Delete detectedApp</span><span class="sxs-lookup"><span data-stu-id="8faef-122">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="8faef-123">无</span><span class="sxs-lookup"><span data-stu-id="8faef-123">None</span></span>|<span data-ttu-id="8faef-124">删除 [detectedApp](../resources/intune-devices-detectedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="8faef-124">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="8faef-125">Update detectedApp</span><span class="sxs-lookup"><span data-stu-id="8faef-125">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="8faef-126">detectedApp</span><span class="sxs-lookup"><span data-stu-id="8faef-126">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="8faef-127">更新 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8faef-127">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8faef-128">属性</span><span class="sxs-lookup"><span data-stu-id="8faef-128">Properties</span></span>
|<span data-ttu-id="8faef-129">属性</span><span class="sxs-lookup"><span data-stu-id="8faef-129">Property</span></span>|<span data-ttu-id="8faef-130">类型</span><span class="sxs-lookup"><span data-stu-id="8faef-130">Type</span></span>|<span data-ttu-id="8faef-131">说明</span><span class="sxs-lookup"><span data-stu-id="8faef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8faef-132">id</span><span class="sxs-lookup"><span data-stu-id="8faef-132">id</span></span>|<span data-ttu-id="8faef-133">String</span><span class="sxs-lookup"><span data-stu-id="8faef-133">String</span></span>|<span data-ttu-id="8faef-134">检测到的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8faef-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="8faef-135">创建此应用程序时，Intune 将自动生成它。</span><span class="sxs-lookup"><span data-stu-id="8faef-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="8faef-136">只读。</span><span class="sxs-lookup"><span data-stu-id="8faef-136">Read-only.</span></span>|
|<span data-ttu-id="8faef-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8faef-137">displayName</span></span>|<span data-ttu-id="8faef-138">String</span><span class="sxs-lookup"><span data-stu-id="8faef-138">String</span></span>|<span data-ttu-id="8faef-139">发现的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="8faef-139">Name of the discovered application.</span></span> <span data-ttu-id="8faef-140">只读</span><span class="sxs-lookup"><span data-stu-id="8faef-140">Read-only</span></span>|
|<span data-ttu-id="8faef-141">version</span><span class="sxs-lookup"><span data-stu-id="8faef-141">version</span></span>|<span data-ttu-id="8faef-142">String</span><span class="sxs-lookup"><span data-stu-id="8faef-142">String</span></span>|<span data-ttu-id="8faef-143">发现的应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="8faef-143">Version of the discovered application.</span></span> <span data-ttu-id="8faef-144">只读</span><span class="sxs-lookup"><span data-stu-id="8faef-144">Read-only</span></span>|
|<span data-ttu-id="8faef-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="8faef-145">sizeInByte</span></span>|<span data-ttu-id="8faef-146">Int64</span><span class="sxs-lookup"><span data-stu-id="8faef-146">Int64</span></span>|<span data-ttu-id="8faef-147">发现的应用程序的大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="8faef-147">Discovered application size in bytes.</span></span> <span data-ttu-id="8faef-148">只读</span><span class="sxs-lookup"><span data-stu-id="8faef-148">Read-only</span></span>|
|<span data-ttu-id="8faef-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="8faef-149">deviceCount</span></span>|<span data-ttu-id="8faef-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8faef-150">Int32</span></span>|<span data-ttu-id="8faef-151">已安装此应用程序的设备数量</span><span class="sxs-lookup"><span data-stu-id="8faef-151">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="8faef-152">关系</span><span class="sxs-lookup"><span data-stu-id="8faef-152">Relationships</span></span>
|<span data-ttu-id="8faef-153">关系</span><span class="sxs-lookup"><span data-stu-id="8faef-153">Relationship</span></span>|<span data-ttu-id="8faef-154">类型</span><span class="sxs-lookup"><span data-stu-id="8faef-154">Type</span></span>|<span data-ttu-id="8faef-155">说明</span><span class="sxs-lookup"><span data-stu-id="8faef-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8faef-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="8faef-156">managedDevices</span></span>|<span data-ttu-id="8faef-157">[managedDevice](../resources/intune-devices-manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8faef-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="8faef-158">已安装发现的应用程序的设备</span><span class="sxs-lookup"><span data-stu-id="8faef-158">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8faef-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8faef-159">JSON Representation</span></span>
<span data-ttu-id="8faef-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8faef-160">Here is a JSON representation of the resource.</span></span>
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




