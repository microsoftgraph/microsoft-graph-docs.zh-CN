---
title: iPv6Range 资源类型
description: IPv6 范围定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e6def6fa06d9cad863dcfd8c2cc7bb03f718bab3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530195"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="118ba-103">iPv6Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="118ba-103">iPv6Range resource type</span></span>

<span data-ttu-id="118ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="118ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="118ba-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="118ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="118ba-106">IPv6 范围定义。</span><span class="sxs-lookup"><span data-stu-id="118ba-106">IPv6 Range definition.</span></span>


<span data-ttu-id="118ba-107">继承自 [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="118ba-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="118ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="118ba-108">Properties</span></span>
|<span data-ttu-id="118ba-109">属性</span><span class="sxs-lookup"><span data-stu-id="118ba-109">Property</span></span>|<span data-ttu-id="118ba-110">类型</span><span class="sxs-lookup"><span data-stu-id="118ba-110">Type</span></span>|<span data-ttu-id="118ba-111">说明</span><span class="sxs-lookup"><span data-stu-id="118ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="118ba-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="118ba-112">lowerAddress</span></span>|<span data-ttu-id="118ba-113">字符串</span><span class="sxs-lookup"><span data-stu-id="118ba-113">String</span></span>|<span data-ttu-id="118ba-114">低地址</span><span class="sxs-lookup"><span data-stu-id="118ba-114">Lower address</span></span>|
|<span data-ttu-id="118ba-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="118ba-115">upperAddress</span></span>|<span data-ttu-id="118ba-116">String</span><span class="sxs-lookup"><span data-stu-id="118ba-116">String</span></span>|<span data-ttu-id="118ba-117">地址上限</span><span class="sxs-lookup"><span data-stu-id="118ba-117">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="118ba-118">关系</span><span class="sxs-lookup"><span data-stu-id="118ba-118">Relationships</span></span>
<span data-ttu-id="118ba-119">无</span><span class="sxs-lookup"><span data-stu-id="118ba-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="118ba-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="118ba-120">JSON Representation</span></span>
<span data-ttu-id="118ba-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="118ba-121">Here is a JSON representation of the resource.</span></span>
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




