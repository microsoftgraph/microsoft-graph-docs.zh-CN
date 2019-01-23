---
title: deviceActionResult 资源类型
description: 设备操作结果
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 518d0d09d7ef4f9fea67ce8d600f97be0345fa63
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404706"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="894d7-103">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="894d7-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="894d7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="894d7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="894d7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="894d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="894d7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="894d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="894d7-107">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="894d7-107">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="894d7-108">属性</span><span class="sxs-lookup"><span data-stu-id="894d7-108">Properties</span></span>
|<span data-ttu-id="894d7-109">属性</span><span class="sxs-lookup"><span data-stu-id="894d7-109">Property</span></span>|<span data-ttu-id="894d7-110">类型</span><span class="sxs-lookup"><span data-stu-id="894d7-110">Type</span></span>|<span data-ttu-id="894d7-111">说明</span><span class="sxs-lookup"><span data-stu-id="894d7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="894d7-112">actionName</span><span class="sxs-lookup"><span data-stu-id="894d7-112">actionName</span></span>|<span data-ttu-id="894d7-113">String</span><span class="sxs-lookup"><span data-stu-id="894d7-113">String</span></span>|<span data-ttu-id="894d7-114">操作名</span><span class="sxs-lookup"><span data-stu-id="894d7-114">Action name</span></span>|
|<span data-ttu-id="894d7-115">actionState</span><span class="sxs-lookup"><span data-stu-id="894d7-115">actionState</span></span>|[<span data-ttu-id="894d7-116">actionState</span><span class="sxs-lookup"><span data-stu-id="894d7-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="894d7-117">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="894d7-117">State of the action.</span></span> <span data-ttu-id="894d7-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="894d7-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="894d7-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="894d7-119">startDateTime</span></span>|<span data-ttu-id="894d7-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="894d7-120">DateTimeOffset</span></span>|<span data-ttu-id="894d7-121">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="894d7-121">Time the action was initiated</span></span>|
|<span data-ttu-id="894d7-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="894d7-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="894d7-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="894d7-123">DateTimeOffset</span></span>|<span data-ttu-id="894d7-124">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="894d7-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="894d7-125">关系</span><span class="sxs-lookup"><span data-stu-id="894d7-125">Relationships</span></span>
<span data-ttu-id="894d7-126">无</span><span class="sxs-lookup"><span data-stu-id="894d7-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="894d7-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="894d7-127">JSON Representation</span></span>
<span data-ttu-id="894d7-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="894d7-128">Here is a JSON representation of the resource.</span></span>
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




