---
title: deviceActionResult 资源类型
description: 设备操作结果
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e33b91b2fdd4b17ebfeef61a2e6917d24edf589d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942127"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="32c1b-103">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="32c1b-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="32c1b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="32c1b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32c1b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32c1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32c1b-106">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="32c1b-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="32c1b-107">属性</span><span class="sxs-lookup"><span data-stu-id="32c1b-107">Properties</span></span>
|<span data-ttu-id="32c1b-108">属性</span><span class="sxs-lookup"><span data-stu-id="32c1b-108">Property</span></span>|<span data-ttu-id="32c1b-109">类型</span><span class="sxs-lookup"><span data-stu-id="32c1b-109">Type</span></span>|<span data-ttu-id="32c1b-110">说明</span><span class="sxs-lookup"><span data-stu-id="32c1b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32c1b-111">actionName</span><span class="sxs-lookup"><span data-stu-id="32c1b-111">actionName</span></span>|<span data-ttu-id="32c1b-112">String</span><span class="sxs-lookup"><span data-stu-id="32c1b-112">String</span></span>|<span data-ttu-id="32c1b-113">操作名</span><span class="sxs-lookup"><span data-stu-id="32c1b-113">Action name</span></span>|
|<span data-ttu-id="32c1b-114">actionState</span><span class="sxs-lookup"><span data-stu-id="32c1b-114">actionState</span></span>|[<span data-ttu-id="32c1b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="32c1b-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="32c1b-116">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="32c1b-116">State of the action.</span></span> <span data-ttu-id="32c1b-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="32c1b-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="32c1b-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="32c1b-118">startDateTime</span></span>|<span data-ttu-id="32c1b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32c1b-119">DateTimeOffset</span></span>|<span data-ttu-id="32c1b-120">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="32c1b-120">Time the action was initiated</span></span>|
|<span data-ttu-id="32c1b-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="32c1b-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="32c1b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32c1b-122">DateTimeOffset</span></span>|<span data-ttu-id="32c1b-123">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="32c1b-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="32c1b-124">关系</span><span class="sxs-lookup"><span data-stu-id="32c1b-124">Relationships</span></span>
<span data-ttu-id="32c1b-125">无</span><span class="sxs-lookup"><span data-stu-id="32c1b-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32c1b-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32c1b-126">JSON Representation</span></span>
<span data-ttu-id="32c1b-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32c1b-127">Here is a JSON representation of the resource.</span></span>
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




