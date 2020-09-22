---
title: macOSAssociatedDomainsKeyValuePair 资源类型
description: 关联域的键值对
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bc73af5746dce61961563b84871e35bab1982c09
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055440"
---
# <a name="macosassociateddomainskeyvaluepair-resource-type"></a><span data-ttu-id="250f2-103">macOSAssociatedDomainsKeyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="250f2-103">macOSAssociatedDomainsKeyValuePair resource type</span></span>

<span data-ttu-id="250f2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="250f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="250f2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="250f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="250f2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="250f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="250f2-107">关联域的键值对</span><span class="sxs-lookup"><span data-stu-id="250f2-107">Key value pair for associated domains</span></span>


<span data-ttu-id="250f2-108">继承自 [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="250f2-108">Inherits from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="250f2-109">属性</span><span class="sxs-lookup"><span data-stu-id="250f2-109">Properties</span></span>
|<span data-ttu-id="250f2-110">属性</span><span class="sxs-lookup"><span data-stu-id="250f2-110">Property</span></span>|<span data-ttu-id="250f2-111">类型</span><span class="sxs-lookup"><span data-stu-id="250f2-111">Type</span></span>|<span data-ttu-id="250f2-112">说明</span><span class="sxs-lookup"><span data-stu-id="250f2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="250f2-113">名称</span><span class="sxs-lookup"><span data-stu-id="250f2-113">name</span></span>|<span data-ttu-id="250f2-114">String</span><span class="sxs-lookup"><span data-stu-id="250f2-114">String</span></span>|<span data-ttu-id="250f2-115">从[KeyValuePair](../resources/intune-shared-keyvaluepair.md)继承的此键/值对的名称</span><span class="sxs-lookup"><span data-stu-id="250f2-115">Name for this key-value pair Inherited from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>|
|<span data-ttu-id="250f2-116">value</span><span class="sxs-lookup"><span data-stu-id="250f2-116">value</span></span>|<span data-ttu-id="250f2-117">String</span><span class="sxs-lookup"><span data-stu-id="250f2-117">String</span></span>|<span data-ttu-id="250f2-118">从[KeyValuePair](../resources/intune-shared-keyvaluepair.md)继承的此键/值对的值</span><span class="sxs-lookup"><span data-stu-id="250f2-118">Value for this key-value pair Inherited from [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="250f2-119">关系</span><span class="sxs-lookup"><span data-stu-id="250f2-119">Relationships</span></span>
<span data-ttu-id="250f2-120">无</span><span class="sxs-lookup"><span data-stu-id="250f2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="250f2-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="250f2-121">JSON Representation</span></span>
<span data-ttu-id="250f2-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="250f2-122">Here is a JSON representation of the resource.</span></span>
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






