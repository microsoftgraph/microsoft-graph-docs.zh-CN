---
title: iPv6Range 资源类型
description: IPv6 范围定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 04183f443d767236a1a7c0afb1d1ed9b92c37889
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038140"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="55e71-103">iPv6Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="55e71-103">iPv6Range resource type</span></span>

> <span data-ttu-id="55e71-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="55e71-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55e71-105">IPv6 范围定义。</span><span class="sxs-lookup"><span data-stu-id="55e71-105">IPv6 Range definition.</span></span>


<span data-ttu-id="55e71-106">继承自 [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="55e71-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="55e71-107">属性</span><span class="sxs-lookup"><span data-stu-id="55e71-107">Properties</span></span>
|<span data-ttu-id="55e71-108">属性</span><span class="sxs-lookup"><span data-stu-id="55e71-108">Property</span></span>|<span data-ttu-id="55e71-109">类型</span><span class="sxs-lookup"><span data-stu-id="55e71-109">Type</span></span>|<span data-ttu-id="55e71-110">说明</span><span class="sxs-lookup"><span data-stu-id="55e71-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55e71-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="55e71-111">lowerAddress</span></span>|<span data-ttu-id="55e71-112">String</span><span class="sxs-lookup"><span data-stu-id="55e71-112">String</span></span>|<span data-ttu-id="55e71-113">低地址</span><span class="sxs-lookup"><span data-stu-id="55e71-113">Lower address</span></span>|
|<span data-ttu-id="55e71-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="55e71-114">upperAddress</span></span>|<span data-ttu-id="55e71-115">String</span><span class="sxs-lookup"><span data-stu-id="55e71-115">String</span></span>|<span data-ttu-id="55e71-116">地址上限</span><span class="sxs-lookup"><span data-stu-id="55e71-116">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="55e71-117">关系</span><span class="sxs-lookup"><span data-stu-id="55e71-117">Relationships</span></span>
<span data-ttu-id="55e71-118">无</span><span class="sxs-lookup"><span data-stu-id="55e71-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55e71-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55e71-119">JSON Representation</span></span>
<span data-ttu-id="55e71-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55e71-120">Here is a JSON representation of the resource.</span></span>
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



