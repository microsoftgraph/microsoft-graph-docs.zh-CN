---
title: deviceActionResult 资源类型
description: 设备操作结果
author: tfitzmac
ms.openlocfilehash: 48429e059616d9af0e3cbdac8544e68354b94fb5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320543"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="d2029-103">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2029-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="d2029-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d2029-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2029-105">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="d2029-105">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="d2029-106">属性</span><span class="sxs-lookup"><span data-stu-id="d2029-106">Properties</span></span>
|<span data-ttu-id="d2029-107">属性</span><span class="sxs-lookup"><span data-stu-id="d2029-107">Property</span></span>|<span data-ttu-id="d2029-108">类型</span><span class="sxs-lookup"><span data-stu-id="d2029-108">Type</span></span>|<span data-ttu-id="d2029-109">说明</span><span class="sxs-lookup"><span data-stu-id="d2029-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2029-110">actionName</span><span class="sxs-lookup"><span data-stu-id="d2029-110">actionName</span></span>|<span data-ttu-id="d2029-111">String</span><span class="sxs-lookup"><span data-stu-id="d2029-111">String</span></span>|<span data-ttu-id="d2029-112">操作名</span><span class="sxs-lookup"><span data-stu-id="d2029-112">Action name</span></span>|
|<span data-ttu-id="d2029-113">actionState</span><span class="sxs-lookup"><span data-stu-id="d2029-113">actionState</span></span>|[<span data-ttu-id="d2029-114">actionState</span><span class="sxs-lookup"><span data-stu-id="d2029-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="d2029-115">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="d2029-115">State of the action.</span></span> <span data-ttu-id="d2029-116">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="d2029-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d2029-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d2029-117">startDateTime</span></span>|<span data-ttu-id="d2029-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2029-118">DateTimeOffset</span></span>|<span data-ttu-id="d2029-119">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="d2029-119">Time the action was initiated</span></span>|
|<span data-ttu-id="d2029-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2029-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="d2029-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2029-121">DateTimeOffset</span></span>|<span data-ttu-id="d2029-122">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="d2029-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2029-123">关系</span><span class="sxs-lookup"><span data-stu-id="d2029-123">Relationships</span></span>
<span data-ttu-id="d2029-124">无</span><span class="sxs-lookup"><span data-stu-id="d2029-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2029-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2029-125">JSON Representation</span></span>
<span data-ttu-id="d2029-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2029-126">Here is a JSON representation of the resource.</span></span>
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



