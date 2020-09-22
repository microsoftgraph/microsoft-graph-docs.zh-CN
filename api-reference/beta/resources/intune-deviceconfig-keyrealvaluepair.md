---
title: keyRealValuePair 资源类型
description: 具有字符串键和实际 (浮点) 值的键/值对。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3ccc5d8c675bd9971d95b8ae3bfd5ac0cc01a87
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092529"
---
# <a name="keyrealvaluepair-resource-type"></a><span data-ttu-id="b3efb-103">keyRealValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3efb-103">keyRealValuePair resource type</span></span>

<span data-ttu-id="b3efb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3efb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3efb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b3efb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3efb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3efb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3efb-107">具有字符串键和实际 (浮点) 值的键/值对。</span><span class="sxs-lookup"><span data-stu-id="b3efb-107">A key-value pair with a string key and a real (floating-point) value.</span></span>


<span data-ttu-id="b3efb-108">继承自 [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b3efb-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b3efb-109">属性</span><span class="sxs-lookup"><span data-stu-id="b3efb-109">Properties</span></span>
|<span data-ttu-id="b3efb-110">属性</span><span class="sxs-lookup"><span data-stu-id="b3efb-110">Property</span></span>|<span data-ttu-id="b3efb-111">类型</span><span class="sxs-lookup"><span data-stu-id="b3efb-111">Type</span></span>|<span data-ttu-id="b3efb-112">说明</span><span class="sxs-lookup"><span data-stu-id="b3efb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3efb-113">Key</span><span class="sxs-lookup"><span data-stu-id="b3efb-113">key</span></span>|<span data-ttu-id="b3efb-114">字符串</span><span class="sxs-lookup"><span data-stu-id="b3efb-114">String</span></span>|<span data-ttu-id="b3efb-115">键/值对的字符串键。</span><span class="sxs-lookup"><span data-stu-id="b3efb-115">The string key of the key-value pair.</span></span> <span data-ttu-id="b3efb-116">继承自 [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b3efb-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="b3efb-117">值</span><span class="sxs-lookup"><span data-stu-id="b3efb-117">value</span></span>|<span data-ttu-id="b3efb-118">双精度</span><span class="sxs-lookup"><span data-stu-id="b3efb-118">Double</span></span>|<span data-ttu-id="b3efb-119">实际 (的键值对的浮点) 值。</span><span class="sxs-lookup"><span data-stu-id="b3efb-119">The real (floating-point) value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3efb-120">关系</span><span class="sxs-lookup"><span data-stu-id="b3efb-120">Relationships</span></span>
<span data-ttu-id="b3efb-121">无</span><span class="sxs-lookup"><span data-stu-id="b3efb-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3efb-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3efb-122">JSON Representation</span></span>
<span data-ttu-id="b3efb-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3efb-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyRealValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyRealValuePair",
  "key": "String",
  "value": "4.2"
}
```






