---
title: deviceActionResult 资源类型
description: 设备操作结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 18e092c91a3e971a81c50e23a6f83c745be5d83c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267752"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="d97b3-103">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="d97b3-103">deviceActionResult resource type</span></span>

<span data-ttu-id="d97b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d97b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d97b3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d97b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d97b3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d97b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d97b3-107">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="d97b3-107">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="d97b3-108">属性</span><span class="sxs-lookup"><span data-stu-id="d97b3-108">Properties</span></span>
|<span data-ttu-id="d97b3-109">属性</span><span class="sxs-lookup"><span data-stu-id="d97b3-109">Property</span></span>|<span data-ttu-id="d97b3-110">类型</span><span class="sxs-lookup"><span data-stu-id="d97b3-110">Type</span></span>|<span data-ttu-id="d97b3-111">说明</span><span class="sxs-lookup"><span data-stu-id="d97b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d97b3-112">actionName</span><span class="sxs-lookup"><span data-stu-id="d97b3-112">actionName</span></span>|<span data-ttu-id="d97b3-113">String</span><span class="sxs-lookup"><span data-stu-id="d97b3-113">String</span></span>|<span data-ttu-id="d97b3-114">操作名</span><span class="sxs-lookup"><span data-stu-id="d97b3-114">Action name</span></span>|
|<span data-ttu-id="d97b3-115">actionState</span><span class="sxs-lookup"><span data-stu-id="d97b3-115">actionState</span></span>|[<span data-ttu-id="d97b3-116">actionState</span><span class="sxs-lookup"><span data-stu-id="d97b3-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d97b3-117">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="d97b3-117">State of the action.</span></span> <span data-ttu-id="d97b3-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="d97b3-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d97b3-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d97b3-119">startDateTime</span></span>|<span data-ttu-id="d97b3-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d97b3-120">DateTimeOffset</span></span>|<span data-ttu-id="d97b3-121">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="d97b3-121">Time the action was initiated</span></span>|
|<span data-ttu-id="d97b3-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d97b3-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="d97b3-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d97b3-123">DateTimeOffset</span></span>|<span data-ttu-id="d97b3-124">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="d97b3-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="d97b3-125">关系</span><span class="sxs-lookup"><span data-stu-id="d97b3-125">Relationships</span></span>
<span data-ttu-id="d97b3-126">无</span><span class="sxs-lookup"><span data-stu-id="d97b3-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d97b3-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d97b3-127">JSON Representation</span></span>
<span data-ttu-id="d97b3-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d97b3-128">Here is a JSON representation of the resource.</span></span>
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




