---
title: managedDeviceModelsAndManufacturers 资源类型
description: 帐户中托管设备的模型和制造商 meatadata
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfd8f068305bdae86a0acc9ef5f9113bb0d1c579
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148298"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="82b97-103">managedDeviceModelsAndManufacturers 资源类型</span><span class="sxs-lookup"><span data-stu-id="82b97-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="82b97-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="82b97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82b97-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82b97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82b97-106">帐户中托管设备的模型和制造商 meatadata</span><span class="sxs-lookup"><span data-stu-id="82b97-106">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="82b97-107">属性</span><span class="sxs-lookup"><span data-stu-id="82b97-107">Properties</span></span>
|<span data-ttu-id="82b97-108">属性</span><span class="sxs-lookup"><span data-stu-id="82b97-108">Property</span></span>|<span data-ttu-id="82b97-109">类型</span><span class="sxs-lookup"><span data-stu-id="82b97-109">Type</span></span>|<span data-ttu-id="82b97-110">说明</span><span class="sxs-lookup"><span data-stu-id="82b97-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82b97-111">deviceModels</span><span class="sxs-lookup"><span data-stu-id="82b97-111">deviceModels</span></span>|<span data-ttu-id="82b97-112">String collection</span><span class="sxs-lookup"><span data-stu-id="82b97-112">String collection</span></span>|<span data-ttu-id="82b97-113">帐户中托管设备的模型列表</span><span class="sxs-lookup"><span data-stu-id="82b97-113">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="82b97-114">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="82b97-114">deviceManufacturers</span></span>|<span data-ttu-id="82b97-115">String collection</span><span class="sxs-lookup"><span data-stu-id="82b97-115">String collection</span></span>|<span data-ttu-id="82b97-116">帐户中托管设备的制造商列表</span><span class="sxs-lookup"><span data-stu-id="82b97-116">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="82b97-117">关系</span><span class="sxs-lookup"><span data-stu-id="82b97-117">Relationships</span></span>
<span data-ttu-id="82b97-118">无</span><span class="sxs-lookup"><span data-stu-id="82b97-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82b97-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82b97-119">JSON Representation</span></span>
<span data-ttu-id="82b97-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82b97-120">Here is a JSON representation of the resource.</span></span>
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




