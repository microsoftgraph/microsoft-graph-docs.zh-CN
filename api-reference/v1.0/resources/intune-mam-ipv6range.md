---
title: iPv6Range 资源类型
description: IPv6 范围定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f171a8ebb28d15e78a30bf542c37a163f0d097f0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258987"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="c7c08-103">iPv6Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7c08-103">iPv6Range resource type</span></span>

> <span data-ttu-id="c7c08-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7c08-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7c08-105">IPv6 范围定义。</span><span class="sxs-lookup"><span data-stu-id="c7c08-105">IPv6 Range definition.</span></span>


<span data-ttu-id="c7c08-106">继承自 [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="c7c08-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7c08-107">属性</span><span class="sxs-lookup"><span data-stu-id="c7c08-107">Properties</span></span>
|<span data-ttu-id="c7c08-108">属性</span><span class="sxs-lookup"><span data-stu-id="c7c08-108">Property</span></span>|<span data-ttu-id="c7c08-109">类型</span><span class="sxs-lookup"><span data-stu-id="c7c08-109">Type</span></span>|<span data-ttu-id="c7c08-110">说明</span><span class="sxs-lookup"><span data-stu-id="c7c08-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7c08-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="c7c08-111">lowerAddress</span></span>|<span data-ttu-id="c7c08-112">String</span><span class="sxs-lookup"><span data-stu-id="c7c08-112">String</span></span>|<span data-ttu-id="c7c08-113">低地址</span><span class="sxs-lookup"><span data-stu-id="c7c08-113">Lower address</span></span>|
|<span data-ttu-id="c7c08-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="c7c08-114">upperAddress</span></span>|<span data-ttu-id="c7c08-115">String</span><span class="sxs-lookup"><span data-stu-id="c7c08-115">String</span></span>|<span data-ttu-id="c7c08-116">地址上限</span><span class="sxs-lookup"><span data-stu-id="c7c08-116">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7c08-117">关系</span><span class="sxs-lookup"><span data-stu-id="c7c08-117">Relationships</span></span>
<span data-ttu-id="c7c08-118">无</span><span class="sxs-lookup"><span data-stu-id="c7c08-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7c08-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7c08-119">JSON Representation</span></span>
<span data-ttu-id="c7c08-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7c08-120">Here is a JSON representation of the resource.</span></span>
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



