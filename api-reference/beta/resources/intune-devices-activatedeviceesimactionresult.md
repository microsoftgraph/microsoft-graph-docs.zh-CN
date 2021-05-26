---
title: activateDeviceEsimActionResult 资源类型
description: 激活设备 eSIM 操作结果
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3c0a391ee52a84b49e105e90eff57510b8ae1010
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52667006"
---
# <a name="activatedeviceesimactionresult-resource-type"></a><span data-ttu-id="79fab-103">activateDeviceEsimActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="79fab-103">activateDeviceEsimActionResult resource type</span></span>

<span data-ttu-id="79fab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79fab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79fab-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="79fab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79fab-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79fab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79fab-107">激活设备 eSIM 操作结果</span><span class="sxs-lookup"><span data-stu-id="79fab-107">Activate device eSIM action result</span></span>


<span data-ttu-id="79fab-108">继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="79fab-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="79fab-109">属性</span><span class="sxs-lookup"><span data-stu-id="79fab-109">Properties</span></span>
|<span data-ttu-id="79fab-110">属性</span><span class="sxs-lookup"><span data-stu-id="79fab-110">Property</span></span>|<span data-ttu-id="79fab-111">类型</span><span class="sxs-lookup"><span data-stu-id="79fab-111">Type</span></span>|<span data-ttu-id="79fab-112">说明</span><span class="sxs-lookup"><span data-stu-id="79fab-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79fab-113">actionName</span><span class="sxs-lookup"><span data-stu-id="79fab-113">actionName</span></span>|<span data-ttu-id="79fab-114">String</span><span class="sxs-lookup"><span data-stu-id="79fab-114">String</span></span>|<span data-ttu-id="79fab-115">操作名称 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="79fab-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="79fab-116">actionState</span><span class="sxs-lookup"><span data-stu-id="79fab-116">actionState</span></span>|[<span data-ttu-id="79fab-117">actionState</span><span class="sxs-lookup"><span data-stu-id="79fab-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="79fab-118">操作的状态 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)。</span><span class="sxs-lookup"><span data-stu-id="79fab-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="79fab-119">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="79fab-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="79fab-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="79fab-120">startDateTime</span></span>|<span data-ttu-id="79fab-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79fab-121">DateTimeOffset</span></span>|<span data-ttu-id="79fab-122">操作启动的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="79fab-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="79fab-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="79fab-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="79fab-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79fab-124">DateTimeOffset</span></span>|<span data-ttu-id="79fab-125">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="79fab-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="79fab-126">carrierUrl</span><span class="sxs-lookup"><span data-stu-id="79fab-126">carrierUrl</span></span>|<span data-ttu-id="79fab-127">String</span><span class="sxs-lookup"><span data-stu-id="79fab-127">String</span></span>|<span data-ttu-id="79fab-128">用于激活设备 eSIM 的运营商 URL</span><span class="sxs-lookup"><span data-stu-id="79fab-128">Carrier Url to activate the device eSIM</span></span> |

## <a name="relationships"></a><span data-ttu-id="79fab-129">关系</span><span class="sxs-lookup"><span data-stu-id="79fab-129">Relationships</span></span>
<span data-ttu-id="79fab-130">无</span><span class="sxs-lookup"><span data-stu-id="79fab-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79fab-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79fab-131">JSON Representation</span></span>
<span data-ttu-id="79fab-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79fab-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.activateDeviceEsimActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.activateDeviceEsimActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "carrierUrl": "String"
}
```




