---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 69924cf755192d8ddefa074b9ec1cfed53a0d5f7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347946"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="bb1f9-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb1f9-103">keyValuePair resource type</span></span>

> <span data-ttu-id="bb1f9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb1f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb1f9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb1f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb1f9-106">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="bb1f9-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="bb1f9-107">属性</span><span class="sxs-lookup"><span data-stu-id="bb1f9-107">Properties</span></span>
|<span data-ttu-id="bb1f9-108">属性</span><span class="sxs-lookup"><span data-stu-id="bb1f9-108">Property</span></span>|<span data-ttu-id="bb1f9-109">类型</span><span class="sxs-lookup"><span data-stu-id="bb1f9-109">Type</span></span>|<span data-ttu-id="bb1f9-110">说明</span><span class="sxs-lookup"><span data-stu-id="bb1f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb1f9-111">name</span><span class="sxs-lookup"><span data-stu-id="bb1f9-111">name</span></span>|<span data-ttu-id="bb1f9-112">String</span><span class="sxs-lookup"><span data-stu-id="bb1f9-112">String</span></span>|<span data-ttu-id="bb1f9-113">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="bb1f9-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="bb1f9-114">value</span><span class="sxs-lookup"><span data-stu-id="bb1f9-114">value</span></span>|<span data-ttu-id="bb1f9-115">String</span><span class="sxs-lookup"><span data-stu-id="bb1f9-115">String</span></span>|<span data-ttu-id="bb1f9-116">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="bb1f9-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb1f9-117">关系</span><span class="sxs-lookup"><span data-stu-id="bb1f9-117">Relationships</span></span>
<span data-ttu-id="bb1f9-118">无</span><span class="sxs-lookup"><span data-stu-id="bb1f9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb1f9-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb1f9-119">JSON Representation</span></span>
<span data-ttu-id="bb1f9-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb1f9-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```



