---
title: vppTokenActionResult 资源类型
description: 使用 Apple volume purchase Program 令牌执行的操作的状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 853c5c12ca0a85fe0f5a16efa86321e46a28ec5c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159386"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="5cfba-103">vppTokenActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="5cfba-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="5cfba-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5cfba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cfba-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5cfba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cfba-106">使用 Apple volume purchase Program 令牌执行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="5cfba-106">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="5cfba-107">属性</span><span class="sxs-lookup"><span data-stu-id="5cfba-107">Properties</span></span>
|<span data-ttu-id="5cfba-108">属性</span><span class="sxs-lookup"><span data-stu-id="5cfba-108">Property</span></span>|<span data-ttu-id="5cfba-109">类型</span><span class="sxs-lookup"><span data-stu-id="5cfba-109">Type</span></span>|<span data-ttu-id="5cfba-110">说明</span><span class="sxs-lookup"><span data-stu-id="5cfba-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cfba-111">actionName</span><span class="sxs-lookup"><span data-stu-id="5cfba-111">actionName</span></span>|<span data-ttu-id="5cfba-112">String</span><span class="sxs-lookup"><span data-stu-id="5cfba-112">String</span></span>|<span data-ttu-id="5cfba-113">操作名</span><span class="sxs-lookup"><span data-stu-id="5cfba-113">Action name</span></span>|
|<span data-ttu-id="5cfba-114">actionState</span><span class="sxs-lookup"><span data-stu-id="5cfba-114">actionState</span></span>|[<span data-ttu-id="5cfba-115">actionState</span><span class="sxs-lookup"><span data-stu-id="5cfba-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="5cfba-116">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="5cfba-116">State of the action.</span></span> <span data-ttu-id="5cfba-117">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="5cfba-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5cfba-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5cfba-118">startDateTime</span></span>|<span data-ttu-id="5cfba-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cfba-119">DateTimeOffset</span></span>|<span data-ttu-id="5cfba-120">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="5cfba-120">Time the action was initiated</span></span>|
|<span data-ttu-id="5cfba-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cfba-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="5cfba-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cfba-122">DateTimeOffset</span></span>|<span data-ttu-id="5cfba-123">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="5cfba-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cfba-124">关系</span><span class="sxs-lookup"><span data-stu-id="5cfba-124">Relationships</span></span>
<span data-ttu-id="5cfba-125">无</span><span class="sxs-lookup"><span data-stu-id="5cfba-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cfba-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5cfba-126">JSON Representation</span></span>
<span data-ttu-id="5cfba-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cfba-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




