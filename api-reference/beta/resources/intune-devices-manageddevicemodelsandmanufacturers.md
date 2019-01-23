---
title: managedDeviceModelsAndManufacturers 资源类型
description: 模型和托管帐户中的设备的制造商 meatadata
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: afcf64cb0e8db4e24ce061490ecc593595690930
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396789"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="be2d5-103">managedDeviceModelsAndManufacturers 资源类型</span><span class="sxs-lookup"><span data-stu-id="be2d5-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="be2d5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="be2d5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="be2d5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="be2d5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be2d5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be2d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be2d5-107">模型和托管帐户中的设备的制造商 meatadata</span><span class="sxs-lookup"><span data-stu-id="be2d5-107">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="be2d5-108">属性</span><span class="sxs-lookup"><span data-stu-id="be2d5-108">Properties</span></span>
|<span data-ttu-id="be2d5-109">属性</span><span class="sxs-lookup"><span data-stu-id="be2d5-109">Property</span></span>|<span data-ttu-id="be2d5-110">类型</span><span class="sxs-lookup"><span data-stu-id="be2d5-110">Type</span></span>|<span data-ttu-id="be2d5-111">说明</span><span class="sxs-lookup"><span data-stu-id="be2d5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be2d5-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="be2d5-112">deviceModels</span></span>|<span data-ttu-id="be2d5-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="be2d5-113">String collection</span></span>|<span data-ttu-id="be2d5-114">模型的托管帐户中的设备的列表</span><span class="sxs-lookup"><span data-stu-id="be2d5-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="be2d5-115">设备制造商</span><span class="sxs-lookup"><span data-stu-id="be2d5-115">deviceManufacturers</span></span>|<span data-ttu-id="be2d5-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="be2d5-116">String collection</span></span>|<span data-ttu-id="be2d5-117">在帐户的托管设备的制造商列表</span><span class="sxs-lookup"><span data-stu-id="be2d5-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="be2d5-118">关系</span><span class="sxs-lookup"><span data-stu-id="be2d5-118">Relationships</span></span>
<span data-ttu-id="be2d5-119">无</span><span class="sxs-lookup"><span data-stu-id="be2d5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be2d5-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be2d5-120">JSON Representation</span></span>
<span data-ttu-id="be2d5-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be2d5-121">Here is a JSON representation of the resource.</span></span>
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




