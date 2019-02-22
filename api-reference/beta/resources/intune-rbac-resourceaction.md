---
title: resourceAction 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d229a6d4d8b514cbf092efb224ff09dfb0c78ad4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157622"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="80128-103">resourceAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="80128-103">resourceAction resource type</span></span>

> <span data-ttu-id="80128-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="80128-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80128-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="80128-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80128-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="80128-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="80128-107">属性</span><span class="sxs-lookup"><span data-stu-id="80128-107">Properties</span></span>
|<span data-ttu-id="80128-108">属性</span><span class="sxs-lookup"><span data-stu-id="80128-108">Property</span></span>|<span data-ttu-id="80128-109">类型</span><span class="sxs-lookup"><span data-stu-id="80128-109">Type</span></span>|<span data-ttu-id="80128-110">说明</span><span class="sxs-lookup"><span data-stu-id="80128-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80128-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="80128-111">allowedResourceActions</span></span>|<span data-ttu-id="80128-112">String collection</span><span class="sxs-lookup"><span data-stu-id="80128-112">String collection</span></span>|<span data-ttu-id="80128-113">允许的操作</span><span class="sxs-lookup"><span data-stu-id="80128-113">Allowed Actions</span></span>|
|<span data-ttu-id="80128-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="80128-114">notAllowedResourceActions</span></span>|<span data-ttu-id="80128-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="80128-115">String collection</span></span>|<span data-ttu-id="80128-116">不允许的操作</span><span class="sxs-lookup"><span data-stu-id="80128-116">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="80128-117">关系</span><span class="sxs-lookup"><span data-stu-id="80128-117">Relationships</span></span>
<span data-ttu-id="80128-118">无</span><span class="sxs-lookup"><span data-stu-id="80128-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80128-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80128-119">JSON Representation</span></span>
<span data-ttu-id="80128-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80128-120">Here is a JSON representation of the resource.</span></span>
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




