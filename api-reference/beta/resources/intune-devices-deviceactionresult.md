---
title: deviceActionResult 资源类型
description: 设备操作结果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c435241056f5e29166355829d1c40438b525a92
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151427"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="ba248-103">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba248-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="ba248-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ba248-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba248-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ba248-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba248-106">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="ba248-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="ba248-107">属性</span><span class="sxs-lookup"><span data-stu-id="ba248-107">Properties</span></span>
|<span data-ttu-id="ba248-108">属性</span><span class="sxs-lookup"><span data-stu-id="ba248-108">Property</span></span>|<span data-ttu-id="ba248-109">类型</span><span class="sxs-lookup"><span data-stu-id="ba248-109">Type</span></span>|<span data-ttu-id="ba248-110">说明</span><span class="sxs-lookup"><span data-stu-id="ba248-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba248-111">actionName</span><span class="sxs-lookup"><span data-stu-id="ba248-111">actionName</span></span>|<span data-ttu-id="ba248-112">String</span><span class="sxs-lookup"><span data-stu-id="ba248-112">String</span></span>|<span data-ttu-id="ba248-113">操作名</span><span class="sxs-lookup"><span data-stu-id="ba248-113">Action name</span></span>|
|<span data-ttu-id="ba248-114">actionState</span><span class="sxs-lookup"><span data-stu-id="ba248-114">actionState</span></span>|[<span data-ttu-id="ba248-115">actionState</span><span class="sxs-lookup"><span data-stu-id="ba248-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ba248-116">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="ba248-116">State of the action.</span></span> <span data-ttu-id="ba248-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="ba248-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ba248-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ba248-118">startDateTime</span></span>|<span data-ttu-id="ba248-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba248-119">DateTimeOffset</span></span>|<span data-ttu-id="ba248-120">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="ba248-120">Time the action was initiated</span></span>|
|<span data-ttu-id="ba248-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba248-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="ba248-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba248-122">DateTimeOffset</span></span>|<span data-ttu-id="ba248-123">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="ba248-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba248-124">关系</span><span class="sxs-lookup"><span data-stu-id="ba248-124">Relationships</span></span>
<span data-ttu-id="ba248-125">无</span><span class="sxs-lookup"><span data-stu-id="ba248-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba248-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba248-126">JSON Representation</span></span>
<span data-ttu-id="ba248-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba248-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




