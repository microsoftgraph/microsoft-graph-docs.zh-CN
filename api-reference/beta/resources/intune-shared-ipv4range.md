---
title: iPv4Range 资源类型
description: IP V4 范围
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a1f76fcd99663fe7ddd34263c8304b5597e6941c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888289"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="db505-103">iPv4Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="db505-103">iPv4Range resource type</span></span>

> <span data-ttu-id="db505-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="db505-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db505-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="db505-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db505-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="db505-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db505-107">IP V4 范围</span><span class="sxs-lookup"><span data-stu-id="db505-107">IP V4 range</span></span>

<span data-ttu-id="db505-108">继承自 [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="db505-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="db505-109">属性</span><span class="sxs-lookup"><span data-stu-id="db505-109">Properties</span></span>
|<span data-ttu-id="db505-110">属性</span><span class="sxs-lookup"><span data-stu-id="db505-110">Property</span></span>|<span data-ttu-id="db505-111">类型</span><span class="sxs-lookup"><span data-stu-id="db505-111">Type</span></span>|<span data-ttu-id="db505-112">说明</span><span class="sxs-lookup"><span data-stu-id="db505-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db505-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="db505-113">lowerAddress</span></span>|<span data-ttu-id="db505-114">String</span><span class="sxs-lookup"><span data-stu-id="db505-114">String</span></span>|<span data-ttu-id="db505-115">IP 地址下限</span><span class="sxs-lookup"><span data-stu-id="db505-115">Lower IP Address</span></span>|
|<span data-ttu-id="db505-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="db505-116">upperAddress</span></span>|<span data-ttu-id="db505-117">String</span><span class="sxs-lookup"><span data-stu-id="db505-117">String</span></span>|<span data-ttu-id="db505-118">IP 地址上限</span><span class="sxs-lookup"><span data-stu-id="db505-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="db505-119">关系</span><span class="sxs-lookup"><span data-stu-id="db505-119">Relationships</span></span>
<span data-ttu-id="db505-120">无</span><span class="sxs-lookup"><span data-stu-id="db505-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db505-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db505-121">JSON Representation</span></span>
<span data-ttu-id="db505-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db505-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



