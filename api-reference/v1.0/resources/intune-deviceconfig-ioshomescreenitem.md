---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dcd542bee3ad68723752dabf421a961c65683c51
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359087"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="e892c-103">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="e892c-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="e892c-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e892c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e892c-105">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="e892c-105">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="e892c-106">属性</span><span class="sxs-lookup"><span data-stu-id="e892c-106">Properties</span></span>
|<span data-ttu-id="e892c-107">属性</span><span class="sxs-lookup"><span data-stu-id="e892c-107">Property</span></span>|<span data-ttu-id="e892c-108">类型</span><span class="sxs-lookup"><span data-stu-id="e892c-108">Type</span></span>|<span data-ttu-id="e892c-109">说明</span><span class="sxs-lookup"><span data-stu-id="e892c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e892c-110">displayName</span><span class="sxs-lookup"><span data-stu-id="e892c-110">displayName</span></span>|<span data-ttu-id="e892c-111">String</span><span class="sxs-lookup"><span data-stu-id="e892c-111">String</span></span>|<span data-ttu-id="e892c-112">应用的名称</span><span class="sxs-lookup"><span data-stu-id="e892c-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="e892c-113">关系</span><span class="sxs-lookup"><span data-stu-id="e892c-113">Relationships</span></span>
<span data-ttu-id="e892c-114">无</span><span class="sxs-lookup"><span data-stu-id="e892c-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e892c-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e892c-115">JSON Representation</span></span>
<span data-ttu-id="e892c-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e892c-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```




