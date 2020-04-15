---
title: omaSetting 资源类型
description: OMA 设置定义。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0172d3cb6955df6e154758750fdc87aef2789292
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473076"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="21980-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="21980-103">omaSetting resource type</span></span>

<span data-ttu-id="21980-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21980-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21980-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21980-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21980-106">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="21980-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="21980-107">属性</span><span class="sxs-lookup"><span data-stu-id="21980-107">Properties</span></span>
|<span data-ttu-id="21980-108">属性</span><span class="sxs-lookup"><span data-stu-id="21980-108">Property</span></span>|<span data-ttu-id="21980-109">类型</span><span class="sxs-lookup"><span data-stu-id="21980-109">Type</span></span>|<span data-ttu-id="21980-110">说明</span><span class="sxs-lookup"><span data-stu-id="21980-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21980-111">displayName</span><span class="sxs-lookup"><span data-stu-id="21980-111">displayName</span></span>|<span data-ttu-id="21980-112">字符串</span><span class="sxs-lookup"><span data-stu-id="21980-112">String</span></span>|<span data-ttu-id="21980-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="21980-113">Display Name.</span></span>|
|<span data-ttu-id="21980-114">description</span><span class="sxs-lookup"><span data-stu-id="21980-114">description</span></span>|<span data-ttu-id="21980-115">String</span><span class="sxs-lookup"><span data-stu-id="21980-115">String</span></span>|<span data-ttu-id="21980-116">说明。</span><span class="sxs-lookup"><span data-stu-id="21980-116">Description.</span></span>|
|<span data-ttu-id="21980-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="21980-117">omaUri</span></span>|<span data-ttu-id="21980-118">String</span><span class="sxs-lookup"><span data-stu-id="21980-118">String</span></span>|<span data-ttu-id="21980-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="21980-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21980-120">关系</span><span class="sxs-lookup"><span data-stu-id="21980-120">Relationships</span></span>
<span data-ttu-id="21980-121">无</span><span class="sxs-lookup"><span data-stu-id="21980-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21980-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21980-122">JSON Representation</span></span>
<span data-ttu-id="21980-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21980-123">Here is a JSON representation of the resource.</span></span>
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







