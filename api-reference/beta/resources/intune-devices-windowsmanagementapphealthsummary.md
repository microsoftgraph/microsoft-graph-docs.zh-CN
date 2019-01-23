---
title: windowsManagementAppHealthSummary 资源类型
description: 包含 Windows 管理应用程序的运行状况摘要属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3ca46f61259b8b956439c541bf8d5703a35aa93b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393849"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="7714a-103">windowsManagementAppHealthSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="7714a-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="7714a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="7714a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7714a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7714a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7714a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7714a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7714a-107">包含 Windows 管理应用程序的运行状况摘要属性。</span><span class="sxs-lookup"><span data-stu-id="7714a-107">Contains properties for the health summary of the Windows management app.</span></span>

## <a name="methods"></a><span data-ttu-id="7714a-108">方法</span><span class="sxs-lookup"><span data-stu-id="7714a-108">Methods</span></span>
|<span data-ttu-id="7714a-109">方法</span><span class="sxs-lookup"><span data-stu-id="7714a-109">Method</span></span>|<span data-ttu-id="7714a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7714a-110">Return Type</span></span>|<span data-ttu-id="7714a-111">说明</span><span class="sxs-lookup"><span data-stu-id="7714a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7714a-112">获取 windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="7714a-112">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="7714a-113">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="7714a-113">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="7714a-114">读取属性和[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="7714a-114">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="7714a-115">更新 windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="7714a-115">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="7714a-116">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="7714a-116">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="7714a-117">更新[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7714a-117">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7714a-118">属性</span><span class="sxs-lookup"><span data-stu-id="7714a-118">Properties</span></span>
|<span data-ttu-id="7714a-119">属性</span><span class="sxs-lookup"><span data-stu-id="7714a-119">Property</span></span>|<span data-ttu-id="7714a-120">类型</span><span class="sxs-lookup"><span data-stu-id="7714a-120">Type</span></span>|<span data-ttu-id="7714a-121">说明</span><span class="sxs-lookup"><span data-stu-id="7714a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7714a-122">id</span><span class="sxs-lookup"><span data-stu-id="7714a-122">id</span></span>|<span data-ttu-id="7714a-123">String</span><span class="sxs-lookup"><span data-stu-id="7714a-123">String</span></span>|<span data-ttu-id="7714a-124">Windows 管理应用程序运行状况摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="7714a-124">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="7714a-125">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7714a-125">healthyDeviceCount</span></span>|<span data-ttu-id="7714a-126">Int32</span><span class="sxs-lookup"><span data-stu-id="7714a-126">Int32</span></span>|<span data-ttu-id="7714a-127">正常运行的设备计数。</span><span class="sxs-lookup"><span data-stu-id="7714a-127">Healthy device count.</span></span>|
|<span data-ttu-id="7714a-128">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7714a-128">unhealthyDeviceCount</span></span>|<span data-ttu-id="7714a-129">Int32</span><span class="sxs-lookup"><span data-stu-id="7714a-129">Int32</span></span>|<span data-ttu-id="7714a-130">正常设备计数。</span><span class="sxs-lookup"><span data-stu-id="7714a-130">Unhealthy device count.</span></span>|
|<span data-ttu-id="7714a-131">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7714a-131">unknownDeviceCount</span></span>|<span data-ttu-id="7714a-132">Int32</span><span class="sxs-lookup"><span data-stu-id="7714a-132">Int32</span></span>|<span data-ttu-id="7714a-133">未知的设备计数。</span><span class="sxs-lookup"><span data-stu-id="7714a-133">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7714a-134">关系</span><span class="sxs-lookup"><span data-stu-id="7714a-134">Relationships</span></span>
<span data-ttu-id="7714a-135">无</span><span class="sxs-lookup"><span data-stu-id="7714a-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7714a-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7714a-136">JSON Representation</span></span>
<span data-ttu-id="7714a-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7714a-137">Here is a JSON representation of the resource.</span></span>
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




