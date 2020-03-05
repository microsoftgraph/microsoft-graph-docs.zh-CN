---
title: vppTokenActionResult 资源类型
description: 使用 Apple Volume Purchase Program 令牌执行的操作的状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f9146b98288a7ed5a7f6de944cc832ddc71f9179
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527695"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="60fe5-103">vppTokenActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="60fe5-103">vppTokenActionResult resource type</span></span>

<span data-ttu-id="60fe5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="60fe5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60fe5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="60fe5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60fe5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="60fe5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60fe5-107">使用 Apple Volume Purchase Program 令牌执行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="60fe5-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="60fe5-108">属性</span><span class="sxs-lookup"><span data-stu-id="60fe5-108">Properties</span></span>
|<span data-ttu-id="60fe5-109">属性</span><span class="sxs-lookup"><span data-stu-id="60fe5-109">Property</span></span>|<span data-ttu-id="60fe5-110">类型</span><span class="sxs-lookup"><span data-stu-id="60fe5-110">Type</span></span>|<span data-ttu-id="60fe5-111">说明</span><span class="sxs-lookup"><span data-stu-id="60fe5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60fe5-112">actionName</span><span class="sxs-lookup"><span data-stu-id="60fe5-112">actionName</span></span>|<span data-ttu-id="60fe5-113">String</span><span class="sxs-lookup"><span data-stu-id="60fe5-113">String</span></span>|<span data-ttu-id="60fe5-114">操作名</span><span class="sxs-lookup"><span data-stu-id="60fe5-114">Action name</span></span>|
|<span data-ttu-id="60fe5-115">actionState</span><span class="sxs-lookup"><span data-stu-id="60fe5-115">actionState</span></span>|[<span data-ttu-id="60fe5-116">actionState</span><span class="sxs-lookup"><span data-stu-id="60fe5-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="60fe5-117">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="60fe5-117">State of the action.</span></span> <span data-ttu-id="60fe5-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="60fe5-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="60fe5-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="60fe5-119">startDateTime</span></span>|<span data-ttu-id="60fe5-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60fe5-120">DateTimeOffset</span></span>|<span data-ttu-id="60fe5-121">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="60fe5-121">Time the action was initiated</span></span>|
|<span data-ttu-id="60fe5-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="60fe5-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="60fe5-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60fe5-123">DateTimeOffset</span></span>|<span data-ttu-id="60fe5-124">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="60fe5-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="60fe5-125">关系</span><span class="sxs-lookup"><span data-stu-id="60fe5-125">Relationships</span></span>
<span data-ttu-id="60fe5-126">无</span><span class="sxs-lookup"><span data-stu-id="60fe5-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60fe5-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60fe5-127">JSON Representation</span></span>
<span data-ttu-id="60fe5-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60fe5-128">Here is a JSON representation of the resource.</span></span>
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



