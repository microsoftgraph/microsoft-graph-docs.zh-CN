---
title: keyIntegerValuePair 资源类型
description: 带有字符串键和整数值的键-值对。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0cd9c4de9f7c2505b12eada575ebc5d869480758
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37200012"
---
# <a name="keyintegervaluepair-resource-type"></a><span data-ttu-id="f8ccf-103">keyIntegerValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8ccf-103">keyIntegerValuePair resource type</span></span>

> <span data-ttu-id="f8ccf-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f8ccf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8ccf-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f8ccf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8ccf-106">带有字符串键和整数值的键-值对。</span><span class="sxs-lookup"><span data-stu-id="f8ccf-106">A key-value pair with a string key and an integer value.</span></span>


<span data-ttu-id="f8ccf-107">继承自[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f8ccf-107">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f8ccf-108">属性</span><span class="sxs-lookup"><span data-stu-id="f8ccf-108">Properties</span></span>
|<span data-ttu-id="f8ccf-109">属性</span><span class="sxs-lookup"><span data-stu-id="f8ccf-109">Property</span></span>|<span data-ttu-id="f8ccf-110">类型</span><span class="sxs-lookup"><span data-stu-id="f8ccf-110">Type</span></span>|<span data-ttu-id="f8ccf-111">说明</span><span class="sxs-lookup"><span data-stu-id="f8ccf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8ccf-112">Key</span><span class="sxs-lookup"><span data-stu-id="f8ccf-112">key</span></span>|<span data-ttu-id="f8ccf-113">String</span><span class="sxs-lookup"><span data-stu-id="f8ccf-113">String</span></span>|<span data-ttu-id="f8ccf-114">键/值对的字符串键。</span><span class="sxs-lookup"><span data-stu-id="f8ccf-114">The string key of the key-value pair.</span></span> <span data-ttu-id="f8ccf-115">继承自[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f8ccf-115">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="f8ccf-116">值</span><span class="sxs-lookup"><span data-stu-id="f8ccf-116">value</span></span>|<span data-ttu-id="f8ccf-117">Int32</span><span class="sxs-lookup"><span data-stu-id="f8ccf-117">Int32</span></span>|<span data-ttu-id="f8ccf-118">键/值对的整数值。</span><span class="sxs-lookup"><span data-stu-id="f8ccf-118">The integer value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8ccf-119">关系</span><span class="sxs-lookup"><span data-stu-id="f8ccf-119">Relationships</span></span>
<span data-ttu-id="f8ccf-120">无</span><span class="sxs-lookup"><span data-stu-id="f8ccf-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8ccf-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8ccf-121">JSON Representation</span></span>
<span data-ttu-id="f8ccf-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8ccf-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyIntegerValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyIntegerValuePair",
  "key": "String",
  "value": 1024
}
```



