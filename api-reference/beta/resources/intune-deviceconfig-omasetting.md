---
title: omaSetting 资源类型
description: OMA 设置定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bb5df5f786eefc1b7b7159b1643f9d3d46d8300
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958702"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="9b0e5-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b0e5-103">omaSetting resource type</span></span>

> <span data-ttu-id="9b0e5-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b0e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b0e5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b0e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b0e5-106">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="9b0e5-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="9b0e5-107">属性</span><span class="sxs-lookup"><span data-stu-id="9b0e5-107">Properties</span></span>
|<span data-ttu-id="9b0e5-108">属性</span><span class="sxs-lookup"><span data-stu-id="9b0e5-108">Property</span></span>|<span data-ttu-id="9b0e5-109">类型</span><span class="sxs-lookup"><span data-stu-id="9b0e5-109">Type</span></span>|<span data-ttu-id="9b0e5-110">说明</span><span class="sxs-lookup"><span data-stu-id="9b0e5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b0e5-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9b0e5-111">displayName</span></span>|<span data-ttu-id="9b0e5-112">字符串</span><span class="sxs-lookup"><span data-stu-id="9b0e5-112">String</span></span>|<span data-ttu-id="9b0e5-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="9b0e5-113">Display Name.</span></span>|
|<span data-ttu-id="9b0e5-114">说明</span><span class="sxs-lookup"><span data-stu-id="9b0e5-114">description</span></span>|<span data-ttu-id="9b0e5-115">String</span><span class="sxs-lookup"><span data-stu-id="9b0e5-115">String</span></span>|<span data-ttu-id="9b0e5-116">说明。</span><span class="sxs-lookup"><span data-stu-id="9b0e5-116">Description.</span></span>|
|<span data-ttu-id="9b0e5-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="9b0e5-117">omaUri</span></span>|<span data-ttu-id="9b0e5-118">String</span><span class="sxs-lookup"><span data-stu-id="9b0e5-118">String</span></span>|<span data-ttu-id="9b0e5-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="9b0e5-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b0e5-120">关系</span><span class="sxs-lookup"><span data-stu-id="9b0e5-120">Relationships</span></span>
<span data-ttu-id="9b0e5-121">无</span><span class="sxs-lookup"><span data-stu-id="9b0e5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b0e5-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b0e5-122">JSON Representation</span></span>
<span data-ttu-id="9b0e5-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b0e5-123">Here is a JSON representation of the resource.</span></span>
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





