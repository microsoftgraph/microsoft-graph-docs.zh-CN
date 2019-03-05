---
title: iPv4Range 资源类型
description: IPv4 范围定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 521c27396c483ba07cc39aec583dd3e610da267d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160513"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="eec5a-103">iPv4Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="eec5a-103">iPv4Range resource type</span></span>

> <span data-ttu-id="eec5a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eec5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eec5a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eec5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eec5a-106">IPv4 范围定义。</span><span class="sxs-lookup"><span data-stu-id="eec5a-106">IPv4 Range definition.</span></span>


<span data-ttu-id="eec5a-107">继承自 [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="eec5a-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eec5a-108">属性</span><span class="sxs-lookup"><span data-stu-id="eec5a-108">Properties</span></span>
|<span data-ttu-id="eec5a-109">属性</span><span class="sxs-lookup"><span data-stu-id="eec5a-109">Property</span></span>|<span data-ttu-id="eec5a-110">类型</span><span class="sxs-lookup"><span data-stu-id="eec5a-110">Type</span></span>|<span data-ttu-id="eec5a-111">说明</span><span class="sxs-lookup"><span data-stu-id="eec5a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eec5a-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="eec5a-112">lowerAddress</span></span>|<span data-ttu-id="eec5a-113">String</span><span class="sxs-lookup"><span data-stu-id="eec5a-113">String</span></span>|<span data-ttu-id="eec5a-114">较低的地址。</span><span class="sxs-lookup"><span data-stu-id="eec5a-114">Lower address.</span></span>|
|<span data-ttu-id="eec5a-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="eec5a-115">upperAddress</span></span>|<span data-ttu-id="eec5a-116">String</span><span class="sxs-lookup"><span data-stu-id="eec5a-116">String</span></span>|<span data-ttu-id="eec5a-117">地址上限。</span><span class="sxs-lookup"><span data-stu-id="eec5a-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eec5a-118">关系</span><span class="sxs-lookup"><span data-stu-id="eec5a-118">Relationships</span></span>
<span data-ttu-id="eec5a-119">无</span><span class="sxs-lookup"><span data-stu-id="eec5a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eec5a-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eec5a-120">JSON Representation</span></span>
<span data-ttu-id="eec5a-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eec5a-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```




