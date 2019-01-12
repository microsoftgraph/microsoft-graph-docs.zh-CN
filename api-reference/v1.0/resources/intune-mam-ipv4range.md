---
title: iPv4Range 资源类型
description: IP V4 范围
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2c260796259ce6084add7eadb48192ea50c209c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931928"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="4cf9d-103">iPv4Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="4cf9d-103">iPv4Range resource type</span></span>

> <span data-ttu-id="4cf9d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4cf9d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cf9d-105">IP V4 范围</span><span class="sxs-lookup"><span data-stu-id="4cf9d-105">IP V4 range</span></span>

<span data-ttu-id="4cf9d-106">继承自 [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="4cf9d-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4cf9d-107">属性</span><span class="sxs-lookup"><span data-stu-id="4cf9d-107">Properties</span></span>
|<span data-ttu-id="4cf9d-108">属性</span><span class="sxs-lookup"><span data-stu-id="4cf9d-108">Property</span></span>|<span data-ttu-id="4cf9d-109">类型</span><span class="sxs-lookup"><span data-stu-id="4cf9d-109">Type</span></span>|<span data-ttu-id="4cf9d-110">说明</span><span class="sxs-lookup"><span data-stu-id="4cf9d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cf9d-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="4cf9d-111">lowerAddress</span></span>|<span data-ttu-id="4cf9d-112">String</span><span class="sxs-lookup"><span data-stu-id="4cf9d-112">String</span></span>|<span data-ttu-id="4cf9d-113">IP 地址下限</span><span class="sxs-lookup"><span data-stu-id="4cf9d-113">Lower IP Address</span></span>|
|<span data-ttu-id="4cf9d-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="4cf9d-114">upperAddress</span></span>|<span data-ttu-id="4cf9d-115">String</span><span class="sxs-lookup"><span data-stu-id="4cf9d-115">String</span></span>|<span data-ttu-id="4cf9d-116">IP 地址上限</span><span class="sxs-lookup"><span data-stu-id="4cf9d-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cf9d-117">关系</span><span class="sxs-lookup"><span data-stu-id="4cf9d-117">Relationships</span></span>
<span data-ttu-id="4cf9d-118">无</span><span class="sxs-lookup"><span data-stu-id="4cf9d-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4cf9d-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4cf9d-119">JSON Representation</span></span>
<span data-ttu-id="4cf9d-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4cf9d-120">Here is a JSON representation of the resource.</span></span>
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



