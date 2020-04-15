---
title: deviceActionResult 资源类型
description: 设备操作结果
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff9b34e6e84b8340e214f46f28ce7e243e72be5e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407041"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="06c65-103">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="06c65-103">deviceActionResult resource type</span></span>

<span data-ttu-id="06c65-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06c65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06c65-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06c65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06c65-106">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="06c65-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="06c65-107">属性</span><span class="sxs-lookup"><span data-stu-id="06c65-107">Properties</span></span>
|<span data-ttu-id="06c65-108">属性</span><span class="sxs-lookup"><span data-stu-id="06c65-108">Property</span></span>|<span data-ttu-id="06c65-109">类型</span><span class="sxs-lookup"><span data-stu-id="06c65-109">Type</span></span>|<span data-ttu-id="06c65-110">说明</span><span class="sxs-lookup"><span data-stu-id="06c65-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06c65-111">actionName</span><span class="sxs-lookup"><span data-stu-id="06c65-111">actionName</span></span>|<span data-ttu-id="06c65-112">String</span><span class="sxs-lookup"><span data-stu-id="06c65-112">String</span></span>|<span data-ttu-id="06c65-113">操作名</span><span class="sxs-lookup"><span data-stu-id="06c65-113">Action name</span></span>|
|<span data-ttu-id="06c65-114">actionState</span><span class="sxs-lookup"><span data-stu-id="06c65-114">actionState</span></span>|[<span data-ttu-id="06c65-115">actionState</span><span class="sxs-lookup"><span data-stu-id="06c65-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="06c65-116">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="06c65-116">State of the action.</span></span> <span data-ttu-id="06c65-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="06c65-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="06c65-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="06c65-118">startDateTime</span></span>|<span data-ttu-id="06c65-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06c65-119">DateTimeOffset</span></span>|<span data-ttu-id="06c65-120">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="06c65-120">Time the action was initiated</span></span>|
|<span data-ttu-id="06c65-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="06c65-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="06c65-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06c65-122">DateTimeOffset</span></span>|<span data-ttu-id="06c65-123">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="06c65-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="06c65-124">关系</span><span class="sxs-lookup"><span data-stu-id="06c65-124">Relationships</span></span>
<span data-ttu-id="06c65-125">无</span><span class="sxs-lookup"><span data-stu-id="06c65-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06c65-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06c65-126">JSON Representation</span></span>
<span data-ttu-id="06c65-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06c65-127">Here is a JSON representation of the resource.</span></span>
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







