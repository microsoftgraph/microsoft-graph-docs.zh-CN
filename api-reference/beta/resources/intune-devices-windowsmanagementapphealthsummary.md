---
title: windowsManagementAppHealthSummary 资源类型
description: 包含 Windows management 应用的运行状况摘要的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d54eb789b33a27f7e7c7a62e3a3e37aafff990ce
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999358"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="35d2f-103">windowsManagementAppHealthSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="35d2f-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="35d2f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35d2f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35d2f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35d2f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35d2f-106">包含 Windows management 应用的运行状况摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="35d2f-106">Contains properties for the health summary of the Windows management app.</span></span>

## <a name="methods"></a><span data-ttu-id="35d2f-107">方法</span><span class="sxs-lookup"><span data-stu-id="35d2f-107">Methods</span></span>
|<span data-ttu-id="35d2f-108">方法</span><span class="sxs-lookup"><span data-stu-id="35d2f-108">Method</span></span>|<span data-ttu-id="35d2f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="35d2f-109">Return Type</span></span>|<span data-ttu-id="35d2f-110">说明</span><span class="sxs-lookup"><span data-stu-id="35d2f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="35d2f-111">获取 windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="35d2f-111">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="35d2f-112">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="35d2f-112">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="35d2f-113">读取[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="35d2f-113">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="35d2f-114">更新 windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="35d2f-114">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="35d2f-115">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="35d2f-115">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="35d2f-116">更新[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="35d2f-116">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="35d2f-117">属性</span><span class="sxs-lookup"><span data-stu-id="35d2f-117">Properties</span></span>
|<span data-ttu-id="35d2f-118">属性</span><span class="sxs-lookup"><span data-stu-id="35d2f-118">Property</span></span>|<span data-ttu-id="35d2f-119">类型</span><span class="sxs-lookup"><span data-stu-id="35d2f-119">Type</span></span>|<span data-ttu-id="35d2f-120">说明</span><span class="sxs-lookup"><span data-stu-id="35d2f-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35d2f-121">id</span><span class="sxs-lookup"><span data-stu-id="35d2f-121">id</span></span>|<span data-ttu-id="35d2f-122">String</span><span class="sxs-lookup"><span data-stu-id="35d2f-122">String</span></span>|<span data-ttu-id="35d2f-123">Windows management 应用运行状况摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="35d2f-123">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="35d2f-124">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="35d2f-124">healthyDeviceCount</span></span>|<span data-ttu-id="35d2f-125">Int32</span><span class="sxs-lookup"><span data-stu-id="35d2f-125">Int32</span></span>|<span data-ttu-id="35d2f-126">正常的设备计数。</span><span class="sxs-lookup"><span data-stu-id="35d2f-126">Healthy device count.</span></span>|
|<span data-ttu-id="35d2f-127">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="35d2f-127">unhealthyDeviceCount</span></span>|<span data-ttu-id="35d2f-128">Int32</span><span class="sxs-lookup"><span data-stu-id="35d2f-128">Int32</span></span>|<span data-ttu-id="35d2f-129">设备计数不正常。</span><span class="sxs-lookup"><span data-stu-id="35d2f-129">Unhealthy device count.</span></span>|
|<span data-ttu-id="35d2f-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="35d2f-130">unknownDeviceCount</span></span>|<span data-ttu-id="35d2f-131">Int32</span><span class="sxs-lookup"><span data-stu-id="35d2f-131">Int32</span></span>|<span data-ttu-id="35d2f-132">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="35d2f-132">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35d2f-133">关系</span><span class="sxs-lookup"><span data-stu-id="35d2f-133">Relationships</span></span>
<span data-ttu-id="35d2f-134">无</span><span class="sxs-lookup"><span data-stu-id="35d2f-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35d2f-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35d2f-135">JSON Representation</span></span>
<span data-ttu-id="35d2f-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35d2f-136">Here is a JSON representation of the resource.</span></span>
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





