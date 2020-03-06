---
title: detectedApp 资源类型
description: 托管设备上安装的托管或未托管应用。 未托管应用仅出现在标记为公司所有的设备上。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dcf11e763ff826ddc0f3c20ff722b6f3d124af57
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530302"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="10042-104">detectedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="10042-104">detectedApp resource type</span></span>

<span data-ttu-id="10042-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10042-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10042-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10042-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10042-107">托管设备上安装的托管或未托管应用。</span><span class="sxs-lookup"><span data-stu-id="10042-107">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="10042-108">未托管应用仅出现在标记为公司所有的设备上。</span><span class="sxs-lookup"><span data-stu-id="10042-108">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="10042-109">Methods</span><span class="sxs-lookup"><span data-stu-id="10042-109">Methods</span></span>
|<span data-ttu-id="10042-110">方法</span><span class="sxs-lookup"><span data-stu-id="10042-110">Method</span></span>|<span data-ttu-id="10042-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="10042-111">Return Type</span></span>|<span data-ttu-id="10042-112">说明</span><span class="sxs-lookup"><span data-stu-id="10042-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="10042-113">List detectedApps</span><span class="sxs-lookup"><span data-stu-id="10042-113">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="10042-114">[detectedApp](../resources/intune-devices-detectedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="10042-114">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="10042-115">列出 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10042-115">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="10042-116">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="10042-116">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="10042-117">detectedApp</span><span class="sxs-lookup"><span data-stu-id="10042-117">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="10042-118">读取 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10042-118">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="10042-119">Create detectedApp</span><span class="sxs-lookup"><span data-stu-id="10042-119">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="10042-120">detectedApp</span><span class="sxs-lookup"><span data-stu-id="10042-120">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="10042-121">创建新的 [detectedApp](../resources/intune-devices-detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="10042-121">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="10042-122">Delete detectedApp</span><span class="sxs-lookup"><span data-stu-id="10042-122">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="10042-123">无</span><span class="sxs-lookup"><span data-stu-id="10042-123">None</span></span>|<span data-ttu-id="10042-124">删除 [detectedApp](../resources/intune-devices-detectedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="10042-124">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="10042-125">Update detectedApp</span><span class="sxs-lookup"><span data-stu-id="10042-125">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="10042-126">detectedApp</span><span class="sxs-lookup"><span data-stu-id="10042-126">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="10042-127">更新 [detectedApp](../resources/intune-devices-detectedapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="10042-127">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="10042-128">属性</span><span class="sxs-lookup"><span data-stu-id="10042-128">Properties</span></span>
|<span data-ttu-id="10042-129">属性</span><span class="sxs-lookup"><span data-stu-id="10042-129">Property</span></span>|<span data-ttu-id="10042-130">类型</span><span class="sxs-lookup"><span data-stu-id="10042-130">Type</span></span>|<span data-ttu-id="10042-131">说明</span><span class="sxs-lookup"><span data-stu-id="10042-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10042-132">id</span><span class="sxs-lookup"><span data-stu-id="10042-132">id</span></span>|<span data-ttu-id="10042-133">字符串</span><span class="sxs-lookup"><span data-stu-id="10042-133">String</span></span>|<span data-ttu-id="10042-134">检测到的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="10042-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="10042-135">创建此应用程序时，Intune 将自动生成它。</span><span class="sxs-lookup"><span data-stu-id="10042-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="10042-136">只读。</span><span class="sxs-lookup"><span data-stu-id="10042-136">Read-only.</span></span>|
|<span data-ttu-id="10042-137">displayName</span><span class="sxs-lookup"><span data-stu-id="10042-137">displayName</span></span>|<span data-ttu-id="10042-138">字符串</span><span class="sxs-lookup"><span data-stu-id="10042-138">String</span></span>|<span data-ttu-id="10042-139">发现的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="10042-139">Name of the discovered application.</span></span> <span data-ttu-id="10042-140">只读</span><span class="sxs-lookup"><span data-stu-id="10042-140">Read-only</span></span>|
|<span data-ttu-id="10042-141">version</span><span class="sxs-lookup"><span data-stu-id="10042-141">version</span></span>|<span data-ttu-id="10042-142">String</span><span class="sxs-lookup"><span data-stu-id="10042-142">String</span></span>|<span data-ttu-id="10042-143">发现的应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="10042-143">Version of the discovered application.</span></span> <span data-ttu-id="10042-144">只读</span><span class="sxs-lookup"><span data-stu-id="10042-144">Read-only</span></span>|
|<span data-ttu-id="10042-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="10042-145">sizeInByte</span></span>|<span data-ttu-id="10042-146">Int64</span><span class="sxs-lookup"><span data-stu-id="10042-146">Int64</span></span>|<span data-ttu-id="10042-147">发现的应用程序的大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="10042-147">Discovered application size in bytes.</span></span> <span data-ttu-id="10042-148">只读</span><span class="sxs-lookup"><span data-stu-id="10042-148">Read-only</span></span>|
|<span data-ttu-id="10042-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="10042-149">deviceCount</span></span>|<span data-ttu-id="10042-150">Int32</span><span class="sxs-lookup"><span data-stu-id="10042-150">Int32</span></span>|<span data-ttu-id="10042-151">已安装此应用程序的设备数量</span><span class="sxs-lookup"><span data-stu-id="10042-151">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="10042-152">关系</span><span class="sxs-lookup"><span data-stu-id="10042-152">Relationships</span></span>
|<span data-ttu-id="10042-153">关系</span><span class="sxs-lookup"><span data-stu-id="10042-153">Relationship</span></span>|<span data-ttu-id="10042-154">类型</span><span class="sxs-lookup"><span data-stu-id="10042-154">Type</span></span>|<span data-ttu-id="10042-155">说明</span><span class="sxs-lookup"><span data-stu-id="10042-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10042-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="10042-156">managedDevices</span></span>|<span data-ttu-id="10042-157">[managedDevice](../resources/intune-devices-manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="10042-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="10042-158">已安装发现的应用程序的设备</span><span class="sxs-lookup"><span data-stu-id="10042-158">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10042-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10042-159">JSON Representation</span></span>
<span data-ttu-id="10042-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10042-160">Here is a JSON representation of the resource.</span></span>
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




