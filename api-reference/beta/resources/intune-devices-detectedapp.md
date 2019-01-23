---
title: detectedApp 资源类型
description: 托管设备上安装的托管或未托管应用。 未托管应用仅出现在标记为公司所有的设备上。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4cba801689cb5051926a3139574d5a27294090a0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403096"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="62b55-104">detectedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="62b55-104">detectedApp resource type</span></span>

> <span data-ttu-id="62b55-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="62b55-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="62b55-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="62b55-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62b55-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="62b55-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62b55-108">托管设备上安装的托管或未托管应用。</span><span class="sxs-lookup"><span data-stu-id="62b55-108">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="62b55-109">未托管应用仅出现在标记为公司所有的设备上。</span><span class="sxs-lookup"><span data-stu-id="62b55-109">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="62b55-110">方法</span><span class="sxs-lookup"><span data-stu-id="62b55-110">Methods</span></span>
|<span data-ttu-id="62b55-111">方法</span><span class="sxs-lookup"><span data-stu-id="62b55-111">Method</span></span>|<span data-ttu-id="62b55-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="62b55-112">Return Type</span></span>|<span data-ttu-id="62b55-113">说明</span><span class="sxs-lookup"><span data-stu-id="62b55-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="62b55-114">List detectedApps</span><span class="sxs-lookup"><span data-stu-id="62b55-114">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="62b55-115">[detectedApp](../resources/intune-devices-detectedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="62b55-115">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="62b55-116">列出 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="62b55-116">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="62b55-117">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="62b55-117">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="62b55-118">detectedApp</span><span class="sxs-lookup"><span data-stu-id="62b55-118">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="62b55-119">读取 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="62b55-119">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="62b55-120">Create detectedApp</span><span class="sxs-lookup"><span data-stu-id="62b55-120">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="62b55-121">detectedApp</span><span class="sxs-lookup"><span data-stu-id="62b55-121">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="62b55-122">创建新的 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="62b55-122">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="62b55-123">Delete detectedApp</span><span class="sxs-lookup"><span data-stu-id="62b55-123">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="62b55-124">无</span><span class="sxs-lookup"><span data-stu-id="62b55-124">None</span></span>|<span data-ttu-id="62b55-125">删除 [detectedApp](../resources/intune-devices-detectedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="62b55-125">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="62b55-126">Update detectedApp</span><span class="sxs-lookup"><span data-stu-id="62b55-126">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="62b55-127">detectedApp</span><span class="sxs-lookup"><span data-stu-id="62b55-127">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="62b55-128">更新 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="62b55-128">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="62b55-129">属性</span><span class="sxs-lookup"><span data-stu-id="62b55-129">Properties</span></span>
|<span data-ttu-id="62b55-130">属性</span><span class="sxs-lookup"><span data-stu-id="62b55-130">Property</span></span>|<span data-ttu-id="62b55-131">类型</span><span class="sxs-lookup"><span data-stu-id="62b55-131">Type</span></span>|<span data-ttu-id="62b55-132">说明</span><span class="sxs-lookup"><span data-stu-id="62b55-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62b55-133">id</span><span class="sxs-lookup"><span data-stu-id="62b55-133">id</span></span>|<span data-ttu-id="62b55-134">String</span><span class="sxs-lookup"><span data-stu-id="62b55-134">String</span></span>|<span data-ttu-id="62b55-135">检测到的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="62b55-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="62b55-136">创建此应用程序时，Intune 将自动生成它。</span><span class="sxs-lookup"><span data-stu-id="62b55-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="62b55-137">只读。</span><span class="sxs-lookup"><span data-stu-id="62b55-137">Read-only.</span></span>|
|<span data-ttu-id="62b55-138">displayName</span><span class="sxs-lookup"><span data-stu-id="62b55-138">displayName</span></span>|<span data-ttu-id="62b55-139">String</span><span class="sxs-lookup"><span data-stu-id="62b55-139">String</span></span>|<span data-ttu-id="62b55-140">发现的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="62b55-140">Name of the discovered application.</span></span> <span data-ttu-id="62b55-141">只读</span><span class="sxs-lookup"><span data-stu-id="62b55-141">Read-only</span></span>|
|<span data-ttu-id="62b55-142">version</span><span class="sxs-lookup"><span data-stu-id="62b55-142">version</span></span>|<span data-ttu-id="62b55-143">String</span><span class="sxs-lookup"><span data-stu-id="62b55-143">String</span></span>|<span data-ttu-id="62b55-144">发现的应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="62b55-144">Version of the discovered application.</span></span> <span data-ttu-id="62b55-145">只读</span><span class="sxs-lookup"><span data-stu-id="62b55-145">Read-only</span></span>|
|<span data-ttu-id="62b55-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="62b55-146">sizeInByte</span></span>|<span data-ttu-id="62b55-147">Int64</span><span class="sxs-lookup"><span data-stu-id="62b55-147">Int64</span></span>|<span data-ttu-id="62b55-148">发现的应用程序的大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="62b55-148">Discovered application size in bytes.</span></span> <span data-ttu-id="62b55-149">只读</span><span class="sxs-lookup"><span data-stu-id="62b55-149">Read-only</span></span>|
|<span data-ttu-id="62b55-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="62b55-150">deviceCount</span></span>|<span data-ttu-id="62b55-151">Int32</span><span class="sxs-lookup"><span data-stu-id="62b55-151">Int32</span></span>|<span data-ttu-id="62b55-152">已安装此应用程序的设备数量</span><span class="sxs-lookup"><span data-stu-id="62b55-152">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="62b55-153">关系</span><span class="sxs-lookup"><span data-stu-id="62b55-153">Relationships</span></span>
|<span data-ttu-id="62b55-154">关系</span><span class="sxs-lookup"><span data-stu-id="62b55-154">Relationship</span></span>|<span data-ttu-id="62b55-155">类型</span><span class="sxs-lookup"><span data-stu-id="62b55-155">Type</span></span>|<span data-ttu-id="62b55-156">说明</span><span class="sxs-lookup"><span data-stu-id="62b55-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62b55-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="62b55-157">managedDevices</span></span>|<span data-ttu-id="62b55-158">[managedDevice](../resources/intune-devices-manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="62b55-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="62b55-159">已安装发现的应用程序的设备</span><span class="sxs-lookup"><span data-stu-id="62b55-159">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62b55-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62b55-160">JSON Representation</span></span>
<span data-ttu-id="62b55-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62b55-161">Here is a JSON representation of the resource.</span></span>
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




