---
title: vppTokenActionResult 资源类型
description: 使用 Apple 卷购买计划令牌执行操作的状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2fb78ea991ed43bd100a424ea7ddd7e23b22412d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414289"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="4ca8f-103">vppTokenActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ca8f-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="4ca8f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4ca8f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4ca8f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4ca8f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ca8f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ca8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ca8f-107">使用 Apple 卷购买计划令牌执行操作的状态。</span><span class="sxs-lookup"><span data-stu-id="4ca8f-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="4ca8f-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ca8f-108">Properties</span></span>
|<span data-ttu-id="4ca8f-109">属性</span><span class="sxs-lookup"><span data-stu-id="4ca8f-109">Property</span></span>|<span data-ttu-id="4ca8f-110">类型</span><span class="sxs-lookup"><span data-stu-id="4ca8f-110">Type</span></span>|<span data-ttu-id="4ca8f-111">说明</span><span class="sxs-lookup"><span data-stu-id="4ca8f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ca8f-112">actionName</span><span class="sxs-lookup"><span data-stu-id="4ca8f-112">actionName</span></span>|<span data-ttu-id="4ca8f-113">String</span><span class="sxs-lookup"><span data-stu-id="4ca8f-113">String</span></span>|<span data-ttu-id="4ca8f-114">操作名</span><span class="sxs-lookup"><span data-stu-id="4ca8f-114">Action name</span></span>|
|<span data-ttu-id="4ca8f-115">actionState</span><span class="sxs-lookup"><span data-stu-id="4ca8f-115">actionState</span></span>|[<span data-ttu-id="4ca8f-116">actionState</span><span class="sxs-lookup"><span data-stu-id="4ca8f-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4ca8f-117">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="4ca8f-117">State of the action.</span></span> <span data-ttu-id="4ca8f-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="4ca8f-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4ca8f-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4ca8f-119">startDateTime</span></span>|<span data-ttu-id="4ca8f-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ca8f-120">DateTimeOffset</span></span>|<span data-ttu-id="4ca8f-121">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="4ca8f-121">Time the action was initiated</span></span>|
|<span data-ttu-id="4ca8f-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ca8f-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="4ca8f-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ca8f-123">DateTimeOffset</span></span>|<span data-ttu-id="4ca8f-124">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="4ca8f-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ca8f-125">关系</span><span class="sxs-lookup"><span data-stu-id="4ca8f-125">Relationships</span></span>
<span data-ttu-id="4ca8f-126">无</span><span class="sxs-lookup"><span data-stu-id="4ca8f-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ca8f-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ca8f-127">JSON Representation</span></span>
<span data-ttu-id="4ca8f-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ca8f-128">Here is a JSON representation of the resource.</span></span>
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




