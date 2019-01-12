---
title: deviceActionResult 资源类型
description: 设备操作结果
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 22fd8e1bc338191bba54ba9f655f03899054ae86
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912300"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="0ef55-103">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ef55-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="0ef55-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0ef55-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ef55-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0ef55-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ef55-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0ef55-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ef55-107">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="0ef55-107">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="0ef55-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ef55-108">Properties</span></span>
|<span data-ttu-id="0ef55-109">属性</span><span class="sxs-lookup"><span data-stu-id="0ef55-109">Property</span></span>|<span data-ttu-id="0ef55-110">类型</span><span class="sxs-lookup"><span data-stu-id="0ef55-110">Type</span></span>|<span data-ttu-id="0ef55-111">说明</span><span class="sxs-lookup"><span data-stu-id="0ef55-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ef55-112">actionName</span><span class="sxs-lookup"><span data-stu-id="0ef55-112">actionName</span></span>|<span data-ttu-id="0ef55-113">String</span><span class="sxs-lookup"><span data-stu-id="0ef55-113">String</span></span>|<span data-ttu-id="0ef55-114">操作名</span><span class="sxs-lookup"><span data-stu-id="0ef55-114">Action name</span></span>|
|<span data-ttu-id="0ef55-115">actionState</span><span class="sxs-lookup"><span data-stu-id="0ef55-115">actionState</span></span>|[<span data-ttu-id="0ef55-116">actionState</span><span class="sxs-lookup"><span data-stu-id="0ef55-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="0ef55-117">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="0ef55-117">State of the action.</span></span> <span data-ttu-id="0ef55-118">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="0ef55-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="0ef55-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0ef55-119">startDateTime</span></span>|<span data-ttu-id="0ef55-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ef55-120">DateTimeOffset</span></span>|<span data-ttu-id="0ef55-121">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="0ef55-121">Time the action was initiated</span></span>|
|<span data-ttu-id="0ef55-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ef55-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="0ef55-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ef55-123">DateTimeOffset</span></span>|<span data-ttu-id="0ef55-124">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="0ef55-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ef55-125">关系</span><span class="sxs-lookup"><span data-stu-id="0ef55-125">Relationships</span></span>
<span data-ttu-id="0ef55-126">无</span><span class="sxs-lookup"><span data-stu-id="0ef55-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0ef55-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ef55-127">JSON Representation</span></span>
<span data-ttu-id="0ef55-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ef55-128">Here is a JSON representation of the resource.</span></span>
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





