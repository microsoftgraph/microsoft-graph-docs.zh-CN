---
title: windowsManagementAppHealthSummary 资源类型
description: 包含 Windows 管理应用程序的运行状况摘要属性。
author: tfitzmac
ms.openlocfilehash: 5717f96cbac534f2726ccf7bcfcbdb54d4c17b28
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326227"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="56859-103">windowsManagementAppHealthSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="56859-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="56859-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="56859-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56859-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="56859-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56859-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="56859-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56859-107">包含 Windows 管理应用程序的运行状况摘要属性。</span><span class="sxs-lookup"><span data-stu-id="56859-107">Contains properties for the health summary of the Windows management app.</span></span>
## <a name="methods"></a><span data-ttu-id="56859-108">方法</span><span class="sxs-lookup"><span data-stu-id="56859-108">Methods</span></span>
|<span data-ttu-id="56859-109">方法</span><span class="sxs-lookup"><span data-stu-id="56859-109">Method</span></span>|<span data-ttu-id="56859-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="56859-110">Return Type</span></span>|<span data-ttu-id="56859-111">说明</span><span class="sxs-lookup"><span data-stu-id="56859-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="56859-112">获取 windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="56859-112">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="56859-113">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="56859-113">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="56859-114">读取属性和[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="56859-114">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="56859-115">更新 windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="56859-115">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="56859-116">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="56859-116">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="56859-117">更新[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="56859-117">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="56859-118">属性</span><span class="sxs-lookup"><span data-stu-id="56859-118">Properties</span></span>
|<span data-ttu-id="56859-119">属性</span><span class="sxs-lookup"><span data-stu-id="56859-119">Property</span></span>|<span data-ttu-id="56859-120">类型</span><span class="sxs-lookup"><span data-stu-id="56859-120">Type</span></span>|<span data-ttu-id="56859-121">说明</span><span class="sxs-lookup"><span data-stu-id="56859-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56859-122">id</span><span class="sxs-lookup"><span data-stu-id="56859-122">id</span></span>|<span data-ttu-id="56859-123">字符串</span><span class="sxs-lookup"><span data-stu-id="56859-123">String</span></span>|<span data-ttu-id="56859-124">Windows 管理应用程序运行状况摘要实体的键。</span><span class="sxs-lookup"><span data-stu-id="56859-124">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="56859-125">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56859-125">healthyDeviceCount</span></span>|<span data-ttu-id="56859-126">Int32</span><span class="sxs-lookup"><span data-stu-id="56859-126">Int32</span></span>|<span data-ttu-id="56859-127">正常运行的设备计数。</span><span class="sxs-lookup"><span data-stu-id="56859-127">Healthy device count.</span></span>|
|<span data-ttu-id="56859-128">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56859-128">unhealthyDeviceCount</span></span>|<span data-ttu-id="56859-129">Int32</span><span class="sxs-lookup"><span data-stu-id="56859-129">Int32</span></span>|<span data-ttu-id="56859-130">正常设备计数。</span><span class="sxs-lookup"><span data-stu-id="56859-130">Unhealthy device count.</span></span>|
|<span data-ttu-id="56859-131">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="56859-131">unknownDeviceCount</span></span>|<span data-ttu-id="56859-132">Int32</span><span class="sxs-lookup"><span data-stu-id="56859-132">Int32</span></span>|<span data-ttu-id="56859-133">未知的设备计数。</span><span class="sxs-lookup"><span data-stu-id="56859-133">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56859-134">Relationships</span><span class="sxs-lookup"><span data-stu-id="56859-134">Relationships</span></span>
<span data-ttu-id="56859-135">无</span><span class="sxs-lookup"><span data-stu-id="56859-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="56859-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56859-136">JSON Representation</span></span>
<span data-ttu-id="56859-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56859-137">Here is a JSON representation of the resource.</span></span>
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





