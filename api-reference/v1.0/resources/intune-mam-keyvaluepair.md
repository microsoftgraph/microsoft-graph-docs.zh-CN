---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c0ced5c90f0e36906a534523836e7be3b99eb797
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533191"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="51c39-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="51c39-103">keyValuePair resource type</span></span>

<span data-ttu-id="51c39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51c39-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51c39-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51c39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51c39-106">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="51c39-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="51c39-107">属性</span><span class="sxs-lookup"><span data-stu-id="51c39-107">Properties</span></span>
|<span data-ttu-id="51c39-108">属性</span><span class="sxs-lookup"><span data-stu-id="51c39-108">Property</span></span>|<span data-ttu-id="51c39-109">类型</span><span class="sxs-lookup"><span data-stu-id="51c39-109">Type</span></span>|<span data-ttu-id="51c39-110">说明</span><span class="sxs-lookup"><span data-stu-id="51c39-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51c39-111">name</span><span class="sxs-lookup"><span data-stu-id="51c39-111">name</span></span>|<span data-ttu-id="51c39-112">字符串</span><span class="sxs-lookup"><span data-stu-id="51c39-112">String</span></span>|<span data-ttu-id="51c39-113">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="51c39-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="51c39-114">value</span><span class="sxs-lookup"><span data-stu-id="51c39-114">value</span></span>|<span data-ttu-id="51c39-115">String</span><span class="sxs-lookup"><span data-stu-id="51c39-115">String</span></span>|<span data-ttu-id="51c39-116">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="51c39-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="51c39-117">关系</span><span class="sxs-lookup"><span data-stu-id="51c39-117">Relationships</span></span>
<span data-ttu-id="51c39-118">无</span><span class="sxs-lookup"><span data-stu-id="51c39-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51c39-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51c39-119">JSON Representation</span></span>
<span data-ttu-id="51c39-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51c39-120">Here is a JSON representation of the resource.</span></span>
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




