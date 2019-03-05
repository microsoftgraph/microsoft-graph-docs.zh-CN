---
title: windowsInformationProtectionResourceCollection 资源类型
description: Windows 信息保护资源集合
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74d7549f57ecc59f70aa1af4350544ec21b156ec
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254819"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="006af-103">windowsInformationProtectionResourceCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="006af-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="006af-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="006af-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="006af-105">Windows 信息保护资源集合</span><span class="sxs-lookup"><span data-stu-id="006af-105">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="006af-106">属性</span><span class="sxs-lookup"><span data-stu-id="006af-106">Properties</span></span>
|<span data-ttu-id="006af-107">属性</span><span class="sxs-lookup"><span data-stu-id="006af-107">Property</span></span>|<span data-ttu-id="006af-108">类型</span><span class="sxs-lookup"><span data-stu-id="006af-108">Type</span></span>|<span data-ttu-id="006af-109">说明</span><span class="sxs-lookup"><span data-stu-id="006af-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="006af-110">displayName</span><span class="sxs-lookup"><span data-stu-id="006af-110">displayName</span></span>|<span data-ttu-id="006af-111">String</span><span class="sxs-lookup"><span data-stu-id="006af-111">String</span></span>|<span data-ttu-id="006af-112">显示名称</span><span class="sxs-lookup"><span data-stu-id="006af-112">Display name</span></span>|
|<span data-ttu-id="006af-113">资源</span><span class="sxs-lookup"><span data-stu-id="006af-113">resources</span></span>|<span data-ttu-id="006af-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="006af-114">String collection</span></span>|<span data-ttu-id="006af-115">资源集合</span><span class="sxs-lookup"><span data-stu-id="006af-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="006af-116">关系</span><span class="sxs-lookup"><span data-stu-id="006af-116">Relationships</span></span>
<span data-ttu-id="006af-117">无</span><span class="sxs-lookup"><span data-stu-id="006af-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="006af-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="006af-118">JSON Representation</span></span>
<span data-ttu-id="006af-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="006af-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```



