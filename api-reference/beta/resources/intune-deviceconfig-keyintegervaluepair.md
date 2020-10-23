---
title: keyIntegerValuePair 资源类型
description: 带有字符串键和整数值的键-值对。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c0f9a3f05982daa036b1a2f38a09cb34011a3fb9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730458"
---
# <a name="keyintegervaluepair-resource-type"></a><span data-ttu-id="9d5b9-103">keyIntegerValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d5b9-103">keyIntegerValuePair resource type</span></span>

<span data-ttu-id="9d5b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d5b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d5b9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9d5b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d5b9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9d5b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d5b9-107">带有字符串键和整数值的键-值对。</span><span class="sxs-lookup"><span data-stu-id="9d5b9-107">A key-value pair with a string key and an integer value.</span></span>


<span data-ttu-id="9d5b9-108">继承自 [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9d5b9-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9d5b9-109">属性</span><span class="sxs-lookup"><span data-stu-id="9d5b9-109">Properties</span></span>
|<span data-ttu-id="9d5b9-110">属性</span><span class="sxs-lookup"><span data-stu-id="9d5b9-110">Property</span></span>|<span data-ttu-id="9d5b9-111">类型</span><span class="sxs-lookup"><span data-stu-id="9d5b9-111">Type</span></span>|<span data-ttu-id="9d5b9-112">说明</span><span class="sxs-lookup"><span data-stu-id="9d5b9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d5b9-113">Key</span><span class="sxs-lookup"><span data-stu-id="9d5b9-113">key</span></span>|<span data-ttu-id="9d5b9-114">String</span><span class="sxs-lookup"><span data-stu-id="9d5b9-114">String</span></span>|<span data-ttu-id="9d5b9-115">键/值对的字符串键。</span><span class="sxs-lookup"><span data-stu-id="9d5b9-115">The string key of the key-value pair.</span></span> <span data-ttu-id="9d5b9-116">继承自 [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9d5b9-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="9d5b9-117">值</span><span class="sxs-lookup"><span data-stu-id="9d5b9-117">value</span></span>|<span data-ttu-id="9d5b9-118">Int32</span><span class="sxs-lookup"><span data-stu-id="9d5b9-118">Int32</span></span>|<span data-ttu-id="9d5b9-119">键/值对的整数值。</span><span class="sxs-lookup"><span data-stu-id="9d5b9-119">The integer value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d5b9-120">关系</span><span class="sxs-lookup"><span data-stu-id="9d5b9-120">Relationships</span></span>
<span data-ttu-id="9d5b9-121">无</span><span class="sxs-lookup"><span data-stu-id="9d5b9-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d5b9-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d5b9-122">JSON Representation</span></span>
<span data-ttu-id="9d5b9-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d5b9-123">Here is a JSON representation of the resource.</span></span>
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





