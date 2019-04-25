---
title: deviceActionResult 资源类型
description: 设备操作结果
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d08b4285f81c7b6f7e4962c4738279f84ba37b7d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541974"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="7fff0-103">deviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="7fff0-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="7fff0-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7fff0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fff0-105">设备操作结果</span><span class="sxs-lookup"><span data-stu-id="7fff0-105">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="7fff0-106">属性</span><span class="sxs-lookup"><span data-stu-id="7fff0-106">Properties</span></span>
|<span data-ttu-id="7fff0-107">属性</span><span class="sxs-lookup"><span data-stu-id="7fff0-107">Property</span></span>|<span data-ttu-id="7fff0-108">类型</span><span class="sxs-lookup"><span data-stu-id="7fff0-108">Type</span></span>|<span data-ttu-id="7fff0-109">说明</span><span class="sxs-lookup"><span data-stu-id="7fff0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fff0-110">actionName</span><span class="sxs-lookup"><span data-stu-id="7fff0-110">actionName</span></span>|<span data-ttu-id="7fff0-111">String</span><span class="sxs-lookup"><span data-stu-id="7fff0-111">String</span></span>|<span data-ttu-id="7fff0-112">操作名</span><span class="sxs-lookup"><span data-stu-id="7fff0-112">Action name</span></span>|
|<span data-ttu-id="7fff0-113">actionState</span><span class="sxs-lookup"><span data-stu-id="7fff0-113">actionState</span></span>|[<span data-ttu-id="7fff0-114">actionState</span><span class="sxs-lookup"><span data-stu-id="7fff0-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="7fff0-115">操作的状态。</span><span class="sxs-lookup"><span data-stu-id="7fff0-115">State of the action.</span></span> <span data-ttu-id="7fff0-116">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="7fff0-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7fff0-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7fff0-117">startDateTime</span></span>|<span data-ttu-id="7fff0-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fff0-118">DateTimeOffset</span></span>|<span data-ttu-id="7fff0-119">初始化操作的时间</span><span class="sxs-lookup"><span data-stu-id="7fff0-119">Time the action was initiated</span></span>|
|<span data-ttu-id="7fff0-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7fff0-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="7fff0-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fff0-121">DateTimeOffset</span></span>|<span data-ttu-id="7fff0-122">操作状态上次更新的时间</span><span class="sxs-lookup"><span data-stu-id="7fff0-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fff0-123">关系</span><span class="sxs-lookup"><span data-stu-id="7fff0-123">Relationships</span></span>
<span data-ttu-id="7fff0-124">无</span><span class="sxs-lookup"><span data-stu-id="7fff0-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7fff0-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7fff0-125">JSON Representation</span></span>
<span data-ttu-id="7fff0-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7fff0-126">Here is a JSON representation of the resource.</span></span>
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



