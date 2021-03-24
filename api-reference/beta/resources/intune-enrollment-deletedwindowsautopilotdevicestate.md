---
title: deletedWindowsAutopilotDeviceState 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 87113449f0c00722f3aa1d3a1e614873524d43a6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146753"
---
# <a name="deletedwindowsautopilotdevicestate-resource-type"></a><span data-ttu-id="53bf0-103">deletedWindowsAutopilotDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="53bf0-103">deletedWindowsAutopilotDeviceState resource type</span></span>

<span data-ttu-id="53bf0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53bf0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53bf0-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="53bf0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53bf0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53bf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53bf0-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="53bf0-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="53bf0-108">属性</span><span class="sxs-lookup"><span data-stu-id="53bf0-108">Properties</span></span>
|<span data-ttu-id="53bf0-109">属性</span><span class="sxs-lookup"><span data-stu-id="53bf0-109">Property</span></span>|<span data-ttu-id="53bf0-110">类型</span><span class="sxs-lookup"><span data-stu-id="53bf0-110">Type</span></span>|<span data-ttu-id="53bf0-111">说明</span><span class="sxs-lookup"><span data-stu-id="53bf0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53bf0-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="53bf0-112">serialNumber</span></span>|<span data-ttu-id="53bf0-113">String</span><span class="sxs-lookup"><span data-stu-id="53bf0-113">String</span></span>|<span data-ttu-id="53bf0-114">Autopilot 设备序列号</span><span class="sxs-lookup"><span data-stu-id="53bf0-114">Autopilot Device Serial Number</span></span>|
|<span data-ttu-id="53bf0-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="53bf0-115">deviceRegistrationId</span></span>|<span data-ttu-id="53bf0-116">字符串</span><span class="sxs-lookup"><span data-stu-id="53bf0-116">String</span></span>|<span data-ttu-id="53bf0-117">ZTD 设备注册 ID 。</span><span class="sxs-lookup"><span data-stu-id="53bf0-117">ZTD Device Registration ID .</span></span>|
|<span data-ttu-id="53bf0-118">deletionState</span><span class="sxs-lookup"><span data-stu-id="53bf0-118">deletionState</span></span>|[<span data-ttu-id="53bf0-119">windowsAutopilotDeviceDeletionState</span><span class="sxs-lookup"><span data-stu-id="53bf0-119">windowsAutopilotDeviceDeletionState</span></span>](../resources/intune-enrollment-windowsautopilotdevicedeletionstate.md)|<span data-ttu-id="53bf0-120">设备删除状态。</span><span class="sxs-lookup"><span data-stu-id="53bf0-120">Device deletion state.</span></span> <span data-ttu-id="53bf0-121">可取值为：`unknown`、`failed`、`accepted`、`error`。</span><span class="sxs-lookup"><span data-stu-id="53bf0-121">Possible values are: `unknown`, `failed`, `accepted`, `error`.</span></span>|
|<span data-ttu-id="53bf0-122">errorMessage</span><span class="sxs-lookup"><span data-stu-id="53bf0-122">errorMessage</span></span>|<span data-ttu-id="53bf0-123">String</span><span class="sxs-lookup"><span data-stu-id="53bf0-123">String</span></span>|<span data-ttu-id="53bf0-124">设备删除错误消息。</span><span class="sxs-lookup"><span data-stu-id="53bf0-124">Device deletion error message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53bf0-125">关系</span><span class="sxs-lookup"><span data-stu-id="53bf0-125">Relationships</span></span>
<span data-ttu-id="53bf0-126">无</span><span class="sxs-lookup"><span data-stu-id="53bf0-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53bf0-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53bf0-127">JSON Representation</span></span>
<span data-ttu-id="53bf0-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53bf0-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deletedWindowsAutopilotDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deletedWindowsAutopilotDeviceState",
  "serialNumber": "String",
  "deviceRegistrationId": "String",
  "deletionState": "String",
  "errorMessage": "String"
}
```




