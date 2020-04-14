---
title: iPv6Range 资源类型
description: IPv6 范围定义。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 77037ad6e8635a9e83da6fb727b30406e77304b4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473580"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="e2b57-103">iPv6Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2b57-103">iPv6Range resource type</span></span>

<span data-ttu-id="e2b57-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2b57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2b57-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e2b57-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2b57-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2b57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2b57-107">IPv6 范围定义。</span><span class="sxs-lookup"><span data-stu-id="e2b57-107">IPv6 Range definition.</span></span>


<span data-ttu-id="e2b57-108">继承自 [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e2b57-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e2b57-109">属性</span><span class="sxs-lookup"><span data-stu-id="e2b57-109">Properties</span></span>
|<span data-ttu-id="e2b57-110">属性</span><span class="sxs-lookup"><span data-stu-id="e2b57-110">Property</span></span>|<span data-ttu-id="e2b57-111">类型</span><span class="sxs-lookup"><span data-stu-id="e2b57-111">Type</span></span>|<span data-ttu-id="e2b57-112">说明</span><span class="sxs-lookup"><span data-stu-id="e2b57-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2b57-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="e2b57-113">lowerAddress</span></span>|<span data-ttu-id="e2b57-114">String</span><span class="sxs-lookup"><span data-stu-id="e2b57-114">String</span></span>|<span data-ttu-id="e2b57-115">较低的地址。</span><span class="sxs-lookup"><span data-stu-id="e2b57-115">Lower address.</span></span>|
|<span data-ttu-id="e2b57-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="e2b57-116">upperAddress</span></span>|<span data-ttu-id="e2b57-117">String</span><span class="sxs-lookup"><span data-stu-id="e2b57-117">String</span></span>|<span data-ttu-id="e2b57-118">地址上限。</span><span class="sxs-lookup"><span data-stu-id="e2b57-118">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2b57-119">关系</span><span class="sxs-lookup"><span data-stu-id="e2b57-119">Relationships</span></span>
<span data-ttu-id="e2b57-120">无</span><span class="sxs-lookup"><span data-stu-id="e2b57-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2b57-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2b57-121">JSON Representation</span></span>
<span data-ttu-id="e2b57-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2b57-122">Here is a JSON representation of the resource.</span></span>
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



