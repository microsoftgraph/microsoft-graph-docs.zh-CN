---
title: vppTokenActionResult 资源类型
description: 使用 Apple Volume Purchase Program 令牌执行的操作的状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0cc4856901af4f97fde87acc57916742a27186ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029349"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="d0139-103">vppTokenActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0139-103">vppTokenActionResult resource type</span></span>

<span data-ttu-id="d0139-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0139-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0139-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d0139-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0139-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0139-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0139-107">使用 Apple Volume Purchase Program 令牌执行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="d0139-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="d0139-108">属性</span><span class="sxs-lookup"><span data-stu-id="d0139-108">Properties</span></span>
|<span data-ttu-id="d0139-109">属性</span><span class="sxs-lookup"><span data-stu-id="d0139-109">Property</span></span>|<span data-ttu-id="d0139-110">类型</span><span class="sxs-lookup"><span data-stu-id="d0139-110">Type</span></span>|<span data-ttu-id="d0139-111">说明</span><span class="sxs-lookup"><span data-stu-id="d0139-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0139-112">actionName</span><span class="sxs-lookup"><span data-stu-id="d0139-112">actionName</span></span>|<span data-ttu-id="d0139-113">String</span><span class="sxs-lookup"><span data-stu-id="d0139-113">String</span></span>|<span data-ttu-id="d0139-114">操作名</span><span class="sxs-lookup"><span data-stu-id="d0139-114">Action name</span></span>|
|<span data-ttu-id="d0139-115">actionState</span><span class="sxs-lookup"><span data-stu-id="d0139-115">actionState</span></span>|[<span data-ttu-id="d0139-116">actionState</span><span class="sxs-lookup"><span data-stu-id="d0139-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d0139-117">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="d0139-117">State of the action.</span></span> <span data-ttu-id="d0139-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="d0139-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d0139-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d0139-119">startDateTime</span></span>|<span data-ttu-id="d0139-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0139-120">DateTimeOffset</span></span>|<span data-ttu-id="d0139-121">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="d0139-121">Time the action was initiated</span></span>|
|<span data-ttu-id="d0139-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0139-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="d0139-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0139-123">DateTimeOffset</span></span>|<span data-ttu-id="d0139-124">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="d0139-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0139-125">关系</span><span class="sxs-lookup"><span data-stu-id="d0139-125">Relationships</span></span>
<span data-ttu-id="d0139-126">无</span><span class="sxs-lookup"><span data-stu-id="d0139-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0139-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0139-127">JSON Representation</span></span>
<span data-ttu-id="d0139-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0139-128">Here is a JSON representation of the resource.</span></span>
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






