---
title: keyValuePair 资源类型
description: 用于存储自定义设置的键值对
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b41f0b18b30945e12df21b780afd7fcf1cade73
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527388"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="192a9-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="192a9-103">keyValuePair resource type</span></span>

<span data-ttu-id="192a9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="192a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="192a9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="192a9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="192a9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="192a9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="192a9-107">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="192a9-107">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="192a9-108">属性</span><span class="sxs-lookup"><span data-stu-id="192a9-108">Properties</span></span>
|<span data-ttu-id="192a9-109">属性</span><span class="sxs-lookup"><span data-stu-id="192a9-109">Property</span></span>|<span data-ttu-id="192a9-110">类型</span><span class="sxs-lookup"><span data-stu-id="192a9-110">Type</span></span>|<span data-ttu-id="192a9-111">说明</span><span class="sxs-lookup"><span data-stu-id="192a9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="192a9-112">name</span><span class="sxs-lookup"><span data-stu-id="192a9-112">name</span></span>|<span data-ttu-id="192a9-113">String</span><span class="sxs-lookup"><span data-stu-id="192a9-113">String</span></span>|<span data-ttu-id="192a9-114">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="192a9-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="192a9-115">value</span><span class="sxs-lookup"><span data-stu-id="192a9-115">value</span></span>|<span data-ttu-id="192a9-116">String</span><span class="sxs-lookup"><span data-stu-id="192a9-116">String</span></span>|<span data-ttu-id="192a9-117">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="192a9-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="192a9-118">关系</span><span class="sxs-lookup"><span data-stu-id="192a9-118">Relationships</span></span>
<span data-ttu-id="192a9-119">无</span><span class="sxs-lookup"><span data-stu-id="192a9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="192a9-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="192a9-120">JSON Representation</span></span>
<span data-ttu-id="192a9-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="192a9-121">Here is a JSON representation of the resource.</span></span>
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



