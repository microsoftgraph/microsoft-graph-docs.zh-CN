---
title: keyBooleanValuePair 资源类型
description: 带有字符串键和布尔值的键-值对。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0d034eea836ed59eecfa712b80d5cadcbb01ea12
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269208"
---
# <a name="keybooleanvaluepair-resource-type"></a><span data-ttu-id="912a1-103">keyBooleanValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="912a1-103">keyBooleanValuePair resource type</span></span>

<span data-ttu-id="912a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="912a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="912a1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="912a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="912a1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="912a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="912a1-107">带有字符串键和布尔值的键-值对。</span><span class="sxs-lookup"><span data-stu-id="912a1-107">A key-value pair with a string key and a Boolean value.</span></span>


<span data-ttu-id="912a1-108">继承自 [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="912a1-108">Inherits from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="912a1-109">属性</span><span class="sxs-lookup"><span data-stu-id="912a1-109">Properties</span></span>
|<span data-ttu-id="912a1-110">属性</span><span class="sxs-lookup"><span data-stu-id="912a1-110">Property</span></span>|<span data-ttu-id="912a1-111">类型</span><span class="sxs-lookup"><span data-stu-id="912a1-111">Type</span></span>|<span data-ttu-id="912a1-112">说明</span><span class="sxs-lookup"><span data-stu-id="912a1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="912a1-113">Key</span><span class="sxs-lookup"><span data-stu-id="912a1-113">key</span></span>|<span data-ttu-id="912a1-114">字符串</span><span class="sxs-lookup"><span data-stu-id="912a1-114">String</span></span>|<span data-ttu-id="912a1-115">键/值对的字符串键。</span><span class="sxs-lookup"><span data-stu-id="912a1-115">The string key of the key-value pair.</span></span> <span data-ttu-id="912a1-116">继承自 [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="912a1-116">Inherited from [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="912a1-117">value</span><span class="sxs-lookup"><span data-stu-id="912a1-117">value</span></span>|<span data-ttu-id="912a1-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="912a1-118">Boolean</span></span>|<span data-ttu-id="912a1-119">键/值对的布尔值。</span><span class="sxs-lookup"><span data-stu-id="912a1-119">The Boolean value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="912a1-120">关系</span><span class="sxs-lookup"><span data-stu-id="912a1-120">Relationships</span></span>
<span data-ttu-id="912a1-121">无</span><span class="sxs-lookup"><span data-stu-id="912a1-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="912a1-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="912a1-122">JSON Representation</span></span>
<span data-ttu-id="912a1-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="912a1-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyBooleanValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyBooleanValuePair",
  "key": "String",
  "value": true
}
```




