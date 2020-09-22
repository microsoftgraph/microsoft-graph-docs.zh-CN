---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e0ead3529d9b5ac3e782631301c8db89a089b9ef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095104"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="9352e-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="9352e-103">keyValuePair resource type</span></span>

<span data-ttu-id="9352e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9352e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9352e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9352e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9352e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9352e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9352e-107">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="9352e-107">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="9352e-108">属性</span><span class="sxs-lookup"><span data-stu-id="9352e-108">Properties</span></span>
|<span data-ttu-id="9352e-109">属性</span><span class="sxs-lookup"><span data-stu-id="9352e-109">Property</span></span>|<span data-ttu-id="9352e-110">类型</span><span class="sxs-lookup"><span data-stu-id="9352e-110">Type</span></span>|<span data-ttu-id="9352e-111">说明</span><span class="sxs-lookup"><span data-stu-id="9352e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9352e-112">名称</span><span class="sxs-lookup"><span data-stu-id="9352e-112">name</span></span>|<span data-ttu-id="9352e-113">字符串</span><span class="sxs-lookup"><span data-stu-id="9352e-113">String</span></span>|<span data-ttu-id="9352e-114">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="9352e-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="9352e-115">value</span><span class="sxs-lookup"><span data-stu-id="9352e-115">value</span></span>|<span data-ttu-id="9352e-116">String</span><span class="sxs-lookup"><span data-stu-id="9352e-116">String</span></span>|<span data-ttu-id="9352e-117">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="9352e-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="9352e-118">关系</span><span class="sxs-lookup"><span data-stu-id="9352e-118">Relationships</span></span>
<span data-ttu-id="9352e-119">无</span><span class="sxs-lookup"><span data-stu-id="9352e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9352e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9352e-120">JSON Representation</span></span>
<span data-ttu-id="9352e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9352e-121">Here is a JSON representation of the resource.</span></span>
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






