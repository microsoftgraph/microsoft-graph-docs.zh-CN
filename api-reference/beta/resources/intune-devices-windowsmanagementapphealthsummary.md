---
title: windowsManagementAppHealthSummary 资源类型
description: 包含 Windows management 应用的运行状况摘要的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f62f5967702143149176cecd2513478256ead6d3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172056"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="9ccef-103">windowsManagementAppHealthSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ccef-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="9ccef-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9ccef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ccef-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ccef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ccef-106">包含 Windows management 应用的运行状况摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="9ccef-106">Contains properties for the health summary of the Windows management app.</span></span>

## <a name="methods"></a><span data-ttu-id="9ccef-107">方法</span><span class="sxs-lookup"><span data-stu-id="9ccef-107">Methods</span></span>
|<span data-ttu-id="9ccef-108">方法</span><span class="sxs-lookup"><span data-stu-id="9ccef-108">Method</span></span>|<span data-ttu-id="9ccef-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9ccef-109">Return Type</span></span>|<span data-ttu-id="9ccef-110">说明</span><span class="sxs-lookup"><span data-stu-id="9ccef-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ccef-111">获取 windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="9ccef-111">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="9ccef-112">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="9ccef-112">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="9ccef-113">读取[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9ccef-113">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="9ccef-114">更新 windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="9ccef-114">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="9ccef-115">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="9ccef-115">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="9ccef-116">更新[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9ccef-116">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ccef-117">属性</span><span class="sxs-lookup"><span data-stu-id="9ccef-117">Properties</span></span>
|<span data-ttu-id="9ccef-118">属性</span><span class="sxs-lookup"><span data-stu-id="9ccef-118">Property</span></span>|<span data-ttu-id="9ccef-119">类型</span><span class="sxs-lookup"><span data-stu-id="9ccef-119">Type</span></span>|<span data-ttu-id="9ccef-120">说明</span><span class="sxs-lookup"><span data-stu-id="9ccef-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ccef-121">id</span><span class="sxs-lookup"><span data-stu-id="9ccef-121">id</span></span>|<span data-ttu-id="9ccef-122">String</span><span class="sxs-lookup"><span data-stu-id="9ccef-122">String</span></span>|<span data-ttu-id="9ccef-123">Windows management 应用运行状况摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="9ccef-123">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="9ccef-124">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9ccef-124">healthyDeviceCount</span></span>|<span data-ttu-id="9ccef-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9ccef-125">Int32</span></span>|<span data-ttu-id="9ccef-126">正常的设备计数。</span><span class="sxs-lookup"><span data-stu-id="9ccef-126">Healthy device count.</span></span>|
|<span data-ttu-id="9ccef-127">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9ccef-127">unhealthyDeviceCount</span></span>|<span data-ttu-id="9ccef-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9ccef-128">Int32</span></span>|<span data-ttu-id="9ccef-129">设备计数不正常。</span><span class="sxs-lookup"><span data-stu-id="9ccef-129">Unhealthy device count.</span></span>|
|<span data-ttu-id="9ccef-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9ccef-130">unknownDeviceCount</span></span>|<span data-ttu-id="9ccef-131">Int32</span><span class="sxs-lookup"><span data-stu-id="9ccef-131">Int32</span></span>|<span data-ttu-id="9ccef-132">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="9ccef-132">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ccef-133">关系</span><span class="sxs-lookup"><span data-stu-id="9ccef-133">Relationships</span></span>
<span data-ttu-id="9ccef-134">无</span><span class="sxs-lookup"><span data-stu-id="9ccef-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ccef-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ccef-135">JSON Representation</span></span>
<span data-ttu-id="9ccef-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ccef-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "String (identifier)",
  "healthyDeviceCount": 1024,
  "unhealthyDeviceCount": 1024,
  "unknownDeviceCount": 1024
}
```




