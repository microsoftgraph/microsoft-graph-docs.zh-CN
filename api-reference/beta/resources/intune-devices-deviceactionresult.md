---
title: deviceActionResult 资源类型
description: 设备操作结果
author: tfitzmac
ms.openlocfilehash: fd2160c501820ec04a94b618b3456a3f8fafa6cd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324946"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="8286e-103">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="8286e-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="8286e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8286e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8286e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8286e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8286e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8286e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8286e-107">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="8286e-107">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="8286e-108">属性</span><span class="sxs-lookup"><span data-stu-id="8286e-108">Properties</span></span>
|<span data-ttu-id="8286e-109">属性</span><span class="sxs-lookup"><span data-stu-id="8286e-109">Property</span></span>|<span data-ttu-id="8286e-110">类型</span><span class="sxs-lookup"><span data-stu-id="8286e-110">Type</span></span>|<span data-ttu-id="8286e-111">说明</span><span class="sxs-lookup"><span data-stu-id="8286e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8286e-112">actionName</span><span class="sxs-lookup"><span data-stu-id="8286e-112">actionName</span></span>|<span data-ttu-id="8286e-113">String</span><span class="sxs-lookup"><span data-stu-id="8286e-113">String</span></span>|<span data-ttu-id="8286e-114">操作名</span><span class="sxs-lookup"><span data-stu-id="8286e-114">Action name</span></span>|
|<span data-ttu-id="8286e-115">actionState</span><span class="sxs-lookup"><span data-stu-id="8286e-115">actionState</span></span>|[<span data-ttu-id="8286e-116">actionState</span><span class="sxs-lookup"><span data-stu-id="8286e-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="8286e-117">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="8286e-117">State of the action.</span></span> <span data-ttu-id="8286e-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="8286e-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="8286e-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8286e-119">startDateTime</span></span>|<span data-ttu-id="8286e-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8286e-120">DateTimeOffset</span></span>|<span data-ttu-id="8286e-121">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="8286e-121">Time the action was initiated</span></span>|
|<span data-ttu-id="8286e-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8286e-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="8286e-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8286e-123">DateTimeOffset</span></span>|<span data-ttu-id="8286e-124">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="8286e-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="8286e-125">关系</span><span class="sxs-lookup"><span data-stu-id="8286e-125">Relationships</span></span>
<span data-ttu-id="8286e-126">无</span><span class="sxs-lookup"><span data-stu-id="8286e-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8286e-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8286e-127">JSON Representation</span></span>
<span data-ttu-id="8286e-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8286e-128">Here is a JSON representation of the resource.</span></span>
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





