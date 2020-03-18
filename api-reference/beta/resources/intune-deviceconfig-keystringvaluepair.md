---
title: keyStringValuePair 资源类型
description: 带有字符串键和字符串值的键-值对。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 029ebbe04532b729b49115fd51cdbcf4ea22a6a3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790403"
---
# <a name="keystringvaluepair-resource-type"></a><span data-ttu-id="46d97-103">keyStringValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="46d97-103">keyStringValuePair resource type</span></span>

> <span data-ttu-id="46d97-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="46d97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46d97-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="46d97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46d97-106">带有字符串键和字符串值的键-值对。</span><span class="sxs-lookup"><span data-stu-id="46d97-106">A key-value pair with a string key and a string value.</span></span>


<span data-ttu-id="46d97-107">继承自[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="46d97-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="46d97-108">属性</span><span class="sxs-lookup"><span data-stu-id="46d97-108">Properties</span></span>
|<span data-ttu-id="46d97-109">属性</span><span class="sxs-lookup"><span data-stu-id="46d97-109">Property</span></span>|<span data-ttu-id="46d97-110">类型</span><span class="sxs-lookup"><span data-stu-id="46d97-110">Type</span></span>|<span data-ttu-id="46d97-111">说明</span><span class="sxs-lookup"><span data-stu-id="46d97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46d97-112">Key</span><span class="sxs-lookup"><span data-stu-id="46d97-112">key</span></span>|<span data-ttu-id="46d97-113">String</span><span class="sxs-lookup"><span data-stu-id="46d97-113">String</span></span>|<span data-ttu-id="46d97-114">键/值对的字符串键。</span><span class="sxs-lookup"><span data-stu-id="46d97-114">The string key of the key-value pair.</span></span> <span data-ttu-id="46d97-115">继承自[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="46d97-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="46d97-116">value</span><span class="sxs-lookup"><span data-stu-id="46d97-116">value</span></span>|<span data-ttu-id="46d97-117">String</span><span class="sxs-lookup"><span data-stu-id="46d97-117">String</span></span>|<span data-ttu-id="46d97-118">键/值对的字符串值。</span><span class="sxs-lookup"><span data-stu-id="46d97-118">The string value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46d97-119">关系</span><span class="sxs-lookup"><span data-stu-id="46d97-119">Relationships</span></span>
<span data-ttu-id="46d97-120">无</span><span class="sxs-lookup"><span data-stu-id="46d97-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46d97-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="46d97-121">JSON Representation</span></span>
<span data-ttu-id="46d97-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46d97-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyStringValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyStringValuePair",
  "key": "String",
  "value": "String"
}
```



