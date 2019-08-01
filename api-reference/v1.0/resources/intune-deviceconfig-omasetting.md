---
title: omaSetting 资源类型
description: OMA 设置定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5a2d2152d107050f655d43dab2cb2c65f114868
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031344"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="6aed0-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="6aed0-103">omaSetting resource type</span></span>

> <span data-ttu-id="6aed0-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6aed0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aed0-105">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="6aed0-105">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="6aed0-106">属性</span><span class="sxs-lookup"><span data-stu-id="6aed0-106">Properties</span></span>
|<span data-ttu-id="6aed0-107">属性</span><span class="sxs-lookup"><span data-stu-id="6aed0-107">Property</span></span>|<span data-ttu-id="6aed0-108">类型</span><span class="sxs-lookup"><span data-stu-id="6aed0-108">Type</span></span>|<span data-ttu-id="6aed0-109">说明</span><span class="sxs-lookup"><span data-stu-id="6aed0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aed0-110">displayName</span><span class="sxs-lookup"><span data-stu-id="6aed0-110">displayName</span></span>|<span data-ttu-id="6aed0-111">字符串</span><span class="sxs-lookup"><span data-stu-id="6aed0-111">String</span></span>|<span data-ttu-id="6aed0-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="6aed0-112">Display Name.</span></span>|
|<span data-ttu-id="6aed0-113">说明</span><span class="sxs-lookup"><span data-stu-id="6aed0-113">description</span></span>|<span data-ttu-id="6aed0-114">String</span><span class="sxs-lookup"><span data-stu-id="6aed0-114">String</span></span>|<span data-ttu-id="6aed0-115">说明。</span><span class="sxs-lookup"><span data-stu-id="6aed0-115">Description.</span></span>|
|<span data-ttu-id="6aed0-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="6aed0-116">omaUri</span></span>|<span data-ttu-id="6aed0-117">String</span><span class="sxs-lookup"><span data-stu-id="6aed0-117">String</span></span>|<span data-ttu-id="6aed0-118">OMA。</span><span class="sxs-lookup"><span data-stu-id="6aed0-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6aed0-119">关系</span><span class="sxs-lookup"><span data-stu-id="6aed0-119">Relationships</span></span>
<span data-ttu-id="6aed0-120">无</span><span class="sxs-lookup"><span data-stu-id="6aed0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6aed0-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6aed0-121">JSON Representation</span></span>
<span data-ttu-id="6aed0-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6aed0-122">Here is a JSON representation of the resource.</span></span>
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



