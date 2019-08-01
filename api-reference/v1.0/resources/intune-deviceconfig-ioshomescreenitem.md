---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d5f7c92b1316b40efd9c87ac39c926669a251d58
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031512"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="61e3d-103">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="61e3d-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="61e3d-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="61e3d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61e3d-105">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="61e3d-105">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="61e3d-106">属性</span><span class="sxs-lookup"><span data-stu-id="61e3d-106">Properties</span></span>
|<span data-ttu-id="61e3d-107">属性</span><span class="sxs-lookup"><span data-stu-id="61e3d-107">Property</span></span>|<span data-ttu-id="61e3d-108">类型</span><span class="sxs-lookup"><span data-stu-id="61e3d-108">Type</span></span>|<span data-ttu-id="61e3d-109">说明</span><span class="sxs-lookup"><span data-stu-id="61e3d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61e3d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="61e3d-110">displayName</span></span>|<span data-ttu-id="61e3d-111">String</span><span class="sxs-lookup"><span data-stu-id="61e3d-111">String</span></span>|<span data-ttu-id="61e3d-112">应用的名称</span><span class="sxs-lookup"><span data-stu-id="61e3d-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="61e3d-113">关系</span><span class="sxs-lookup"><span data-stu-id="61e3d-113">Relationships</span></span>
<span data-ttu-id="61e3d-114">无</span><span class="sxs-lookup"><span data-stu-id="61e3d-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61e3d-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61e3d-115">JSON Representation</span></span>
<span data-ttu-id="61e3d-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61e3d-116">Here is a JSON representation of the resource.</span></span>
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



