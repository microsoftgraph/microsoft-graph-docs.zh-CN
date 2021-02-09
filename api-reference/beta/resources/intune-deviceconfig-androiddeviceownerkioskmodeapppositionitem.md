---
title: androidDeviceOwnerKioskModeAppPositionItem 资源类型
description: 应用位置列表中的一个项目，用于设置托管主屏幕上的项目顺序
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 788b7ac612fd025bb778c387be2051769de66ccb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160202"
---
# <a name="androiddeviceownerkioskmodeapppositionitem-resource-type"></a><span data-ttu-id="91562-103">androidDeviceOwnerKioskModeAppPositionItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="91562-103">androidDeviceOwnerKioskModeAppPositionItem resource type</span></span>

<span data-ttu-id="91562-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91562-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91562-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="91562-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91562-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="91562-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91562-107">应用位置列表中的一个项目，用于设置托管主屏幕上的项目顺序</span><span class="sxs-lookup"><span data-stu-id="91562-107">An item in the list of app positions that sets the order of items on the Managed Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="91562-108">属性</span><span class="sxs-lookup"><span data-stu-id="91562-108">Properties</span></span>
|<span data-ttu-id="91562-109">属性</span><span class="sxs-lookup"><span data-stu-id="91562-109">Property</span></span>|<span data-ttu-id="91562-110">类型</span><span class="sxs-lookup"><span data-stu-id="91562-110">Type</span></span>|<span data-ttu-id="91562-111">说明</span><span class="sxs-lookup"><span data-stu-id="91562-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91562-112">position</span><span class="sxs-lookup"><span data-stu-id="91562-112">position</span></span>|<span data-ttu-id="91562-113">Int32</span><span class="sxs-lookup"><span data-stu-id="91562-113">Int32</span></span>|<span data-ttu-id="91562-114">项在网格上的位置。</span><span class="sxs-lookup"><span data-stu-id="91562-114">Position of the item on the grid.</span></span> <span data-ttu-id="91562-115">有效值为 0 到 9999999</span><span class="sxs-lookup"><span data-stu-id="91562-115">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="91562-116">项</span><span class="sxs-lookup"><span data-stu-id="91562-116">item</span></span>|[<span data-ttu-id="91562-117">androidDeviceOwnerKioskModeHomeScreenItem</span><span class="sxs-lookup"><span data-stu-id="91562-117">androidDeviceOwnerKioskModeHomeScreenItem</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)|<span data-ttu-id="91562-118">要排列的项目</span><span class="sxs-lookup"><span data-stu-id="91562-118">Item to be arranged</span></span>|

## <a name="relationships"></a><span data-ttu-id="91562-119">关系</span><span class="sxs-lookup"><span data-stu-id="91562-119">Relationships</span></span>
<span data-ttu-id="91562-120">无</span><span class="sxs-lookup"><span data-stu-id="91562-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91562-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91562-121">JSON Representation</span></span>
<span data-ttu-id="91562-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91562-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
  "position": 1024,
  "item": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
    "label": "String",
    "link": "String"
  }
}
```




