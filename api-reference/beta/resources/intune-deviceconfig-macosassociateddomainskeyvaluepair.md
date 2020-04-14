---
title: macOSAssociatedDomainsKeyValuePair 资源类型
description: 关联域的键值对
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ebf62a01d4a97fde51974ea2e7984b97c39dc5d4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439720"
---
# <a name="macosassociateddomainskeyvaluepair-resource-type"></a><span data-ttu-id="6048b-103">macOSAssociatedDomainsKeyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="6048b-103">macOSAssociatedDomainsKeyValuePair resource type</span></span>

<span data-ttu-id="6048b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6048b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6048b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6048b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6048b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6048b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6048b-107">关联域的键值对</span><span class="sxs-lookup"><span data-stu-id="6048b-107">Key value pair for associated domains</span></span>


<span data-ttu-id="6048b-108">继承自[keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6048b-108">Inherits from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6048b-109">属性</span><span class="sxs-lookup"><span data-stu-id="6048b-109">Properties</span></span>
|<span data-ttu-id="6048b-110">属性</span><span class="sxs-lookup"><span data-stu-id="6048b-110">Property</span></span>|<span data-ttu-id="6048b-111">类型</span><span class="sxs-lookup"><span data-stu-id="6048b-111">Type</span></span>|<span data-ttu-id="6048b-112">说明</span><span class="sxs-lookup"><span data-stu-id="6048b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6048b-113">name</span><span class="sxs-lookup"><span data-stu-id="6048b-113">name</span></span>|<span data-ttu-id="6048b-114">String</span><span class="sxs-lookup"><span data-stu-id="6048b-114">String</span></span>|<span data-ttu-id="6048b-115">从[KeyValuePair](../resources/intune-shared-keyvaluepair.md)继承的此键/值对的名称</span><span class="sxs-lookup"><span data-stu-id="6048b-115">Name for this key-value pair Inherited from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>|
|<span data-ttu-id="6048b-116">value</span><span class="sxs-lookup"><span data-stu-id="6048b-116">value</span></span>|<span data-ttu-id="6048b-117">String</span><span class="sxs-lookup"><span data-stu-id="6048b-117">String</span></span>|<span data-ttu-id="6048b-118">从[KeyValuePair](../resources/intune-shared-keyvaluepair.md)继承的此键/值对的值</span><span class="sxs-lookup"><span data-stu-id="6048b-118">Value for this key-value pair Inherited from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6048b-119">关系</span><span class="sxs-lookup"><span data-stu-id="6048b-119">Relationships</span></span>
<span data-ttu-id="6048b-120">无</span><span class="sxs-lookup"><span data-stu-id="6048b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6048b-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6048b-121">JSON Representation</span></span>
<span data-ttu-id="6048b-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6048b-122">Here is a JSON representation of the resource.</span></span>
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



