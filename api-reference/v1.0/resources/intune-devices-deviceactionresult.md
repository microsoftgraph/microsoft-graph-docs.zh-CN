---
title: deviceActionResult 资源类型
description: 设备操作结果
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1965a537726ebbaa0d461ea31403dd1110867f9a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533302"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="055f2-103">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="055f2-103">deviceActionResult resource type</span></span>

<span data-ttu-id="055f2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="055f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="055f2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="055f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="055f2-106">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="055f2-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="055f2-107">属性</span><span class="sxs-lookup"><span data-stu-id="055f2-107">Properties</span></span>
|<span data-ttu-id="055f2-108">属性</span><span class="sxs-lookup"><span data-stu-id="055f2-108">Property</span></span>|<span data-ttu-id="055f2-109">类型</span><span class="sxs-lookup"><span data-stu-id="055f2-109">Type</span></span>|<span data-ttu-id="055f2-110">说明</span><span class="sxs-lookup"><span data-stu-id="055f2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="055f2-111">actionName</span><span class="sxs-lookup"><span data-stu-id="055f2-111">actionName</span></span>|<span data-ttu-id="055f2-112">String</span><span class="sxs-lookup"><span data-stu-id="055f2-112">String</span></span>|<span data-ttu-id="055f2-113">操作名</span><span class="sxs-lookup"><span data-stu-id="055f2-113">Action name</span></span>|
|<span data-ttu-id="055f2-114">actionState</span><span class="sxs-lookup"><span data-stu-id="055f2-114">actionState</span></span>|[<span data-ttu-id="055f2-115">actionState</span><span class="sxs-lookup"><span data-stu-id="055f2-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="055f2-116">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="055f2-116">State of the action.</span></span> <span data-ttu-id="055f2-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="055f2-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="055f2-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="055f2-118">startDateTime</span></span>|<span data-ttu-id="055f2-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="055f2-119">DateTimeOffset</span></span>|<span data-ttu-id="055f2-120">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="055f2-120">Time the action was initiated</span></span>|
|<span data-ttu-id="055f2-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="055f2-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="055f2-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="055f2-122">DateTimeOffset</span></span>|<span data-ttu-id="055f2-123">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="055f2-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="055f2-124">关系</span><span class="sxs-lookup"><span data-stu-id="055f2-124">Relationships</span></span>
<span data-ttu-id="055f2-125">无</span><span class="sxs-lookup"><span data-stu-id="055f2-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="055f2-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="055f2-126">JSON Representation</span></span>
<span data-ttu-id="055f2-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="055f2-127">Here is a JSON representation of the resource.</span></span>
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




