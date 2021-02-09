---
title: unmanagedDevice 资源类型
description: 在网络中发现非托管设备。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0163fb0f3704bee86622574428954b3c3c9f805a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160208"
---
# <a name="unmanageddevice-resource-type"></a><span data-ttu-id="4e8be-103">unmanagedDevice 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e8be-103">unmanagedDevice resource type</span></span>

<span data-ttu-id="4e8be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e8be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e8be-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4e8be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e8be-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e8be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e8be-107">在网络中发现非托管设备。</span><span class="sxs-lookup"><span data-stu-id="4e8be-107">Unmanaged device discovered in the network.</span></span>

## <a name="properties"></a><span data-ttu-id="4e8be-108">属性</span><span class="sxs-lookup"><span data-stu-id="4e8be-108">Properties</span></span>
|<span data-ttu-id="4e8be-109">属性</span><span class="sxs-lookup"><span data-stu-id="4e8be-109">Property</span></span>|<span data-ttu-id="4e8be-110">类型</span><span class="sxs-lookup"><span data-stu-id="4e8be-110">Type</span></span>|<span data-ttu-id="4e8be-111">说明</span><span class="sxs-lookup"><span data-stu-id="4e8be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e8be-112">os</span><span class="sxs-lookup"><span data-stu-id="4e8be-112">os</span></span>|<span data-ttu-id="4e8be-113">String</span><span class="sxs-lookup"><span data-stu-id="4e8be-113">String</span></span>|<span data-ttu-id="4e8be-114">操作系统。</span><span class="sxs-lookup"><span data-stu-id="4e8be-114">Operating system.</span></span>|
|<span data-ttu-id="4e8be-115">osVersion</span><span class="sxs-lookup"><span data-stu-id="4e8be-115">osVersion</span></span>|<span data-ttu-id="4e8be-116">String</span><span class="sxs-lookup"><span data-stu-id="4e8be-116">String</span></span>|<span data-ttu-id="4e8be-117">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="4e8be-117">Operating system version.</span></span>|
|<span data-ttu-id="4e8be-118">ipAddress</span><span class="sxs-lookup"><span data-stu-id="4e8be-118">ipAddress</span></span>|<span data-ttu-id="4e8be-119">String</span><span class="sxs-lookup"><span data-stu-id="4e8be-119">String</span></span>|<span data-ttu-id="4e8be-120">IP 地址。</span><span class="sxs-lookup"><span data-stu-id="4e8be-120">IP address.</span></span>|
|<span data-ttu-id="4e8be-121">deviceName</span><span class="sxs-lookup"><span data-stu-id="4e8be-121">deviceName</span></span>|<span data-ttu-id="4e8be-122">String</span><span class="sxs-lookup"><span data-stu-id="4e8be-122">String</span></span>|<span data-ttu-id="4e8be-123">设备名称。</span><span class="sxs-lookup"><span data-stu-id="4e8be-123">Device name.</span></span>|
|<span data-ttu-id="4e8be-124">macAddress</span><span class="sxs-lookup"><span data-stu-id="4e8be-124">macAddress</span></span>|<span data-ttu-id="4e8be-125">String</span><span class="sxs-lookup"><span data-stu-id="4e8be-125">String</span></span>|<span data-ttu-id="4e8be-126">MAC 地址。</span><span class="sxs-lookup"><span data-stu-id="4e8be-126">MAC address.</span></span>|
|<span data-ttu-id="4e8be-127">domain</span><span class="sxs-lookup"><span data-stu-id="4e8be-127">domain</span></span>|<span data-ttu-id="4e8be-128">String</span><span class="sxs-lookup"><span data-stu-id="4e8be-128">String</span></span>|<span data-ttu-id="4e8be-129">域。</span><span class="sxs-lookup"><span data-stu-id="4e8be-129">Domain.</span></span>|
|<span data-ttu-id="4e8be-130">manufacturer</span><span class="sxs-lookup"><span data-stu-id="4e8be-130">manufacturer</span></span>|<span data-ttu-id="4e8be-131">String</span><span class="sxs-lookup"><span data-stu-id="4e8be-131">String</span></span>|<span data-ttu-id="4e8be-132">制造商。</span><span class="sxs-lookup"><span data-stu-id="4e8be-132">Manufacturer.</span></span>|
|<span data-ttu-id="4e8be-133">model</span><span class="sxs-lookup"><span data-stu-id="4e8be-133">model</span></span>|<span data-ttu-id="4e8be-134">String</span><span class="sxs-lookup"><span data-stu-id="4e8be-134">String</span></span>|<span data-ttu-id="4e8be-135">模型。</span><span class="sxs-lookup"><span data-stu-id="4e8be-135">Model.</span></span>|
|<span data-ttu-id="4e8be-136">位置</span><span class="sxs-lookup"><span data-stu-id="4e8be-136">location</span></span>|<span data-ttu-id="4e8be-137">String</span><span class="sxs-lookup"><span data-stu-id="4e8be-137">String</span></span>|<span data-ttu-id="4e8be-138">位置。</span><span class="sxs-lookup"><span data-stu-id="4e8be-138">Location.</span></span>|
|<span data-ttu-id="4e8be-139">lastLoggedOnUser</span><span class="sxs-lookup"><span data-stu-id="4e8be-139">lastLoggedOnUser</span></span>|<span data-ttu-id="4e8be-140">String</span><span class="sxs-lookup"><span data-stu-id="4e8be-140">String</span></span>|<span data-ttu-id="4e8be-141">上次登录的用户。</span><span class="sxs-lookup"><span data-stu-id="4e8be-141">Last logged on user.</span></span>|
|<span data-ttu-id="4e8be-142">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="4e8be-142">lastSeenDateTime</span></span>|<span data-ttu-id="4e8be-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e8be-143">DateTimeOffset</span></span>|<span data-ttu-id="4e8be-144">上次看到的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4e8be-144">Last seen date and time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e8be-145">关系</span><span class="sxs-lookup"><span data-stu-id="4e8be-145">Relationships</span></span>
<span data-ttu-id="4e8be-146">无</span><span class="sxs-lookup"><span data-stu-id="4e8be-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e8be-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e8be-147">JSON Representation</span></span>
<span data-ttu-id="4e8be-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e8be-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unmanagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unmanagedDevice",
  "os": "String",
  "osVersion": "String",
  "ipAddress": "String",
  "deviceName": "String",
  "macAddress": "String",
  "domain": "String",
  "manufacturer": "String",
  "model": "String",
  "location": "String",
  "lastLoggedOnUser": "String",
  "lastSeenDateTime": "String (timestamp)"
}
```




