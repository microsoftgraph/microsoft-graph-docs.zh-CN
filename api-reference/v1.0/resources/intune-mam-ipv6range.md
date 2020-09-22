---
title: iPv6Range 资源类型
description: IPv6 范围定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a7bdde3831a3634dce25e562ea1d1a332c18fac2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984423"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="4d1a2-103">iPv6Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d1a2-103">iPv6Range resource type</span></span>

<span data-ttu-id="4d1a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d1a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d1a2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4d1a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d1a2-106">IPv6 范围定义。</span><span class="sxs-lookup"><span data-stu-id="4d1a2-106">IPv6 Range definition.</span></span>


<span data-ttu-id="4d1a2-107">继承自 [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="4d1a2-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4d1a2-108">属性</span><span class="sxs-lookup"><span data-stu-id="4d1a2-108">Properties</span></span>
|<span data-ttu-id="4d1a2-109">属性</span><span class="sxs-lookup"><span data-stu-id="4d1a2-109">Property</span></span>|<span data-ttu-id="4d1a2-110">类型</span><span class="sxs-lookup"><span data-stu-id="4d1a2-110">Type</span></span>|<span data-ttu-id="4d1a2-111">说明</span><span class="sxs-lookup"><span data-stu-id="4d1a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d1a2-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="4d1a2-112">lowerAddress</span></span>|<span data-ttu-id="4d1a2-113">String</span><span class="sxs-lookup"><span data-stu-id="4d1a2-113">String</span></span>|<span data-ttu-id="4d1a2-114">低地址</span><span class="sxs-lookup"><span data-stu-id="4d1a2-114">Lower address</span></span>|
|<span data-ttu-id="4d1a2-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="4d1a2-115">upperAddress</span></span>|<span data-ttu-id="4d1a2-116">String</span><span class="sxs-lookup"><span data-stu-id="4d1a2-116">String</span></span>|<span data-ttu-id="4d1a2-117">地址上限</span><span class="sxs-lookup"><span data-stu-id="4d1a2-117">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d1a2-118">关系</span><span class="sxs-lookup"><span data-stu-id="4d1a2-118">Relationships</span></span>
<span data-ttu-id="4d1a2-119">无</span><span class="sxs-lookup"><span data-stu-id="4d1a2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d1a2-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d1a2-120">JSON Representation</span></span>
<span data-ttu-id="4d1a2-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d1a2-121">Here is a JSON representation of the resource.</span></span>
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









