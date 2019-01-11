---
title: iPv6Range 资源类型
description: IPV6 范围
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 84d925cc7885dab4b3e87dbd62060894e741f52c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845743"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="34409-103">iPv6Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="34409-103">iPv6Range resource type</span></span>

> <span data-ttu-id="34409-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="34409-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34409-105">IPV6 范围</span><span class="sxs-lookup"><span data-stu-id="34409-105">IP V6 range</span></span>

<span data-ttu-id="34409-106">继承自 [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="34409-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34409-107">属性</span><span class="sxs-lookup"><span data-stu-id="34409-107">Properties</span></span>
|<span data-ttu-id="34409-108">属性</span><span class="sxs-lookup"><span data-stu-id="34409-108">Property</span></span>|<span data-ttu-id="34409-109">类型</span><span class="sxs-lookup"><span data-stu-id="34409-109">Type</span></span>|<span data-ttu-id="34409-110">说明</span><span class="sxs-lookup"><span data-stu-id="34409-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34409-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="34409-111">lowerAddress</span></span>|<span data-ttu-id="34409-112">String</span><span class="sxs-lookup"><span data-stu-id="34409-112">String</span></span>|<span data-ttu-id="34409-113">IP 地址下限</span><span class="sxs-lookup"><span data-stu-id="34409-113">Lower IP Address</span></span>|
|<span data-ttu-id="34409-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="34409-114">upperAddress</span></span>|<span data-ttu-id="34409-115">String</span><span class="sxs-lookup"><span data-stu-id="34409-115">String</span></span>|<span data-ttu-id="34409-116">IP 地址上限</span><span class="sxs-lookup"><span data-stu-id="34409-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="34409-117">关系</span><span class="sxs-lookup"><span data-stu-id="34409-117">Relationships</span></span>
<span data-ttu-id="34409-118">无</span><span class="sxs-lookup"><span data-stu-id="34409-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="34409-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34409-119">JSON Representation</span></span>
<span data-ttu-id="34409-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34409-120">Here is a JSON representation of the resource.</span></span>
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



