---
title: detectedApp 资源类型
description: 托管设备上安装的托管或未托管应用。 未托管应用仅出现在标记为公司所有的设备上。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8b28965cb506075c8caf7d983ddf41eafcdda78d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881422"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="dbcb0-104">detectedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="dbcb0-104">detectedApp resource type</span></span>

> <span data-ttu-id="dbcb0-105">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dbcb0-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dbcb0-106">托管设备上安装的托管或未托管应用。</span><span class="sxs-lookup"><span data-stu-id="dbcb0-106">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="dbcb0-107">未托管应用仅出现在标记为公司所有的设备上。</span><span class="sxs-lookup"><span data-stu-id="dbcb0-107">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>
## <a name="methods"></a><span data-ttu-id="dbcb0-108">方法</span><span class="sxs-lookup"><span data-stu-id="dbcb0-108">Methods</span></span>
|<span data-ttu-id="dbcb0-109">方法</span><span class="sxs-lookup"><span data-stu-id="dbcb0-109">Method</span></span>|<span data-ttu-id="dbcb0-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="dbcb0-110">Return Type</span></span>|<span data-ttu-id="dbcb0-111">说明</span><span class="sxs-lookup"><span data-stu-id="dbcb0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dbcb0-112">List detectedApps</span><span class="sxs-lookup"><span data-stu-id="dbcb0-112">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="dbcb0-113">[detectedApp](../resources/intune-devices-detectedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dbcb0-113">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="dbcb0-114">列出 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dbcb0-114">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="dbcb0-115">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="dbcb0-115">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="dbcb0-116">detectedApp</span><span class="sxs-lookup"><span data-stu-id="dbcb0-116">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="dbcb0-117">读取 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dbcb0-117">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="dbcb0-118">Create detectedApp</span><span class="sxs-lookup"><span data-stu-id="dbcb0-118">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="dbcb0-119">detectedApp</span><span class="sxs-lookup"><span data-stu-id="dbcb0-119">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="dbcb0-120">创建新的 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dbcb0-120">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="dbcb0-121">Delete detectedApp</span><span class="sxs-lookup"><span data-stu-id="dbcb0-121">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="dbcb0-122">无</span><span class="sxs-lookup"><span data-stu-id="dbcb0-122">None</span></span>|<span data-ttu-id="dbcb0-123">删除 [detectedApp](../resources/intune-devices-detectedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="dbcb0-123">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="dbcb0-124">Update detectedApp</span><span class="sxs-lookup"><span data-stu-id="dbcb0-124">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="dbcb0-125">detectedApp</span><span class="sxs-lookup"><span data-stu-id="dbcb0-125">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="dbcb0-126">更新 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dbcb0-126">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dbcb0-127">属性</span><span class="sxs-lookup"><span data-stu-id="dbcb0-127">Properties</span></span>
|<span data-ttu-id="dbcb0-128">属性</span><span class="sxs-lookup"><span data-stu-id="dbcb0-128">Property</span></span>|<span data-ttu-id="dbcb0-129">类型</span><span class="sxs-lookup"><span data-stu-id="dbcb0-129">Type</span></span>|<span data-ttu-id="dbcb0-130">说明</span><span class="sxs-lookup"><span data-stu-id="dbcb0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbcb0-131">id</span><span class="sxs-lookup"><span data-stu-id="dbcb0-131">id</span></span>|<span data-ttu-id="dbcb0-132">String</span><span class="sxs-lookup"><span data-stu-id="dbcb0-132">String</span></span>|<span data-ttu-id="dbcb0-133">检测到的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="dbcb0-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="dbcb0-134">创建此应用程序时，Intune 将自动生成它。</span><span class="sxs-lookup"><span data-stu-id="dbcb0-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="dbcb0-135">只读。</span><span class="sxs-lookup"><span data-stu-id="dbcb0-135">Read-only.</span></span>|
|<span data-ttu-id="dbcb0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="dbcb0-136">displayName</span></span>|<span data-ttu-id="dbcb0-137">String</span><span class="sxs-lookup"><span data-stu-id="dbcb0-137">String</span></span>|<span data-ttu-id="dbcb0-138">发现的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="dbcb0-138">Name of the discovered application.</span></span> <span data-ttu-id="dbcb0-139">只读</span><span class="sxs-lookup"><span data-stu-id="dbcb0-139">Read-only</span></span>|
|<span data-ttu-id="dbcb0-140">version</span><span class="sxs-lookup"><span data-stu-id="dbcb0-140">version</span></span>|<span data-ttu-id="dbcb0-141">String</span><span class="sxs-lookup"><span data-stu-id="dbcb0-141">String</span></span>|<span data-ttu-id="dbcb0-142">发现的应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="dbcb0-142">Version of the discovered application.</span></span> <span data-ttu-id="dbcb0-143">只读</span><span class="sxs-lookup"><span data-stu-id="dbcb0-143">Read-only</span></span>|
|<span data-ttu-id="dbcb0-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="dbcb0-144">sizeInByte</span></span>|<span data-ttu-id="dbcb0-145">Int64</span><span class="sxs-lookup"><span data-stu-id="dbcb0-145">Int64</span></span>|<span data-ttu-id="dbcb0-146">发现的应用程序的大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="dbcb0-146">Discovered application size in bytes.</span></span> <span data-ttu-id="dbcb0-147">只读</span><span class="sxs-lookup"><span data-stu-id="dbcb0-147">Read-only</span></span>|
|<span data-ttu-id="dbcb0-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="dbcb0-148">deviceCount</span></span>|<span data-ttu-id="dbcb0-149">Int32</span><span class="sxs-lookup"><span data-stu-id="dbcb0-149">Int32</span></span>|<span data-ttu-id="dbcb0-150">已安装此应用程序的设备数量</span><span class="sxs-lookup"><span data-stu-id="dbcb0-150">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbcb0-151">关系</span><span class="sxs-lookup"><span data-stu-id="dbcb0-151">Relationships</span></span>
|<span data-ttu-id="dbcb0-152">关系</span><span class="sxs-lookup"><span data-stu-id="dbcb0-152">Relationship</span></span>|<span data-ttu-id="dbcb0-153">类型</span><span class="sxs-lookup"><span data-stu-id="dbcb0-153">Type</span></span>|<span data-ttu-id="dbcb0-154">说明</span><span class="sxs-lookup"><span data-stu-id="dbcb0-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbcb0-155">managedDevices</span><span class="sxs-lookup"><span data-stu-id="dbcb0-155">managedDevices</span></span>|<span data-ttu-id="dbcb0-156">[managedDevice](../resources/intune-devices-manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dbcb0-156">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="dbcb0-157">已安装发现的应用程序的设备</span><span class="sxs-lookup"><span data-stu-id="dbcb0-157">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dbcb0-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dbcb0-158">JSON Representation</span></span>
<span data-ttu-id="dbcb0-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dbcb0-159">Here is a JSON representation of the resource.</span></span>
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



