---
title: iPv6Range 资源类型
description: IPv6 范围定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 383d75ceafd1946d317cc3ee146f39a0433accd0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255831"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="046c0-103">iPv6Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="046c0-103">iPv6Range resource type</span></span>

<span data-ttu-id="046c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="046c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="046c0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="046c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="046c0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="046c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="046c0-107">IPv6 范围定义。</span><span class="sxs-lookup"><span data-stu-id="046c0-107">IPv6 Range definition.</span></span>


<span data-ttu-id="046c0-108">继承自 [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="046c0-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="046c0-109">属性</span><span class="sxs-lookup"><span data-stu-id="046c0-109">Properties</span></span>
|<span data-ttu-id="046c0-110">属性</span><span class="sxs-lookup"><span data-stu-id="046c0-110">Property</span></span>|<span data-ttu-id="046c0-111">类型</span><span class="sxs-lookup"><span data-stu-id="046c0-111">Type</span></span>|<span data-ttu-id="046c0-112">描述</span><span class="sxs-lookup"><span data-stu-id="046c0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="046c0-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="046c0-113">lowerAddress</span></span>|<span data-ttu-id="046c0-114">String</span><span class="sxs-lookup"><span data-stu-id="046c0-114">String</span></span>|<span data-ttu-id="046c0-115">较低的地址。</span><span class="sxs-lookup"><span data-stu-id="046c0-115">Lower address.</span></span>|
|<span data-ttu-id="046c0-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="046c0-116">upperAddress</span></span>|<span data-ttu-id="046c0-117">String</span><span class="sxs-lookup"><span data-stu-id="046c0-117">String</span></span>|<span data-ttu-id="046c0-118">地址上限。</span><span class="sxs-lookup"><span data-stu-id="046c0-118">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="046c0-119">关系</span><span class="sxs-lookup"><span data-stu-id="046c0-119">Relationships</span></span>
<span data-ttu-id="046c0-120">无</span><span class="sxs-lookup"><span data-stu-id="046c0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="046c0-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="046c0-121">JSON Representation</span></span>
<span data-ttu-id="046c0-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="046c0-122">Here is a JSON representation of the resource.</span></span>
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




