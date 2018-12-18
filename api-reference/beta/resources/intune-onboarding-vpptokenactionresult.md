---
title: vppTokenActionResult 资源类型
description: 使用 Apple 卷购买计划令牌执行操作的状态。
author: tfitzmac
ms.openlocfilehash: 0b8b074e879321d0aed361373c49e6ed1fd16e62
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341676"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="006e1-103">vppTokenActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="006e1-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="006e1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="006e1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="006e1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="006e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="006e1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="006e1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="006e1-107">使用 Apple 卷购买计划令牌执行操作的状态。</span><span class="sxs-lookup"><span data-stu-id="006e1-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>
## <a name="properties"></a><span data-ttu-id="006e1-108">属性</span><span class="sxs-lookup"><span data-stu-id="006e1-108">Properties</span></span>
|<span data-ttu-id="006e1-109">属性</span><span class="sxs-lookup"><span data-stu-id="006e1-109">Property</span></span>|<span data-ttu-id="006e1-110">类型</span><span class="sxs-lookup"><span data-stu-id="006e1-110">Type</span></span>|<span data-ttu-id="006e1-111">说明</span><span class="sxs-lookup"><span data-stu-id="006e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="006e1-112">actionName</span><span class="sxs-lookup"><span data-stu-id="006e1-112">actionName</span></span>|<span data-ttu-id="006e1-113">String</span><span class="sxs-lookup"><span data-stu-id="006e1-113">String</span></span>|<span data-ttu-id="006e1-114">操作名</span><span class="sxs-lookup"><span data-stu-id="006e1-114">Action name</span></span>|
|<span data-ttu-id="006e1-115">actionState</span><span class="sxs-lookup"><span data-stu-id="006e1-115">actionState</span></span>|[<span data-ttu-id="006e1-116">actionState</span><span class="sxs-lookup"><span data-stu-id="006e1-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="006e1-117">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="006e1-117">State of the action.</span></span> <span data-ttu-id="006e1-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="006e1-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="006e1-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="006e1-119">startDateTime</span></span>|<span data-ttu-id="006e1-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="006e1-120">DateTimeOffset</span></span>|<span data-ttu-id="006e1-121">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="006e1-121">Time the action was initiated</span></span>|
|<span data-ttu-id="006e1-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="006e1-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="006e1-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="006e1-123">DateTimeOffset</span></span>|<span data-ttu-id="006e1-124">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="006e1-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="006e1-125">关系</span><span class="sxs-lookup"><span data-stu-id="006e1-125">Relationships</span></span>
<span data-ttu-id="006e1-126">无</span><span class="sxs-lookup"><span data-stu-id="006e1-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="006e1-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="006e1-127">JSON Representation</span></span>
<span data-ttu-id="006e1-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="006e1-128">Here is a JSON representation of the resource.</span></span>
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





