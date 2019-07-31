---
title: iPv6Range 资源类型
description: IPv6 范围定义。
author: rolyon
localization_priority: Normal
doc_type: resourcePageType
ms.prod: Intune
ms.openlocfilehash: 1f2b46cea71d097955ca9e78cc74f6f0cddd1002
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967371"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="75c62-103">iPv6Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="75c62-103">iPv6Range resource type</span></span>

> <span data-ttu-id="75c62-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="75c62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75c62-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="75c62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75c62-106">IPv6 范围定义。</span><span class="sxs-lookup"><span data-stu-id="75c62-106">IPv6 Range definition.</span></span>


<span data-ttu-id="75c62-107">继承自 [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="75c62-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="75c62-108">属性</span><span class="sxs-lookup"><span data-stu-id="75c62-108">Properties</span></span>
|<span data-ttu-id="75c62-109">属性</span><span class="sxs-lookup"><span data-stu-id="75c62-109">Property</span></span>|<span data-ttu-id="75c62-110">类型</span><span class="sxs-lookup"><span data-stu-id="75c62-110">Type</span></span>|<span data-ttu-id="75c62-111">说明</span><span class="sxs-lookup"><span data-stu-id="75c62-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75c62-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="75c62-112">lowerAddress</span></span>|<span data-ttu-id="75c62-113">String</span><span class="sxs-lookup"><span data-stu-id="75c62-113">String</span></span>|<span data-ttu-id="75c62-114">较低的地址。</span><span class="sxs-lookup"><span data-stu-id="75c62-114">Lower address.</span></span>|
|<span data-ttu-id="75c62-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="75c62-115">upperAddress</span></span>|<span data-ttu-id="75c62-116">String</span><span class="sxs-lookup"><span data-stu-id="75c62-116">String</span></span>|<span data-ttu-id="75c62-117">地址上限。</span><span class="sxs-lookup"><span data-stu-id="75c62-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75c62-118">关系</span><span class="sxs-lookup"><span data-stu-id="75c62-118">Relationships</span></span>
<span data-ttu-id="75c62-119">无</span><span class="sxs-lookup"><span data-stu-id="75c62-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75c62-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75c62-120">JSON Representation</span></span>
<span data-ttu-id="75c62-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75c62-121">Here is a JSON representation of the resource.</span></span>
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





