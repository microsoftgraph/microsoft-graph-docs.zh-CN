---
title: omaSetting 资源类型
description: OMA 设置定义。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 86cb06b35a0f64052860c268764696a1db8459e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888380"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="6e297-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="6e297-103">omaSetting resource type</span></span>

> <span data-ttu-id="6e297-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6e297-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6e297-105">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="6e297-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="6e297-106">属性</span><span class="sxs-lookup"><span data-stu-id="6e297-106">Properties</span></span>
|<span data-ttu-id="6e297-107">属性</span><span class="sxs-lookup"><span data-stu-id="6e297-107">Property</span></span>|<span data-ttu-id="6e297-108">类型</span><span class="sxs-lookup"><span data-stu-id="6e297-108">Type</span></span>|<span data-ttu-id="6e297-109">说明</span><span class="sxs-lookup"><span data-stu-id="6e297-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e297-110">displayName</span><span class="sxs-lookup"><span data-stu-id="6e297-110">displayName</span></span>|<span data-ttu-id="6e297-111">String</span><span class="sxs-lookup"><span data-stu-id="6e297-111">String</span></span>|<span data-ttu-id="6e297-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="6e297-112">Display Name.</span></span>|
|<span data-ttu-id="6e297-113">description</span><span class="sxs-lookup"><span data-stu-id="6e297-113">description</span></span>|<span data-ttu-id="6e297-114">String</span><span class="sxs-lookup"><span data-stu-id="6e297-114">String</span></span>|<span data-ttu-id="6e297-115">说明。</span><span class="sxs-lookup"><span data-stu-id="6e297-115">Description.</span></span>|
|<span data-ttu-id="6e297-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="6e297-116">omaUri</span></span>|<span data-ttu-id="6e297-117">String</span><span class="sxs-lookup"><span data-stu-id="6e297-117">String</span></span>|<span data-ttu-id="6e297-118">OMA。</span><span class="sxs-lookup"><span data-stu-id="6e297-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e297-119">关系</span><span class="sxs-lookup"><span data-stu-id="6e297-119">Relationships</span></span>
<span data-ttu-id="6e297-120">无</span><span class="sxs-lookup"><span data-stu-id="6e297-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6e297-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6e297-121">JSON Representation</span></span>
<span data-ttu-id="6e297-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e297-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```



