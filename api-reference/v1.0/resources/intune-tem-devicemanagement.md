---
title: deviceManagement 资源类型
description: 充当所有设备管理功能的容器的单例实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 847ba54fd3cb755d6ade878112e15deffb5d8812
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757469"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="a76a9-103">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="a76a9-103">deviceManagement resource type</span></span>

<span data-ttu-id="a76a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a76a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a76a9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a76a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a76a9-106">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="a76a9-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="a76a9-107">方法</span><span class="sxs-lookup"><span data-stu-id="a76a9-107">Methods</span></span>
|<span data-ttu-id="a76a9-108">方法</span><span class="sxs-lookup"><span data-stu-id="a76a9-108">Method</span></span>|<span data-ttu-id="a76a9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a76a9-109">Return Type</span></span>|<span data-ttu-id="a76a9-110">说明</span><span class="sxs-lookup"><span data-stu-id="a76a9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a76a9-111">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="a76a9-111">Get deviceManagement</span></span>](../api/intune-tem-devicemanagement-get.md)|[<span data-ttu-id="a76a9-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="a76a9-112">deviceManagement</span></span>](../resources/intune-tem-devicemanagement.md)|<span data-ttu-id="a76a9-113">读取 [deviceManagement](../resources/intune-tem-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a76a9-113">Read properties and relationships of the [deviceManagement](../resources/intune-tem-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="a76a9-114">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="a76a9-114">Update deviceManagement</span></span>](../api/intune-tem-devicemanagement-update.md)|[<span data-ttu-id="a76a9-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="a76a9-115">deviceManagement</span></span>](../resources/intune-tem-devicemanagement.md)|<span data-ttu-id="a76a9-116">更新 [deviceManagement](../resources/intune-tem-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a76a9-116">Update the properties of a [deviceManagement](../resources/intune-tem-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a76a9-117">属性</span><span class="sxs-lookup"><span data-stu-id="a76a9-117">Properties</span></span>
|<span data-ttu-id="a76a9-118">属性</span><span class="sxs-lookup"><span data-stu-id="a76a9-118">Property</span></span>|<span data-ttu-id="a76a9-119">类型</span><span class="sxs-lookup"><span data-stu-id="a76a9-119">Type</span></span>|<span data-ttu-id="a76a9-120">说明</span><span class="sxs-lookup"><span data-stu-id="a76a9-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a76a9-121">id</span><span class="sxs-lookup"><span data-stu-id="a76a9-121">id</span></span>|<span data-ttu-id="a76a9-122">String</span><span class="sxs-lookup"><span data-stu-id="a76a9-122">String</span></span>|<span data-ttu-id="a76a9-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a76a9-123">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="a76a9-124">关系</span><span class="sxs-lookup"><span data-stu-id="a76a9-124">Relationships</span></span>
|<span data-ttu-id="a76a9-125">关系</span><span class="sxs-lookup"><span data-stu-id="a76a9-125">Relationship</span></span>|<span data-ttu-id="a76a9-126">类型</span><span class="sxs-lookup"><span data-stu-id="a76a9-126">Type</span></span>|<span data-ttu-id="a76a9-127">说明</span><span class="sxs-lookup"><span data-stu-id="a76a9-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a76a9-128">telecomExpenseManagementPartners</span><span class="sxs-lookup"><span data-stu-id="a76a9-128">telecomExpenseManagementPartners</span></span>|<span data-ttu-id="a76a9-129">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a76a9-129">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) collection</span></span>|<span data-ttu-id="a76a9-130">电信费用管理合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="a76a9-130">The telecom expense management partners.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a76a9-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a76a9-131">JSON Representation</span></span>
<span data-ttu-id="a76a9-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a76a9-132">Here is a JSON representation of the resource.</span></span>
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




