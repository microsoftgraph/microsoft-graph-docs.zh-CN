---
title: omaSetting 资源类型
description: OMA 设置定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f53e50bdf3584ab7f34afedbd938ad0749eb23b6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788483"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="753d4-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="753d4-103">omaSetting resource type</span></span>

> <span data-ttu-id="753d4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="753d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="753d4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="753d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="753d4-106">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="753d4-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="753d4-107">属性</span><span class="sxs-lookup"><span data-stu-id="753d4-107">Properties</span></span>
|<span data-ttu-id="753d4-108">属性</span><span class="sxs-lookup"><span data-stu-id="753d4-108">Property</span></span>|<span data-ttu-id="753d4-109">类型</span><span class="sxs-lookup"><span data-stu-id="753d4-109">Type</span></span>|<span data-ttu-id="753d4-110">说明</span><span class="sxs-lookup"><span data-stu-id="753d4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="753d4-111">displayName</span><span class="sxs-lookup"><span data-stu-id="753d4-111">displayName</span></span>|<span data-ttu-id="753d4-112">字符串</span><span class="sxs-lookup"><span data-stu-id="753d4-112">String</span></span>|<span data-ttu-id="753d4-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="753d4-113">Display Name.</span></span>|
|<span data-ttu-id="753d4-114">说明</span><span class="sxs-lookup"><span data-stu-id="753d4-114">description</span></span>|<span data-ttu-id="753d4-115">String</span><span class="sxs-lookup"><span data-stu-id="753d4-115">String</span></span>|<span data-ttu-id="753d4-116">说明。</span><span class="sxs-lookup"><span data-stu-id="753d4-116">Description.</span></span>|
|<span data-ttu-id="753d4-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="753d4-117">omaUri</span></span>|<span data-ttu-id="753d4-118">String</span><span class="sxs-lookup"><span data-stu-id="753d4-118">String</span></span>|<span data-ttu-id="753d4-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="753d4-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="753d4-120">关系</span><span class="sxs-lookup"><span data-stu-id="753d4-120">Relationships</span></span>
<span data-ttu-id="753d4-121">无</span><span class="sxs-lookup"><span data-stu-id="753d4-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="753d4-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="753d4-122">JSON Representation</span></span>
<span data-ttu-id="753d4-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="753d4-123">Here is a JSON representation of the resource.</span></span>
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



