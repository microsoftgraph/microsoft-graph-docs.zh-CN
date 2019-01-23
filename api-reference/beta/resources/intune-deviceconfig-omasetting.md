---
title: omaSetting 资源类型
description: OMA 设置定义。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fdf74ba7e8932ce06bca83d88336239c2abcacf4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411034"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="bb667-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb667-103">omaSetting resource type</span></span>

> <span data-ttu-id="bb667-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="bb667-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bb667-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bb667-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb667-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb667-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb667-107">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="bb667-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="bb667-108">属性</span><span class="sxs-lookup"><span data-stu-id="bb667-108">Properties</span></span>
|<span data-ttu-id="bb667-109">属性</span><span class="sxs-lookup"><span data-stu-id="bb667-109">Property</span></span>|<span data-ttu-id="bb667-110">类型</span><span class="sxs-lookup"><span data-stu-id="bb667-110">Type</span></span>|<span data-ttu-id="bb667-111">说明</span><span class="sxs-lookup"><span data-stu-id="bb667-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb667-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bb667-112">displayName</span></span>|<span data-ttu-id="bb667-113">String</span><span class="sxs-lookup"><span data-stu-id="bb667-113">String</span></span>|<span data-ttu-id="bb667-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="bb667-114">Display Name.</span></span>|
|<span data-ttu-id="bb667-115">description</span><span class="sxs-lookup"><span data-stu-id="bb667-115">description</span></span>|<span data-ttu-id="bb667-116">String</span><span class="sxs-lookup"><span data-stu-id="bb667-116">String</span></span>|<span data-ttu-id="bb667-117">说明。</span><span class="sxs-lookup"><span data-stu-id="bb667-117">Description.</span></span>|
|<span data-ttu-id="bb667-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="bb667-118">omaUri</span></span>|<span data-ttu-id="bb667-119">String</span><span class="sxs-lookup"><span data-stu-id="bb667-119">String</span></span>|<span data-ttu-id="bb667-120">OMA。</span><span class="sxs-lookup"><span data-stu-id="bb667-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb667-121">关系</span><span class="sxs-lookup"><span data-stu-id="bb667-121">Relationships</span></span>
<span data-ttu-id="bb667-122">无</span><span class="sxs-lookup"><span data-stu-id="bb667-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb667-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb667-123">JSON Representation</span></span>
<span data-ttu-id="bb667-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb667-124">Here is a JSON representation of the resource.</span></span>
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




