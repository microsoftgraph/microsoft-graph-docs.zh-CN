---
title: deviceActionResult 资源类型
description: 设备操作结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 759db547e2b1d33dbf8881cbd3ee5c5d5dfa3e4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091269"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="61ab7-103">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="61ab7-103">deviceActionResult resource type</span></span>

<span data-ttu-id="61ab7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61ab7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61ab7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="61ab7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61ab7-106">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="61ab7-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="61ab7-107">属性</span><span class="sxs-lookup"><span data-stu-id="61ab7-107">Properties</span></span>
|<span data-ttu-id="61ab7-108">属性</span><span class="sxs-lookup"><span data-stu-id="61ab7-108">Property</span></span>|<span data-ttu-id="61ab7-109">类型</span><span class="sxs-lookup"><span data-stu-id="61ab7-109">Type</span></span>|<span data-ttu-id="61ab7-110">说明</span><span class="sxs-lookup"><span data-stu-id="61ab7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61ab7-111">actionName</span><span class="sxs-lookup"><span data-stu-id="61ab7-111">actionName</span></span>|<span data-ttu-id="61ab7-112">String</span><span class="sxs-lookup"><span data-stu-id="61ab7-112">String</span></span>|<span data-ttu-id="61ab7-113">操作名</span><span class="sxs-lookup"><span data-stu-id="61ab7-113">Action name</span></span>|
|<span data-ttu-id="61ab7-114">actionState</span><span class="sxs-lookup"><span data-stu-id="61ab7-114">actionState</span></span>|[<span data-ttu-id="61ab7-115">actionState</span><span class="sxs-lookup"><span data-stu-id="61ab7-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="61ab7-116">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="61ab7-116">State of the action.</span></span> <span data-ttu-id="61ab7-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="61ab7-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="61ab7-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="61ab7-118">startDateTime</span></span>|<span data-ttu-id="61ab7-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61ab7-119">DateTimeOffset</span></span>|<span data-ttu-id="61ab7-120">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="61ab7-120">Time the action was initiated</span></span>|
|<span data-ttu-id="61ab7-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="61ab7-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="61ab7-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61ab7-122">DateTimeOffset</span></span>|<span data-ttu-id="61ab7-123">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="61ab7-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="61ab7-124">关系</span><span class="sxs-lookup"><span data-stu-id="61ab7-124">Relationships</span></span>
<span data-ttu-id="61ab7-125">无</span><span class="sxs-lookup"><span data-stu-id="61ab7-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61ab7-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61ab7-126">JSON Representation</span></span>
<span data-ttu-id="61ab7-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61ab7-127">Here is a JSON representation of the resource.</span></span>
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









