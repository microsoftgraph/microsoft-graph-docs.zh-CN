---
title: managedDeviceModelsAndManufacturers 资源类型
description: 模型和托管帐户中的设备的制造商 meatadata
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8a1769f82153fd8184807877c484a4dc31ebda1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927525"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="7e7bb-103">managedDeviceModelsAndManufacturers 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e7bb-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="7e7bb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7e7bb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e7bb-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7e7bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e7bb-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7e7bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e7bb-107">模型和托管帐户中的设备的制造商 meatadata</span><span class="sxs-lookup"><span data-stu-id="7e7bb-107">Models and Manufactures meatadata for managed devices in the account</span></span>
## <a name="properties"></a><span data-ttu-id="7e7bb-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e7bb-108">Properties</span></span>
|<span data-ttu-id="7e7bb-109">属性</span><span class="sxs-lookup"><span data-stu-id="7e7bb-109">Property</span></span>|<span data-ttu-id="7e7bb-110">类型</span><span class="sxs-lookup"><span data-stu-id="7e7bb-110">Type</span></span>|<span data-ttu-id="7e7bb-111">Description</span><span class="sxs-lookup"><span data-stu-id="7e7bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e7bb-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="7e7bb-112">deviceModels</span></span>|<span data-ttu-id="7e7bb-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="7e7bb-113">String collection</span></span>|<span data-ttu-id="7e7bb-114">模型的托管帐户中的设备的列表</span><span class="sxs-lookup"><span data-stu-id="7e7bb-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="7e7bb-115">设备制造商</span><span class="sxs-lookup"><span data-stu-id="7e7bb-115">deviceManufacturers</span></span>|<span data-ttu-id="7e7bb-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="7e7bb-116">String collection</span></span>|<span data-ttu-id="7e7bb-117">在帐户的托管设备的制造商列表</span><span class="sxs-lookup"><span data-stu-id="7e7bb-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e7bb-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="7e7bb-118">Relationships</span></span>
<span data-ttu-id="7e7bb-119">无</span><span class="sxs-lookup"><span data-stu-id="7e7bb-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7e7bb-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e7bb-120">JSON Representation</span></span>
<span data-ttu-id="7e7bb-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e7bb-121">Here is a JSON representation of the resource.</span></span>
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





