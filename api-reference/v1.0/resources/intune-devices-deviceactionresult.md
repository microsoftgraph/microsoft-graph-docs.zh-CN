---
title: deviceActionResult 资源类型
description: 设备操作结果
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1b802d1b09fbe65e9e1e72e4c34a387462e12113
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861122"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="b9d40-103">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9d40-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="b9d40-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b9d40-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9d40-105">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="b9d40-105">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="b9d40-106">属性</span><span class="sxs-lookup"><span data-stu-id="b9d40-106">Properties</span></span>
|<span data-ttu-id="b9d40-107">属性</span><span class="sxs-lookup"><span data-stu-id="b9d40-107">Property</span></span>|<span data-ttu-id="b9d40-108">类型</span><span class="sxs-lookup"><span data-stu-id="b9d40-108">Type</span></span>|<span data-ttu-id="b9d40-109">说明</span><span class="sxs-lookup"><span data-stu-id="b9d40-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9d40-110">actionName</span><span class="sxs-lookup"><span data-stu-id="b9d40-110">actionName</span></span>|<span data-ttu-id="b9d40-111">String</span><span class="sxs-lookup"><span data-stu-id="b9d40-111">String</span></span>|<span data-ttu-id="b9d40-112">操作名</span><span class="sxs-lookup"><span data-stu-id="b9d40-112">Action name</span></span>|
|<span data-ttu-id="b9d40-113">actionState</span><span class="sxs-lookup"><span data-stu-id="b9d40-113">actionState</span></span>|[<span data-ttu-id="b9d40-114">actionState</span><span class="sxs-lookup"><span data-stu-id="b9d40-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="b9d40-115">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="b9d40-115">State of the action.</span></span> <span data-ttu-id="b9d40-116">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="b9d40-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b9d40-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b9d40-117">startDateTime</span></span>|<span data-ttu-id="b9d40-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9d40-118">DateTimeOffset</span></span>|<span data-ttu-id="b9d40-119">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="b9d40-119">Time the action was initiated</span></span>|
|<span data-ttu-id="b9d40-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9d40-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="b9d40-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9d40-121">DateTimeOffset</span></span>|<span data-ttu-id="b9d40-122">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="b9d40-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9d40-123">关系</span><span class="sxs-lookup"><span data-stu-id="b9d40-123">Relationships</span></span>
<span data-ttu-id="b9d40-124">无</span><span class="sxs-lookup"><span data-stu-id="b9d40-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b9d40-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9d40-125">JSON Representation</span></span>
<span data-ttu-id="b9d40-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9d40-126">Here is a JSON representation of the resource.</span></span>
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



