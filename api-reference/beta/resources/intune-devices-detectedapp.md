---
title: detectedApp 资源类型
description: 托管设备上安装的托管或未托管应用。 未托管应用仅出现在标记为公司所有的设备上。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ddc854a825241b2a7b87d18faaaa7e8399c2fb1c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968888"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="d3d9a-104">detectedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3d9a-104">detectedApp resource type</span></span>

> <span data-ttu-id="d3d9a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3d9a-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3d9a-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3d9a-108">托管设备上安装的托管或未托管应用。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-108">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="d3d9a-109">未托管应用仅出现在标记为公司所有的设备上。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-109">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>
## <a name="methods"></a><span data-ttu-id="d3d9a-110">方法</span><span class="sxs-lookup"><span data-stu-id="d3d9a-110">Methods</span></span>
|<span data-ttu-id="d3d9a-111">方法</span><span class="sxs-lookup"><span data-stu-id="d3d9a-111">Method</span></span>|<span data-ttu-id="d3d9a-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="d3d9a-112">Return Type</span></span>|<span data-ttu-id="d3d9a-113">说明</span><span class="sxs-lookup"><span data-stu-id="d3d9a-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d3d9a-114">List detectedApps</span><span class="sxs-lookup"><span data-stu-id="d3d9a-114">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="d3d9a-115">[detectedApp](../resources/intune-devices-detectedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3d9a-115">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="d3d9a-116">列出 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-116">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="d3d9a-117">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="d3d9a-117">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="d3d9a-118">detectedApp</span><span class="sxs-lookup"><span data-stu-id="d3d9a-118">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="d3d9a-119">读取 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-119">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="d3d9a-120">Create detectedApp</span><span class="sxs-lookup"><span data-stu-id="d3d9a-120">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="d3d9a-121">detectedApp</span><span class="sxs-lookup"><span data-stu-id="d3d9a-121">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="d3d9a-122">创建新的 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-122">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="d3d9a-123">Delete detectedApp</span><span class="sxs-lookup"><span data-stu-id="d3d9a-123">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="d3d9a-124">无</span><span class="sxs-lookup"><span data-stu-id="d3d9a-124">None</span></span>|<span data-ttu-id="d3d9a-125">删除 [detectedApp](../resources/intune-devices-detectedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-125">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="d3d9a-126">Update detectedApp</span><span class="sxs-lookup"><span data-stu-id="d3d9a-126">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="d3d9a-127">detectedApp</span><span class="sxs-lookup"><span data-stu-id="d3d9a-127">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="d3d9a-128">更新 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-128">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d3d9a-129">属性</span><span class="sxs-lookup"><span data-stu-id="d3d9a-129">Properties</span></span>
|<span data-ttu-id="d3d9a-130">属性</span><span class="sxs-lookup"><span data-stu-id="d3d9a-130">Property</span></span>|<span data-ttu-id="d3d9a-131">类型</span><span class="sxs-lookup"><span data-stu-id="d3d9a-131">Type</span></span>|<span data-ttu-id="d3d9a-132">说明</span><span class="sxs-lookup"><span data-stu-id="d3d9a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3d9a-133">id</span><span class="sxs-lookup"><span data-stu-id="d3d9a-133">id</span></span>|<span data-ttu-id="d3d9a-134">String</span><span class="sxs-lookup"><span data-stu-id="d3d9a-134">String</span></span>|<span data-ttu-id="d3d9a-135">检测到的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="d3d9a-136">创建此应用程序时，Intune 将自动生成它。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="d3d9a-137">只读。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-137">Read-only.</span></span>|
|<span data-ttu-id="d3d9a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d3d9a-138">displayName</span></span>|<span data-ttu-id="d3d9a-139">String</span><span class="sxs-lookup"><span data-stu-id="d3d9a-139">String</span></span>|<span data-ttu-id="d3d9a-140">发现的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-140">Name of the discovered application.</span></span> <span data-ttu-id="d3d9a-141">只读</span><span class="sxs-lookup"><span data-stu-id="d3d9a-141">Read-only</span></span>|
|<span data-ttu-id="d3d9a-142">version</span><span class="sxs-lookup"><span data-stu-id="d3d9a-142">version</span></span>|<span data-ttu-id="d3d9a-143">String</span><span class="sxs-lookup"><span data-stu-id="d3d9a-143">String</span></span>|<span data-ttu-id="d3d9a-144">发现的应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-144">Version of the discovered application.</span></span> <span data-ttu-id="d3d9a-145">只读</span><span class="sxs-lookup"><span data-stu-id="d3d9a-145">Read-only</span></span>|
|<span data-ttu-id="d3d9a-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="d3d9a-146">sizeInByte</span></span>|<span data-ttu-id="d3d9a-147">Int64</span><span class="sxs-lookup"><span data-stu-id="d3d9a-147">Int64</span></span>|<span data-ttu-id="d3d9a-148">发现的应用程序的大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-148">Discovered application size in bytes.</span></span> <span data-ttu-id="d3d9a-149">只读</span><span class="sxs-lookup"><span data-stu-id="d3d9a-149">Read-only</span></span>|
|<span data-ttu-id="d3d9a-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="d3d9a-150">deviceCount</span></span>|<span data-ttu-id="d3d9a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d3d9a-151">Int32</span></span>|<span data-ttu-id="d3d9a-152">已安装此应用程序的设备数量</span><span class="sxs-lookup"><span data-stu-id="d3d9a-152">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3d9a-153">关系</span><span class="sxs-lookup"><span data-stu-id="d3d9a-153">Relationships</span></span>
|<span data-ttu-id="d3d9a-154">关系</span><span class="sxs-lookup"><span data-stu-id="d3d9a-154">Relationship</span></span>|<span data-ttu-id="d3d9a-155">类型</span><span class="sxs-lookup"><span data-stu-id="d3d9a-155">Type</span></span>|<span data-ttu-id="d3d9a-156">说明</span><span class="sxs-lookup"><span data-stu-id="d3d9a-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3d9a-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="d3d9a-157">managedDevices</span></span>|<span data-ttu-id="d3d9a-158">[managedDevice](../resources/intune-devices-manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3d9a-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="d3d9a-159">已安装发现的应用程序的设备</span><span class="sxs-lookup"><span data-stu-id="d3d9a-159">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3d9a-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3d9a-160">JSON Representation</span></span>
<span data-ttu-id="d3d9a-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3d9a-161">Here is a JSON representation of the resource.</span></span>
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





