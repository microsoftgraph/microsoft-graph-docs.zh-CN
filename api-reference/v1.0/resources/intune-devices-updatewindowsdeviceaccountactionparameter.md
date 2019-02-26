---
title: updateWindowsDeviceAccountActionParameter 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d67599dfc9db2afa337324e3f1ba9334134458f4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256670"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="6117d-103">updateWindowsDeviceAccountActionParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="6117d-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="6117d-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6117d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6117d-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6117d-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6117d-106">属性</span><span class="sxs-lookup"><span data-stu-id="6117d-106">Properties</span></span>
|<span data-ttu-id="6117d-107">属性</span><span class="sxs-lookup"><span data-stu-id="6117d-107">Property</span></span>|<span data-ttu-id="6117d-108">类型</span><span class="sxs-lookup"><span data-stu-id="6117d-108">Type</span></span>|<span data-ttu-id="6117d-109">说明</span><span class="sxs-lookup"><span data-stu-id="6117d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6117d-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="6117d-110">deviceAccount</span></span>|[<span data-ttu-id="6117d-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="6117d-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="6117d-112">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6117d-112">Not yet documented</span></span>|
|<span data-ttu-id="6117d-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="6117d-113">passwordRotationEnabled</span></span>|<span data-ttu-id="6117d-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="6117d-114">Boolean</span></span>|<span data-ttu-id="6117d-115">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6117d-115">Not yet documented</span></span>|
|<span data-ttu-id="6117d-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="6117d-116">calendarSyncEnabled</span></span>|<span data-ttu-id="6117d-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="6117d-117">Boolean</span></span>|<span data-ttu-id="6117d-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6117d-118">Not yet documented</span></span>|
|<span data-ttu-id="6117d-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="6117d-119">deviceAccountEmail</span></span>|<span data-ttu-id="6117d-120">String</span><span class="sxs-lookup"><span data-stu-id="6117d-120">String</span></span>|<span data-ttu-id="6117d-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6117d-121">Not yet documented</span></span>|
|<span data-ttu-id="6117d-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="6117d-122">exchangeServer</span></span>|<span data-ttu-id="6117d-123">String</span><span class="sxs-lookup"><span data-stu-id="6117d-123">String</span></span>|<span data-ttu-id="6117d-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6117d-124">Not yet documented</span></span>|
|<span data-ttu-id="6117d-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="6117d-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="6117d-126">String</span><span class="sxs-lookup"><span data-stu-id="6117d-126">String</span></span>|<span data-ttu-id="6117d-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6117d-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="6117d-128">关系</span><span class="sxs-lookup"><span data-stu-id="6117d-128">Relationships</span></span>
<span data-ttu-id="6117d-129">无</span><span class="sxs-lookup"><span data-stu-id="6117d-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6117d-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6117d-130">JSON Representation</span></span>
<span data-ttu-id="6117d-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6117d-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount",
    "password": "String"
  },
  "passwordRotationEnabled": true,
  "calendarSyncEnabled": true,
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "sessionInitiationProtocalAddress": "String"
}
```



