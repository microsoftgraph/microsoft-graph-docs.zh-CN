---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc34bad30ff5bc33f60e6ec4e561e6644b97cc37
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938658"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="525e5-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="525e5-103">keyValuePair resource type</span></span>

> <span data-ttu-id="525e5-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="525e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="525e5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="525e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="525e5-106">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="525e5-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="525e5-107">属性</span><span class="sxs-lookup"><span data-stu-id="525e5-107">Properties</span></span>
|<span data-ttu-id="525e5-108">属性</span><span class="sxs-lookup"><span data-stu-id="525e5-108">Property</span></span>|<span data-ttu-id="525e5-109">类型</span><span class="sxs-lookup"><span data-stu-id="525e5-109">Type</span></span>|<span data-ttu-id="525e5-110">说明</span><span class="sxs-lookup"><span data-stu-id="525e5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="525e5-111">name</span><span class="sxs-lookup"><span data-stu-id="525e5-111">name</span></span>|<span data-ttu-id="525e5-112">String</span><span class="sxs-lookup"><span data-stu-id="525e5-112">String</span></span>|<span data-ttu-id="525e5-113">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="525e5-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="525e5-114">value</span><span class="sxs-lookup"><span data-stu-id="525e5-114">value</span></span>|<span data-ttu-id="525e5-115">String</span><span class="sxs-lookup"><span data-stu-id="525e5-115">String</span></span>|<span data-ttu-id="525e5-116">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="525e5-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="525e5-117">关系</span><span class="sxs-lookup"><span data-stu-id="525e5-117">Relationships</span></span>
<span data-ttu-id="525e5-118">无</span><span class="sxs-lookup"><span data-stu-id="525e5-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="525e5-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="525e5-119">JSON Representation</span></span>
<span data-ttu-id="525e5-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="525e5-120">Here is a JSON representation of the resource.</span></span>
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




