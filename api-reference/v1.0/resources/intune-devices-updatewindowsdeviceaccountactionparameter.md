---
title: updateWindowsDeviceAccountActionParameter 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d67599dfc9db2afa337324e3f1ba9334134458f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523306"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="f29a8-103">updateWindowsDeviceAccountActionParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="f29a8-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="f29a8-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f29a8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f29a8-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f29a8-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f29a8-106">属性</span><span class="sxs-lookup"><span data-stu-id="f29a8-106">Properties</span></span>
|<span data-ttu-id="f29a8-107">属性</span><span class="sxs-lookup"><span data-stu-id="f29a8-107">Property</span></span>|<span data-ttu-id="f29a8-108">类型</span><span class="sxs-lookup"><span data-stu-id="f29a8-108">Type</span></span>|<span data-ttu-id="f29a8-109">说明</span><span class="sxs-lookup"><span data-stu-id="f29a8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f29a8-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="f29a8-110">deviceAccount</span></span>|[<span data-ttu-id="f29a8-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="f29a8-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="f29a8-112">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f29a8-112">Not yet documented</span></span>|
|<span data-ttu-id="f29a8-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="f29a8-113">passwordRotationEnabled</span></span>|<span data-ttu-id="f29a8-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="f29a8-114">Boolean</span></span>|<span data-ttu-id="f29a8-115">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f29a8-115">Not yet documented</span></span>|
|<span data-ttu-id="f29a8-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="f29a8-116">calendarSyncEnabled</span></span>|<span data-ttu-id="f29a8-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="f29a8-117">Boolean</span></span>|<span data-ttu-id="f29a8-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f29a8-118">Not yet documented</span></span>|
|<span data-ttu-id="f29a8-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="f29a8-119">deviceAccountEmail</span></span>|<span data-ttu-id="f29a8-120">String</span><span class="sxs-lookup"><span data-stu-id="f29a8-120">String</span></span>|<span data-ttu-id="f29a8-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f29a8-121">Not yet documented</span></span>|
|<span data-ttu-id="f29a8-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="f29a8-122">exchangeServer</span></span>|<span data-ttu-id="f29a8-123">String</span><span class="sxs-lookup"><span data-stu-id="f29a8-123">String</span></span>|<span data-ttu-id="f29a8-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f29a8-124">Not yet documented</span></span>|
|<span data-ttu-id="f29a8-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="f29a8-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="f29a8-126">String</span><span class="sxs-lookup"><span data-stu-id="f29a8-126">String</span></span>|<span data-ttu-id="f29a8-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f29a8-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="f29a8-128">关系</span><span class="sxs-lookup"><span data-stu-id="f29a8-128">Relationships</span></span>
<span data-ttu-id="f29a8-129">无</span><span class="sxs-lookup"><span data-stu-id="f29a8-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f29a8-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f29a8-130">JSON Representation</span></span>
<span data-ttu-id="f29a8-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f29a8-131">Here is a JSON representation of the resource.</span></span>
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



