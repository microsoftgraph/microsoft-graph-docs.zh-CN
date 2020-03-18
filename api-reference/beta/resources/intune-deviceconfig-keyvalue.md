---
title: 键值资源类型
description: 项值定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e875ba06ff704f01cc2fd7b7dd48c2b8cfcfba63
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790382"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="9c7d4-103">键值资源类型</span><span class="sxs-lookup"><span data-stu-id="9c7d4-103">keyValue resource type</span></span>

> <span data-ttu-id="9c7d4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c7d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c7d4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c7d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c7d4-106">项值定义。</span><span class="sxs-lookup"><span data-stu-id="9c7d4-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="9c7d4-107">属性</span><span class="sxs-lookup"><span data-stu-id="9c7d4-107">Properties</span></span>
|<span data-ttu-id="9c7d4-108">属性</span><span class="sxs-lookup"><span data-stu-id="9c7d4-108">Property</span></span>|<span data-ttu-id="9c7d4-109">类型</span><span class="sxs-lookup"><span data-stu-id="9c7d4-109">Type</span></span>|<span data-ttu-id="9c7d4-110">说明</span><span class="sxs-lookup"><span data-stu-id="9c7d4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c7d4-111">Key</span><span class="sxs-lookup"><span data-stu-id="9c7d4-111">key</span></span>|<span data-ttu-id="9c7d4-112">String</span><span class="sxs-lookup"><span data-stu-id="9c7d4-112">String</span></span>|<span data-ttu-id="9c7d4-113">键。</span><span class="sxs-lookup"><span data-stu-id="9c7d4-113">Key.</span></span>|
|<span data-ttu-id="9c7d4-114">value</span><span class="sxs-lookup"><span data-stu-id="9c7d4-114">value</span></span>|<span data-ttu-id="9c7d4-115">String</span><span class="sxs-lookup"><span data-stu-id="9c7d4-115">String</span></span>|<span data-ttu-id="9c7d4-116">值。</span><span class="sxs-lookup"><span data-stu-id="9c7d4-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c7d4-117">关系</span><span class="sxs-lookup"><span data-stu-id="9c7d4-117">Relationships</span></span>
<span data-ttu-id="9c7d4-118">无</span><span class="sxs-lookup"><span data-stu-id="9c7d4-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c7d4-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c7d4-119">JSON Representation</span></span>
<span data-ttu-id="9c7d4-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c7d4-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```



