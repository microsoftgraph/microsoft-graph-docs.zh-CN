---
title: managedDeviceModelsAndManufacturers 资源类型
description: 帐户中托管设备的模型和制造商 meatadata
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: db6d5a59a748f5e8befbe662a0b317a185437665
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443952"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="0f3b0-103">managedDeviceModelsAndManufacturers 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f3b0-103">managedDeviceModelsAndManufacturers resource type</span></span>

<span data-ttu-id="0f3b0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f3b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f3b0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0f3b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f3b0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f3b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f3b0-107">帐户中托管设备的模型和制造商 meatadata</span><span class="sxs-lookup"><span data-stu-id="0f3b0-107">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="0f3b0-108">属性</span><span class="sxs-lookup"><span data-stu-id="0f3b0-108">Properties</span></span>
|<span data-ttu-id="0f3b0-109">属性</span><span class="sxs-lookup"><span data-stu-id="0f3b0-109">Property</span></span>|<span data-ttu-id="0f3b0-110">类型</span><span class="sxs-lookup"><span data-stu-id="0f3b0-110">Type</span></span>|<span data-ttu-id="0f3b0-111">说明</span><span class="sxs-lookup"><span data-stu-id="0f3b0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f3b0-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="0f3b0-112">deviceModels</span></span>|<span data-ttu-id="0f3b0-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="0f3b0-113">String collection</span></span>|<span data-ttu-id="0f3b0-114">帐户中托管设备的模型列表</span><span class="sxs-lookup"><span data-stu-id="0f3b0-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="0f3b0-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="0f3b0-115">deviceManufacturers</span></span>|<span data-ttu-id="0f3b0-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="0f3b0-116">String collection</span></span>|<span data-ttu-id="0f3b0-117">帐户中托管设备的制造商列表</span><span class="sxs-lookup"><span data-stu-id="0f3b0-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f3b0-118">关系</span><span class="sxs-lookup"><span data-stu-id="0f3b0-118">Relationships</span></span>
<span data-ttu-id="0f3b0-119">无</span><span class="sxs-lookup"><span data-stu-id="0f3b0-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f3b0-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f3b0-120">JSON Representation</span></span>
<span data-ttu-id="0f3b0-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f3b0-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```



