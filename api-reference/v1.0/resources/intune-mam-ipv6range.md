---
title: iPv6Range 资源类型
description: IPv6 范围定义。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b0e0b733ceea2585198a46e62d0f033b76748035
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439367"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="80329-103">iPv6Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="80329-103">iPv6Range resource type</span></span>

<span data-ttu-id="80329-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80329-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80329-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="80329-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80329-106">IPv6 范围定义。</span><span class="sxs-lookup"><span data-stu-id="80329-106">IPv6 Range definition.</span></span>


<span data-ttu-id="80329-107">继承自 [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="80329-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="80329-108">属性</span><span class="sxs-lookup"><span data-stu-id="80329-108">Properties</span></span>
|<span data-ttu-id="80329-109">属性</span><span class="sxs-lookup"><span data-stu-id="80329-109">Property</span></span>|<span data-ttu-id="80329-110">类型</span><span class="sxs-lookup"><span data-stu-id="80329-110">Type</span></span>|<span data-ttu-id="80329-111">说明</span><span class="sxs-lookup"><span data-stu-id="80329-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80329-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="80329-112">lowerAddress</span></span>|<span data-ttu-id="80329-113">String</span><span class="sxs-lookup"><span data-stu-id="80329-113">String</span></span>|<span data-ttu-id="80329-114">低地址</span><span class="sxs-lookup"><span data-stu-id="80329-114">Lower address</span></span>|
|<span data-ttu-id="80329-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="80329-115">upperAddress</span></span>|<span data-ttu-id="80329-116">String</span><span class="sxs-lookup"><span data-stu-id="80329-116">String</span></span>|<span data-ttu-id="80329-117">地址上限</span><span class="sxs-lookup"><span data-stu-id="80329-117">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="80329-118">关系</span><span class="sxs-lookup"><span data-stu-id="80329-118">Relationships</span></span>
<span data-ttu-id="80329-119">无</span><span class="sxs-lookup"><span data-stu-id="80329-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80329-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80329-120">JSON Representation</span></span>
<span data-ttu-id="80329-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80329-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```







