---
title: deviceAppManagement 资源类型
description: 设备应用管理单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b98aaacf4af9b646bb25f4131150d613e2336a87
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757474"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="c21fe-103">deviceAppManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="c21fe-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="c21fe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c21fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c21fe-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c21fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c21fe-106">设备应用管理单例实体。</span><span class="sxs-lookup"><span data-stu-id="c21fe-106">Device app management singleton entity.</span></span>

## <a name="methods"></a><span data-ttu-id="c21fe-107">方法</span><span class="sxs-lookup"><span data-stu-id="c21fe-107">Methods</span></span>
|<span data-ttu-id="c21fe-108">方法</span><span class="sxs-lookup"><span data-stu-id="c21fe-108">Method</span></span>|<span data-ttu-id="c21fe-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c21fe-109">Return Type</span></span>|<span data-ttu-id="c21fe-110">说明</span><span class="sxs-lookup"><span data-stu-id="c21fe-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c21fe-111">获取 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="c21fe-111">Get deviceAppManagement</span></span>](../api/intune-partnerintegration-deviceappmanagement-get.md)|[<span data-ttu-id="c21fe-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="c21fe-112">deviceAppManagement</span></span>](../resources/intune-partnerintegration-deviceappmanagement.md)|<span data-ttu-id="c21fe-113">读取 [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c21fe-113">Read properties and relationships of the [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="c21fe-114">更新 deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="c21fe-114">Update deviceAppManagement</span></span>](../api/intune-partnerintegration-deviceappmanagement-update.md)|[<span data-ttu-id="c21fe-115">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="c21fe-115">deviceAppManagement</span></span>](../resources/intune-partnerintegration-deviceappmanagement.md)|<span data-ttu-id="c21fe-116">更新 [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c21fe-116">Update the properties of a [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c21fe-117">属性</span><span class="sxs-lookup"><span data-stu-id="c21fe-117">Properties</span></span>
|<span data-ttu-id="c21fe-118">属性</span><span class="sxs-lookup"><span data-stu-id="c21fe-118">Property</span></span>|<span data-ttu-id="c21fe-119">类型</span><span class="sxs-lookup"><span data-stu-id="c21fe-119">Type</span></span>|<span data-ttu-id="c21fe-120">说明</span><span class="sxs-lookup"><span data-stu-id="c21fe-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c21fe-121">id</span><span class="sxs-lookup"><span data-stu-id="c21fe-121">id</span></span>|<span data-ttu-id="c21fe-122">String</span><span class="sxs-lookup"><span data-stu-id="c21fe-122">String</span></span>|<span data-ttu-id="c21fe-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c21fe-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c21fe-124">关系</span><span class="sxs-lookup"><span data-stu-id="c21fe-124">Relationships</span></span>
<span data-ttu-id="c21fe-125">无</span><span class="sxs-lookup"><span data-stu-id="c21fe-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c21fe-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c21fe-126">JSON Representation</span></span>
<span data-ttu-id="c21fe-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c21fe-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




