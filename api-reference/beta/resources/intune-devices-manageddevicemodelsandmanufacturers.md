---
title: managedDeviceModelsAndManufacturers 资源类型
description: 帐户中托管设备的模型和制造商 meatadata
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7cfedad0fce093d8fc3358afcf622ac8beb58d6b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999772"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="4dda9-103">managedDeviceModelsAndManufacturers 资源类型</span><span class="sxs-lookup"><span data-stu-id="4dda9-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="4dda9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4dda9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dda9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4dda9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dda9-106">帐户中托管设备的模型和制造商 meatadata</span><span class="sxs-lookup"><span data-stu-id="4dda9-106">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="4dda9-107">属性</span><span class="sxs-lookup"><span data-stu-id="4dda9-107">Properties</span></span>
|<span data-ttu-id="4dda9-108">属性</span><span class="sxs-lookup"><span data-stu-id="4dda9-108">Property</span></span>|<span data-ttu-id="4dda9-109">类型</span><span class="sxs-lookup"><span data-stu-id="4dda9-109">Type</span></span>|<span data-ttu-id="4dda9-110">说明</span><span class="sxs-lookup"><span data-stu-id="4dda9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dda9-111">deviceModels</span><span class="sxs-lookup"><span data-stu-id="4dda9-111">deviceModels</span></span>|<span data-ttu-id="4dda9-112">String collection</span><span class="sxs-lookup"><span data-stu-id="4dda9-112">String collection</span></span>|<span data-ttu-id="4dda9-113">帐户中托管设备的模型列表</span><span class="sxs-lookup"><span data-stu-id="4dda9-113">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="4dda9-114">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="4dda9-114">deviceManufacturers</span></span>|<span data-ttu-id="4dda9-115">String collection</span><span class="sxs-lookup"><span data-stu-id="4dda9-115">String collection</span></span>|<span data-ttu-id="4dda9-116">帐户中托管设备的制造商列表</span><span class="sxs-lookup"><span data-stu-id="4dda9-116">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dda9-117">关系</span><span class="sxs-lookup"><span data-stu-id="4dda9-117">Relationships</span></span>
<span data-ttu-id="4dda9-118">无</span><span class="sxs-lookup"><span data-stu-id="4dda9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4dda9-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4dda9-119">JSON Representation</span></span>
<span data-ttu-id="4dda9-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4dda9-120">Here is a JSON representation of the resource.</span></span>
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





