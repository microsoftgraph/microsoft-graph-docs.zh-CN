---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a8feecabeca3cfc916c0bd3ce1b87cab3a68809
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160793"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="f751b-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="f751b-103">keyValuePair resource type</span></span>

> <span data-ttu-id="f751b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f751b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f751b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f751b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f751b-106">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="f751b-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="f751b-107">属性</span><span class="sxs-lookup"><span data-stu-id="f751b-107">Properties</span></span>
|<span data-ttu-id="f751b-108">属性</span><span class="sxs-lookup"><span data-stu-id="f751b-108">Property</span></span>|<span data-ttu-id="f751b-109">类型</span><span class="sxs-lookup"><span data-stu-id="f751b-109">Type</span></span>|<span data-ttu-id="f751b-110">说明</span><span class="sxs-lookup"><span data-stu-id="f751b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f751b-111">name</span><span class="sxs-lookup"><span data-stu-id="f751b-111">name</span></span>|<span data-ttu-id="f751b-112">String</span><span class="sxs-lookup"><span data-stu-id="f751b-112">String</span></span>|<span data-ttu-id="f751b-113">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="f751b-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="f751b-114">值</span><span class="sxs-lookup"><span data-stu-id="f751b-114">value</span></span>|<span data-ttu-id="f751b-115">String</span><span class="sxs-lookup"><span data-stu-id="f751b-115">String</span></span>|<span data-ttu-id="f751b-116">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="f751b-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="f751b-117">关系</span><span class="sxs-lookup"><span data-stu-id="f751b-117">Relationships</span></span>
<span data-ttu-id="f751b-118">无</span><span class="sxs-lookup"><span data-stu-id="f751b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f751b-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f751b-119">JSON Representation</span></span>
<span data-ttu-id="f751b-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f751b-120">Here is a JSON representation of the resource.</span></span>
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




