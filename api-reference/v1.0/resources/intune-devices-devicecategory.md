---
title: deviceCategory 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 824cc226c6c11326d0d9683c4a4d46e90de62e89
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755278"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="cf601-103">deviceCategory 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf601-103">deviceCategory resource type</span></span>

<span data-ttu-id="cf601-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf601-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf601-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cf601-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf601-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cf601-106">Not yet documented</span></span>

## <a name="methods"></a><span data-ttu-id="cf601-107">方法</span><span class="sxs-lookup"><span data-stu-id="cf601-107">Methods</span></span>
|<span data-ttu-id="cf601-108">方法</span><span class="sxs-lookup"><span data-stu-id="cf601-108">Method</span></span>|<span data-ttu-id="cf601-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cf601-109">Return Type</span></span>|<span data-ttu-id="cf601-110">说明</span><span class="sxs-lookup"><span data-stu-id="cf601-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cf601-111">获取 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="cf601-111">Get deviceCategory</span></span>](../api/intune-devices-devicecategory-get.md)|[<span data-ttu-id="cf601-112">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="cf601-112">deviceCategory</span></span>](../resources/intune-devices-devicecategory.md)|<span data-ttu-id="cf601-113">读取 [deviceCategory](../resources/intune-devices-devicecategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cf601-113">Read properties and relationships of the [deviceCategory](../resources/intune-devices-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="cf601-114">更新 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="cf601-114">Update deviceCategory</span></span>](../api/intune-devices-devicecategory-update.md)|[<span data-ttu-id="cf601-115">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="cf601-115">deviceCategory</span></span>](../resources/intune-devices-devicecategory.md)|<span data-ttu-id="cf601-116">更新 [deviceCategory](../resources/intune-devices-devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cf601-116">Update the properties of a [deviceCategory](../resources/intune-devices-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cf601-117">属性</span><span class="sxs-lookup"><span data-stu-id="cf601-117">Properties</span></span>
|<span data-ttu-id="cf601-118">属性</span><span class="sxs-lookup"><span data-stu-id="cf601-118">Property</span></span>|<span data-ttu-id="cf601-119">类型</span><span class="sxs-lookup"><span data-stu-id="cf601-119">Type</span></span>|<span data-ttu-id="cf601-120">说明</span><span class="sxs-lookup"><span data-stu-id="cf601-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf601-121">id</span><span class="sxs-lookup"><span data-stu-id="cf601-121">id</span></span>|<span data-ttu-id="cf601-122">String</span><span class="sxs-lookup"><span data-stu-id="cf601-122">String</span></span>|<span data-ttu-id="cf601-123">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cf601-123">Unique identifier for the device category.</span></span> <span data-ttu-id="cf601-124">只读。</span><span class="sxs-lookup"><span data-stu-id="cf601-124">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf601-125">关系</span><span class="sxs-lookup"><span data-stu-id="cf601-125">Relationships</span></span>
<span data-ttu-id="cf601-126">无</span><span class="sxs-lookup"><span data-stu-id="cf601-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf601-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf601-127">JSON Representation</span></span>
<span data-ttu-id="cf601-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf601-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)"
}
```




