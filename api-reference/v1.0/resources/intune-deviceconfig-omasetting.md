---
title: omaSetting 资源类型
description: OMA 设置定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6c1b464d8947bfa0125ba7edc9991b7bc6f34296
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367383"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="5282a-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="5282a-103">omaSetting resource type</span></span>

> <span data-ttu-id="5282a-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5282a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5282a-105">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="5282a-105">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="5282a-106">属性</span><span class="sxs-lookup"><span data-stu-id="5282a-106">Properties</span></span>
|<span data-ttu-id="5282a-107">属性</span><span class="sxs-lookup"><span data-stu-id="5282a-107">Property</span></span>|<span data-ttu-id="5282a-108">类型</span><span class="sxs-lookup"><span data-stu-id="5282a-108">Type</span></span>|<span data-ttu-id="5282a-109">说明</span><span class="sxs-lookup"><span data-stu-id="5282a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5282a-110">displayName</span><span class="sxs-lookup"><span data-stu-id="5282a-110">displayName</span></span>|<span data-ttu-id="5282a-111">字符串</span><span class="sxs-lookup"><span data-stu-id="5282a-111">String</span></span>|<span data-ttu-id="5282a-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="5282a-112">Display Name.</span></span>|
|<span data-ttu-id="5282a-113">说明</span><span class="sxs-lookup"><span data-stu-id="5282a-113">description</span></span>|<span data-ttu-id="5282a-114">String</span><span class="sxs-lookup"><span data-stu-id="5282a-114">String</span></span>|<span data-ttu-id="5282a-115">说明。</span><span class="sxs-lookup"><span data-stu-id="5282a-115">Description.</span></span>|
|<span data-ttu-id="5282a-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="5282a-116">omaUri</span></span>|<span data-ttu-id="5282a-117">String</span><span class="sxs-lookup"><span data-stu-id="5282a-117">String</span></span>|<span data-ttu-id="5282a-118">OMA。</span><span class="sxs-lookup"><span data-stu-id="5282a-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5282a-119">关系</span><span class="sxs-lookup"><span data-stu-id="5282a-119">Relationships</span></span>
<span data-ttu-id="5282a-120">无</span><span class="sxs-lookup"><span data-stu-id="5282a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5282a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5282a-121">JSON Representation</span></span>
<span data-ttu-id="5282a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5282a-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```




