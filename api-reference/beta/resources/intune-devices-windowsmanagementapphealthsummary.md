---
title: windowsManagementAppHealthSummary 资源类型
description: 包含 Windows management 应用的运行状况摘要的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8033f5e66928de4e0f913eaaab0aaa271fa2894
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983979"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="9fe1a-103">windowsManagementAppHealthSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="9fe1a-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="9fe1a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9fe1a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fe1a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9fe1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fe1a-106">包含 Windows management 应用的运行状况摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="9fe1a-106">Contains properties for the health summary of the Windows management app.</span></span>

## <a name="methods"></a><span data-ttu-id="9fe1a-107">方法</span><span class="sxs-lookup"><span data-stu-id="9fe1a-107">Methods</span></span>
|<span data-ttu-id="9fe1a-108">方法</span><span class="sxs-lookup"><span data-stu-id="9fe1a-108">Method</span></span>|<span data-ttu-id="9fe1a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9fe1a-109">Return Type</span></span>|<span data-ttu-id="9fe1a-110">说明</span><span class="sxs-lookup"><span data-stu-id="9fe1a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9fe1a-111">获取 windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="9fe1a-111">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="9fe1a-112">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="9fe1a-112">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="9fe1a-113">读取[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9fe1a-113">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="9fe1a-114">更新 windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="9fe1a-114">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="9fe1a-115">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="9fe1a-115">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="9fe1a-116">更新[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9fe1a-116">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9fe1a-117">属性</span><span class="sxs-lookup"><span data-stu-id="9fe1a-117">Properties</span></span>
|<span data-ttu-id="9fe1a-118">属性</span><span class="sxs-lookup"><span data-stu-id="9fe1a-118">Property</span></span>|<span data-ttu-id="9fe1a-119">类型</span><span class="sxs-lookup"><span data-stu-id="9fe1a-119">Type</span></span>|<span data-ttu-id="9fe1a-120">说明</span><span class="sxs-lookup"><span data-stu-id="9fe1a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fe1a-121">id</span><span class="sxs-lookup"><span data-stu-id="9fe1a-121">id</span></span>|<span data-ttu-id="9fe1a-122">String</span><span class="sxs-lookup"><span data-stu-id="9fe1a-122">String</span></span>|<span data-ttu-id="9fe1a-123">Windows management 应用运行状况摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="9fe1a-123">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="9fe1a-124">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9fe1a-124">healthyDeviceCount</span></span>|<span data-ttu-id="9fe1a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="9fe1a-125">Int32</span></span>|<span data-ttu-id="9fe1a-126">正常的设备计数。</span><span class="sxs-lookup"><span data-stu-id="9fe1a-126">Healthy device count.</span></span>|
|<span data-ttu-id="9fe1a-127">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9fe1a-127">unhealthyDeviceCount</span></span>|<span data-ttu-id="9fe1a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9fe1a-128">Int32</span></span>|<span data-ttu-id="9fe1a-129">设备计数不正常。</span><span class="sxs-lookup"><span data-stu-id="9fe1a-129">Unhealthy device count.</span></span>|
|<span data-ttu-id="9fe1a-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9fe1a-130">unknownDeviceCount</span></span>|<span data-ttu-id="9fe1a-131">Int32</span><span class="sxs-lookup"><span data-stu-id="9fe1a-131">Int32</span></span>|<span data-ttu-id="9fe1a-132">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="9fe1a-132">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fe1a-133">关系</span><span class="sxs-lookup"><span data-stu-id="9fe1a-133">Relationships</span></span>
<span data-ttu-id="9fe1a-134">无</span><span class="sxs-lookup"><span data-stu-id="9fe1a-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fe1a-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9fe1a-135">JSON Representation</span></span>
<span data-ttu-id="9fe1a-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fe1a-136">Here is a JSON representation of the resource.</span></span>
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





