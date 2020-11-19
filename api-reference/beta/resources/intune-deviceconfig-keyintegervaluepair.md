---
title: keyIntegerValuePair 资源类型
description: 带有字符串键和整数值的键-值对。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8cdc38003e1c16c91b1ff734e74e1c7bd6fee18
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269173"
---
# <a name="keyintegervaluepair-resource-type"></a><span data-ttu-id="95a3a-103">keyIntegerValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="95a3a-103">keyIntegerValuePair resource type</span></span>

<span data-ttu-id="95a3a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95a3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95a3a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95a3a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95a3a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95a3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95a3a-107">带有字符串键和整数值的键-值对。</span><span class="sxs-lookup"><span data-stu-id="95a3a-107">A key-value pair with a string key and an integer value.</span></span>


<span data-ttu-id="95a3a-108">继承自 [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="95a3a-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="95a3a-109">属性</span><span class="sxs-lookup"><span data-stu-id="95a3a-109">Properties</span></span>
|<span data-ttu-id="95a3a-110">属性</span><span class="sxs-lookup"><span data-stu-id="95a3a-110">Property</span></span>|<span data-ttu-id="95a3a-111">类型</span><span class="sxs-lookup"><span data-stu-id="95a3a-111">Type</span></span>|<span data-ttu-id="95a3a-112">说明</span><span class="sxs-lookup"><span data-stu-id="95a3a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95a3a-113">Key</span><span class="sxs-lookup"><span data-stu-id="95a3a-113">key</span></span>|<span data-ttu-id="95a3a-114">字符串</span><span class="sxs-lookup"><span data-stu-id="95a3a-114">String</span></span>|<span data-ttu-id="95a3a-115">键/值对的字符串键。</span><span class="sxs-lookup"><span data-stu-id="95a3a-115">The string key of the key-value pair.</span></span> <span data-ttu-id="95a3a-116">继承自 [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="95a3a-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="95a3a-117">值</span><span class="sxs-lookup"><span data-stu-id="95a3a-117">value</span></span>|<span data-ttu-id="95a3a-118">Int32</span><span class="sxs-lookup"><span data-stu-id="95a3a-118">Int32</span></span>|<span data-ttu-id="95a3a-119">键/值对的整数值。</span><span class="sxs-lookup"><span data-stu-id="95a3a-119">The integer value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95a3a-120">关系</span><span class="sxs-lookup"><span data-stu-id="95a3a-120">Relationships</span></span>
<span data-ttu-id="95a3a-121">无</span><span class="sxs-lookup"><span data-stu-id="95a3a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95a3a-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95a3a-122">JSON Representation</span></span>
<span data-ttu-id="95a3a-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95a3a-123">Here is a JSON representation of the resource.</span></span>
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




