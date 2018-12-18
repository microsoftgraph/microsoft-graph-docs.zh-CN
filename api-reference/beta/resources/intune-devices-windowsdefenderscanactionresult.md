---
title: windowsDefenderScanActionResult 资源类型
description: Windows Defender 最后扫描结果
author: tfitzmac
ms.openlocfilehash: fa988a971925cf61db0ab9f7e962162565e8a4b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323035"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="4e59f-103">windowsDefenderScanActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e59f-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="4e59f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4e59f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e59f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4e59f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e59f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4e59f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e59f-107">Windows Defender 最后扫描结果</span><span class="sxs-lookup"><span data-stu-id="4e59f-107">Windows Defender last scan result</span></span>

<span data-ttu-id="4e59f-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4e59f-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4e59f-109">属性</span><span class="sxs-lookup"><span data-stu-id="4e59f-109">Properties</span></span>
|<span data-ttu-id="4e59f-110">属性</span><span class="sxs-lookup"><span data-stu-id="4e59f-110">Property</span></span>|<span data-ttu-id="4e59f-111">类型</span><span class="sxs-lookup"><span data-stu-id="4e59f-111">Type</span></span>|<span data-ttu-id="4e59f-112">说明</span><span class="sxs-lookup"><span data-stu-id="4e59f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e59f-113">actionName</span><span class="sxs-lookup"><span data-stu-id="4e59f-113">actionName</span></span>|<span data-ttu-id="4e59f-114">String</span><span class="sxs-lookup"><span data-stu-id="4e59f-114">String</span></span>|<span data-ttu-id="4e59f-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4e59f-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4e59f-116">actionState</span><span class="sxs-lookup"><span data-stu-id="4e59f-116">actionState</span></span>|[<span data-ttu-id="4e59f-117">actionState</span><span class="sxs-lookup"><span data-stu-id="4e59f-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4e59f-118">从[deviceActionResult](../resources/intune-devices-deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="4e59f-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="4e59f-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="4e59f-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4e59f-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4e59f-120">startDateTime</span></span>|<span data-ttu-id="4e59f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e59f-121">DateTimeOffset</span></span>|<span data-ttu-id="4e59f-122">启动操作的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4e59f-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4e59f-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e59f-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="4e59f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e59f-124">DateTimeOffset</span></span>|<span data-ttu-id="4e59f-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4e59f-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4e59f-126">scanType</span><span class="sxs-lookup"><span data-stu-id="4e59f-126">scanType</span></span>|<span data-ttu-id="4e59f-127">String</span><span class="sxs-lookup"><span data-stu-id="4e59f-127">String</span></span>|<span data-ttu-id="4e59f-128">扫描类型（完全扫描或快速扫描）</span><span class="sxs-lookup"><span data-stu-id="4e59f-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e59f-129">关系</span><span class="sxs-lookup"><span data-stu-id="4e59f-129">Relationships</span></span>
<span data-ttu-id="4e59f-130">无</span><span class="sxs-lookup"><span data-stu-id="4e59f-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4e59f-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e59f-131">JSON Representation</span></span>
<span data-ttu-id="4e59f-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e59f-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```





