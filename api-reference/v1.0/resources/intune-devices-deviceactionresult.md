---
title: deviceActionResult 资源类型
description: 设备操作结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 808d9e559494338a7831626fd6d4d77f20092dcb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755775"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="fe163-103">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe163-103">deviceActionResult resource type</span></span>

<span data-ttu-id="fe163-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe163-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe163-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fe163-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe163-106">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="fe163-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="fe163-107">属性</span><span class="sxs-lookup"><span data-stu-id="fe163-107">Properties</span></span>
|<span data-ttu-id="fe163-108">属性</span><span class="sxs-lookup"><span data-stu-id="fe163-108">Property</span></span>|<span data-ttu-id="fe163-109">类型</span><span class="sxs-lookup"><span data-stu-id="fe163-109">Type</span></span>|<span data-ttu-id="fe163-110">Description</span><span class="sxs-lookup"><span data-stu-id="fe163-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe163-111">actionName</span><span class="sxs-lookup"><span data-stu-id="fe163-111">actionName</span></span>|<span data-ttu-id="fe163-112">String</span><span class="sxs-lookup"><span data-stu-id="fe163-112">String</span></span>|<span data-ttu-id="fe163-113">操作名</span><span class="sxs-lookup"><span data-stu-id="fe163-113">Action name</span></span>|
|<span data-ttu-id="fe163-114">actionState</span><span class="sxs-lookup"><span data-stu-id="fe163-114">actionState</span></span>|[<span data-ttu-id="fe163-115">actionState</span><span class="sxs-lookup"><span data-stu-id="fe163-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="fe163-116">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="fe163-116">State of the action.</span></span> <span data-ttu-id="fe163-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="fe163-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="fe163-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fe163-118">startDateTime</span></span>|<span data-ttu-id="fe163-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe163-119">DateTimeOffset</span></span>|<span data-ttu-id="fe163-120">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="fe163-120">Time the action was initiated</span></span>|
|<span data-ttu-id="fe163-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe163-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="fe163-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe163-122">DateTimeOffset</span></span>|<span data-ttu-id="fe163-123">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="fe163-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe163-124">关系</span><span class="sxs-lookup"><span data-stu-id="fe163-124">Relationships</span></span>
<span data-ttu-id="fe163-125">无</span><span class="sxs-lookup"><span data-stu-id="fe163-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe163-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe163-126">JSON Representation</span></span>
<span data-ttu-id="fe163-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe163-127">Here is a JSON representation of the resource.</span></span>
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




