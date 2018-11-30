---
title: iPv6Range 资源类型
description: IPV6 范围
ms.openlocfilehash: c2f17529b589fc2d7837f6a8f539ff64d5d82dd9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011647"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="a5fce-103">iPv6Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5fce-103">iPv6Range resource type</span></span>

> <span data-ttu-id="a5fce-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a5fce-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5fce-105">IPV6 范围</span><span class="sxs-lookup"><span data-stu-id="a5fce-105">IP V6 range</span></span>

<span data-ttu-id="a5fce-106">继承自 [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="a5fce-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a5fce-107">属性</span><span class="sxs-lookup"><span data-stu-id="a5fce-107">Properties</span></span>
|<span data-ttu-id="a5fce-108">属性</span><span class="sxs-lookup"><span data-stu-id="a5fce-108">Property</span></span>|<span data-ttu-id="a5fce-109">类型</span><span class="sxs-lookup"><span data-stu-id="a5fce-109">Type</span></span>|<span data-ttu-id="a5fce-110">说明</span><span class="sxs-lookup"><span data-stu-id="a5fce-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5fce-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="a5fce-111">lowerAddress</span></span>|<span data-ttu-id="a5fce-112">String</span><span class="sxs-lookup"><span data-stu-id="a5fce-112">String</span></span>|<span data-ttu-id="a5fce-113">IP 地址下限</span><span class="sxs-lookup"><span data-stu-id="a5fce-113">Lower IP Address</span></span>|
|<span data-ttu-id="a5fce-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="a5fce-114">upperAddress</span></span>|<span data-ttu-id="a5fce-115">String</span><span class="sxs-lookup"><span data-stu-id="a5fce-115">String</span></span>|<span data-ttu-id="a5fce-116">IP 地址上限</span><span class="sxs-lookup"><span data-stu-id="a5fce-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5fce-117">关系</span><span class="sxs-lookup"><span data-stu-id="a5fce-117">Relationships</span></span>
<span data-ttu-id="a5fce-118">无</span><span class="sxs-lookup"><span data-stu-id="a5fce-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a5fce-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5fce-119">JSON Representation</span></span>
<span data-ttu-id="a5fce-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5fce-120">Here is a JSON representation of the resource.</span></span>
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



