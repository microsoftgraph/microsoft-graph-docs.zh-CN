---
title: keyRealValuePair 资源类型
description: 带有字符串键和实际（浮点）值的键/值对。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6b90c7faa0bb3ffabe5b057d03503745801af8c8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790424"
---
# <a name="keyrealvaluepair-resource-type"></a><span data-ttu-id="a4918-103">keyRealValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4918-103">keyRealValuePair resource type</span></span>

> <span data-ttu-id="a4918-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a4918-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4918-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4918-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4918-106">带有字符串键和实际（浮点）值的键/值对。</span><span class="sxs-lookup"><span data-stu-id="a4918-106">A key-value pair with a string key and a real (floating-point) value.</span></span>


<span data-ttu-id="a4918-107">继承自[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="a4918-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a4918-108">属性</span><span class="sxs-lookup"><span data-stu-id="a4918-108">Properties</span></span>
|<span data-ttu-id="a4918-109">属性</span><span class="sxs-lookup"><span data-stu-id="a4918-109">Property</span></span>|<span data-ttu-id="a4918-110">类型</span><span class="sxs-lookup"><span data-stu-id="a4918-110">Type</span></span>|<span data-ttu-id="a4918-111">说明</span><span class="sxs-lookup"><span data-stu-id="a4918-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4918-112">Key</span><span class="sxs-lookup"><span data-stu-id="a4918-112">key</span></span>|<span data-ttu-id="a4918-113">String</span><span class="sxs-lookup"><span data-stu-id="a4918-113">String</span></span>|<span data-ttu-id="a4918-114">键/值对的字符串键。</span><span class="sxs-lookup"><span data-stu-id="a4918-114">The string key of the key-value pair.</span></span> <span data-ttu-id="a4918-115">继承自[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="a4918-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="a4918-116">值</span><span class="sxs-lookup"><span data-stu-id="a4918-116">value</span></span>|<span data-ttu-id="a4918-117">双精度</span><span class="sxs-lookup"><span data-stu-id="a4918-117">Double</span></span>|<span data-ttu-id="a4918-118">键/值对的实际（浮点）值。</span><span class="sxs-lookup"><span data-stu-id="a4918-118">The real (floating-point) value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4918-119">关系</span><span class="sxs-lookup"><span data-stu-id="a4918-119">Relationships</span></span>
<span data-ttu-id="a4918-120">无</span><span class="sxs-lookup"><span data-stu-id="a4918-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4918-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4918-121">JSON Representation</span></span>
<span data-ttu-id="a4918-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4918-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyRealValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyRealValuePair",
  "key": "String",
  "value": "<Unknown Primitive Type Edm.Double>"
}
```



