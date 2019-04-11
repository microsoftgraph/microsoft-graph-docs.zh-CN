---
title: omaSetting 资源类型
description: OMA 设置定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d4c232f346e9966c72bcd60e0fd08af139db068
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783225"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="c8969-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8969-103">omaSetting resource type</span></span>

> <span data-ttu-id="c8969-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c8969-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8969-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c8969-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8969-106">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="c8969-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="c8969-107">属性</span><span class="sxs-lookup"><span data-stu-id="c8969-107">Properties</span></span>
|<span data-ttu-id="c8969-108">属性</span><span class="sxs-lookup"><span data-stu-id="c8969-108">Property</span></span>|<span data-ttu-id="c8969-109">类型</span><span class="sxs-lookup"><span data-stu-id="c8969-109">Type</span></span>|<span data-ttu-id="c8969-110">说明</span><span class="sxs-lookup"><span data-stu-id="c8969-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8969-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c8969-111">displayName</span></span>|<span data-ttu-id="c8969-112">字符串</span><span class="sxs-lookup"><span data-stu-id="c8969-112">String</span></span>|<span data-ttu-id="c8969-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="c8969-113">Display Name.</span></span>|
|<span data-ttu-id="c8969-114">description</span><span class="sxs-lookup"><span data-stu-id="c8969-114">description</span></span>|<span data-ttu-id="c8969-115">String</span><span class="sxs-lookup"><span data-stu-id="c8969-115">String</span></span>|<span data-ttu-id="c8969-116">说明。</span><span class="sxs-lookup"><span data-stu-id="c8969-116">Description.</span></span>|
|<span data-ttu-id="c8969-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="c8969-117">omaUri</span></span>|<span data-ttu-id="c8969-118">String</span><span class="sxs-lookup"><span data-stu-id="c8969-118">String</span></span>|<span data-ttu-id="c8969-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="c8969-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8969-120">关系</span><span class="sxs-lookup"><span data-stu-id="c8969-120">Relationships</span></span>
<span data-ttu-id="c8969-121">无</span><span class="sxs-lookup"><span data-stu-id="c8969-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8969-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8969-122">JSON Representation</span></span>
<span data-ttu-id="c8969-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8969-123">Here is a JSON representation of the resource.</span></span>
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





