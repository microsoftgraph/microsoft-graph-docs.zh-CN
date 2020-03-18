---
title: macOSAssociatedDomainsKeyValuePair 资源类型
description: 关联域的键值对
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08a59f0566da2e2dffa64c059cc913923ec5cf58
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790319"
---
# <a name="macosassociateddomainskeyvaluepair-resource-type"></a><span data-ttu-id="0909c-103">macOSAssociatedDomainsKeyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="0909c-103">macOSAssociatedDomainsKeyValuePair resource type</span></span>

> <span data-ttu-id="0909c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0909c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0909c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0909c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0909c-106">关联域的键值对</span><span class="sxs-lookup"><span data-stu-id="0909c-106">Key value pair for associated domains</span></span>


<span data-ttu-id="0909c-107">继承自[keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="0909c-107">Inherits from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0909c-108">属性</span><span class="sxs-lookup"><span data-stu-id="0909c-108">Properties</span></span>
|<span data-ttu-id="0909c-109">属性</span><span class="sxs-lookup"><span data-stu-id="0909c-109">Property</span></span>|<span data-ttu-id="0909c-110">类型</span><span class="sxs-lookup"><span data-stu-id="0909c-110">Type</span></span>|<span data-ttu-id="0909c-111">说明</span><span class="sxs-lookup"><span data-stu-id="0909c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0909c-112">name</span><span class="sxs-lookup"><span data-stu-id="0909c-112">name</span></span>|<span data-ttu-id="0909c-113">String</span><span class="sxs-lookup"><span data-stu-id="0909c-113">String</span></span>|<span data-ttu-id="0909c-114">从[KeyValuePair](../resources/intune-shared-keyvaluepair.md)继承的此键/值对的名称</span><span class="sxs-lookup"><span data-stu-id="0909c-114">Name for this key-value pair Inherited from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>|
|<span data-ttu-id="0909c-115">value</span><span class="sxs-lookup"><span data-stu-id="0909c-115">value</span></span>|<span data-ttu-id="0909c-116">String</span><span class="sxs-lookup"><span data-stu-id="0909c-116">String</span></span>|<span data-ttu-id="0909c-117">从[KeyValuePair](../resources/intune-shared-keyvaluepair.md)继承的此键/值对的值</span><span class="sxs-lookup"><span data-stu-id="0909c-117">Value for this key-value pair Inherited from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0909c-118">关系</span><span class="sxs-lookup"><span data-stu-id="0909c-118">Relationships</span></span>
<span data-ttu-id="0909c-119">无</span><span class="sxs-lookup"><span data-stu-id="0909c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0909c-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0909c-120">JSON Representation</span></span>
<span data-ttu-id="0909c-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0909c-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAssociatedDomainsKeyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAssociatedDomainsKeyValuePair",
  "name": "String",
  "value": "String"
}
```



