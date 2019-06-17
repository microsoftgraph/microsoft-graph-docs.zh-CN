---
title: 键值资源类型
description: 项值定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c8e8028a4863ee313499f8c4982b569ca25747b3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989376"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="bda74-103">键值资源类型</span><span class="sxs-lookup"><span data-stu-id="bda74-103">keyValue resource type</span></span>

> <span data-ttu-id="bda74-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bda74-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bda74-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bda74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bda74-106">项值定义。</span><span class="sxs-lookup"><span data-stu-id="bda74-106">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="bda74-107">属性</span><span class="sxs-lookup"><span data-stu-id="bda74-107">Properties</span></span>
|<span data-ttu-id="bda74-108">属性</span><span class="sxs-lookup"><span data-stu-id="bda74-108">Property</span></span>|<span data-ttu-id="bda74-109">类型</span><span class="sxs-lookup"><span data-stu-id="bda74-109">Type</span></span>|<span data-ttu-id="bda74-110">说明</span><span class="sxs-lookup"><span data-stu-id="bda74-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bda74-111">Key</span><span class="sxs-lookup"><span data-stu-id="bda74-111">key</span></span>|<span data-ttu-id="bda74-112">String</span><span class="sxs-lookup"><span data-stu-id="bda74-112">String</span></span>|<span data-ttu-id="bda74-113">键。</span><span class="sxs-lookup"><span data-stu-id="bda74-113">Key.</span></span>|
|<span data-ttu-id="bda74-114">value</span><span class="sxs-lookup"><span data-stu-id="bda74-114">value</span></span>|<span data-ttu-id="bda74-115">String</span><span class="sxs-lookup"><span data-stu-id="bda74-115">String</span></span>|<span data-ttu-id="bda74-116">值。</span><span class="sxs-lookup"><span data-stu-id="bda74-116">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bda74-117">关系</span><span class="sxs-lookup"><span data-stu-id="bda74-117">Relationships</span></span>
<span data-ttu-id="bda74-118">无</span><span class="sxs-lookup"><span data-stu-id="bda74-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bda74-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bda74-119">JSON Representation</span></span>
<span data-ttu-id="bda74-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bda74-120">Here is a JSON representation of the resource.</span></span>
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





