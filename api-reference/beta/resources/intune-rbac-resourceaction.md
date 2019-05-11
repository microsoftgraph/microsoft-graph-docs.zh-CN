---
title: resourceAction 资源类型
description: 资源的允许和不允许的操作的集合。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 597a9c7cdc2f04247e799772f100d1a0b778453e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939985"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="a7cbe-103">resourceAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7cbe-103">resourceAction resource type</span></span>

> <span data-ttu-id="a7cbe-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a7cbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7cbe-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a7cbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7cbe-106">资源的允许和不允许的操作的集合。</span><span class="sxs-lookup"><span data-stu-id="a7cbe-106">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="a7cbe-107">属性</span><span class="sxs-lookup"><span data-stu-id="a7cbe-107">Properties</span></span>
|<span data-ttu-id="a7cbe-108">属性</span><span class="sxs-lookup"><span data-stu-id="a7cbe-108">Property</span></span>|<span data-ttu-id="a7cbe-109">类型</span><span class="sxs-lookup"><span data-stu-id="a7cbe-109">Type</span></span>|<span data-ttu-id="a7cbe-110">说明</span><span class="sxs-lookup"><span data-stu-id="a7cbe-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7cbe-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="a7cbe-111">allowedResourceActions</span></span>|<span data-ttu-id="a7cbe-112">字符串集合</span><span class="sxs-lookup"><span data-stu-id="a7cbe-112">String collection</span></span>|<span data-ttu-id="a7cbe-113">允许的操作</span><span class="sxs-lookup"><span data-stu-id="a7cbe-113">Allowed Actions</span></span>|
|<span data-ttu-id="a7cbe-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="a7cbe-114">notAllowedResourceActions</span></span>|<span data-ttu-id="a7cbe-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="a7cbe-115">String collection</span></span>|<span data-ttu-id="a7cbe-116">不允许操作。</span><span class="sxs-lookup"><span data-stu-id="a7cbe-116">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7cbe-117">关系</span><span class="sxs-lookup"><span data-stu-id="a7cbe-117">Relationships</span></span>
<span data-ttu-id="a7cbe-118">无</span><span class="sxs-lookup"><span data-stu-id="a7cbe-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7cbe-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7cbe-119">JSON Representation</span></span>
<span data-ttu-id="a7cbe-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7cbe-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```




