---
title: deviceActionResult 资源类型
description: 设备操作结果
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0f0e6612eccf309cc03dea51c50dfcf06d1b6567
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456876"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="0df65-103">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="0df65-103">deviceActionResult resource type</span></span>

<span data-ttu-id="0df65-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0df65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0df65-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0df65-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0df65-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0df65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0df65-107">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="0df65-107">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="0df65-108">属性</span><span class="sxs-lookup"><span data-stu-id="0df65-108">Properties</span></span>
|<span data-ttu-id="0df65-109">属性</span><span class="sxs-lookup"><span data-stu-id="0df65-109">Property</span></span>|<span data-ttu-id="0df65-110">类型</span><span class="sxs-lookup"><span data-stu-id="0df65-110">Type</span></span>|<span data-ttu-id="0df65-111">说明</span><span class="sxs-lookup"><span data-stu-id="0df65-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0df65-112">actionName</span><span class="sxs-lookup"><span data-stu-id="0df65-112">actionName</span></span>|<span data-ttu-id="0df65-113">String</span><span class="sxs-lookup"><span data-stu-id="0df65-113">String</span></span>|<span data-ttu-id="0df65-114">操作名</span><span class="sxs-lookup"><span data-stu-id="0df65-114">Action name</span></span>|
|<span data-ttu-id="0df65-115">actionState</span><span class="sxs-lookup"><span data-stu-id="0df65-115">actionState</span></span>|[<span data-ttu-id="0df65-116">actionState</span><span class="sxs-lookup"><span data-stu-id="0df65-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="0df65-117">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="0df65-117">State of the action.</span></span> <span data-ttu-id="0df65-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="0df65-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="0df65-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0df65-119">startDateTime</span></span>|<span data-ttu-id="0df65-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0df65-120">DateTimeOffset</span></span>|<span data-ttu-id="0df65-121">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="0df65-121">Time the action was initiated</span></span>|
|<span data-ttu-id="0df65-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0df65-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="0df65-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0df65-123">DateTimeOffset</span></span>|<span data-ttu-id="0df65-124">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="0df65-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="0df65-125">关系</span><span class="sxs-lookup"><span data-stu-id="0df65-125">Relationships</span></span>
<span data-ttu-id="0df65-126">无</span><span class="sxs-lookup"><span data-stu-id="0df65-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0df65-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0df65-127">JSON Representation</span></span>
<span data-ttu-id="0df65-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0df65-128">Here is a JSON representation of the resource.</span></span>
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



