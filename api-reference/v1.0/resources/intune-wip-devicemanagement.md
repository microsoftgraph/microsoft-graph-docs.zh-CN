---
title: deviceManagement 资源类型
description: 充当所有设备管理功能的容器的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 28b6894dd5c5d7118bb939ce0251108525d9f4c9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751831"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="120a1-103">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="120a1-103">deviceManagement resource type</span></span>

<span data-ttu-id="120a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="120a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="120a1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="120a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="120a1-106">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="120a1-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="120a1-107">方法</span><span class="sxs-lookup"><span data-stu-id="120a1-107">Methods</span></span>
|<span data-ttu-id="120a1-108">方法</span><span class="sxs-lookup"><span data-stu-id="120a1-108">Method</span></span>|<span data-ttu-id="120a1-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="120a1-109">Return Type</span></span>|<span data-ttu-id="120a1-110">说明</span><span class="sxs-lookup"><span data-stu-id="120a1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="120a1-111">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="120a1-111">Get deviceManagement</span></span>](../api/intune-wip-devicemanagement-get.md)|[<span data-ttu-id="120a1-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="120a1-112">deviceManagement</span></span>](../resources/intune-wip-devicemanagement.md)|<span data-ttu-id="120a1-113">读取 [deviceManagement](../resources/intune-wip-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="120a1-113">Read properties and relationships of the [deviceManagement](../resources/intune-wip-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="120a1-114">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="120a1-114">Update deviceManagement</span></span>](../api/intune-wip-devicemanagement-update.md)|[<span data-ttu-id="120a1-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="120a1-115">deviceManagement</span></span>](../resources/intune-wip-devicemanagement.md)|<span data-ttu-id="120a1-116">更新 [deviceManagement](../resources/intune-wip-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="120a1-116">Update the properties of a [deviceManagement](../resources/intune-wip-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="120a1-117">属性</span><span class="sxs-lookup"><span data-stu-id="120a1-117">Properties</span></span>
|<span data-ttu-id="120a1-118">属性</span><span class="sxs-lookup"><span data-stu-id="120a1-118">Property</span></span>|<span data-ttu-id="120a1-119">类型</span><span class="sxs-lookup"><span data-stu-id="120a1-119">Type</span></span>|<span data-ttu-id="120a1-120">说明</span><span class="sxs-lookup"><span data-stu-id="120a1-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="120a1-121">id</span><span class="sxs-lookup"><span data-stu-id="120a1-121">id</span></span>|<span data-ttu-id="120a1-122">String</span><span class="sxs-lookup"><span data-stu-id="120a1-122">String</span></span>|<span data-ttu-id="120a1-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="120a1-123">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="120a1-124">关系</span><span class="sxs-lookup"><span data-stu-id="120a1-124">Relationships</span></span>
|<span data-ttu-id="120a1-125">关系</span><span class="sxs-lookup"><span data-stu-id="120a1-125">Relationship</span></span>|<span data-ttu-id="120a1-126">类型</span><span class="sxs-lookup"><span data-stu-id="120a1-126">Type</span></span>|<span data-ttu-id="120a1-127">说明</span><span class="sxs-lookup"><span data-stu-id="120a1-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="120a1-128">windowsInformationProtectionAppLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="120a1-128">windowsInformationProtectionAppLearningSummaries</span></span>|<span data-ttu-id="120a1-129">[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="120a1-129">[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) collection</span></span>|<span data-ttu-id="120a1-130">Windows 信息保护应用学习摘要。</span><span class="sxs-lookup"><span data-stu-id="120a1-130">The windows information protection app learning summaries.</span></span>|
|<span data-ttu-id="120a1-131">windowsInformationProtectionNetworkLearningSummaries</span><span class="sxs-lookup"><span data-stu-id="120a1-131">windowsInformationProtectionNetworkLearningSummaries</span></span>|<span data-ttu-id="120a1-132">[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="120a1-132">[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) collection</span></span>|<span data-ttu-id="120a1-133">Windows 信息保护网络学习摘要。</span><span class="sxs-lookup"><span data-stu-id="120a1-133">The windows information protection network learning summaries.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="120a1-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="120a1-134">JSON Representation</span></span>
<span data-ttu-id="120a1-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="120a1-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```




