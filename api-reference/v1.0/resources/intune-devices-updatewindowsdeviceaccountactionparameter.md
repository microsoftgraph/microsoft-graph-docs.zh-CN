---
title: updateWindowsDeviceAccountActionParameter 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 27007548c0d17351502e9ede3b8070afa52d6d80
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030658"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="908f1-103">updateWindowsDeviceAccountActionParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="908f1-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="908f1-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="908f1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="908f1-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="908f1-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="908f1-106">属性</span><span class="sxs-lookup"><span data-stu-id="908f1-106">Properties</span></span>
|<span data-ttu-id="908f1-107">属性</span><span class="sxs-lookup"><span data-stu-id="908f1-107">Property</span></span>|<span data-ttu-id="908f1-108">类型</span><span class="sxs-lookup"><span data-stu-id="908f1-108">Type</span></span>|<span data-ttu-id="908f1-109">说明</span><span class="sxs-lookup"><span data-stu-id="908f1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="908f1-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="908f1-110">deviceAccount</span></span>|[<span data-ttu-id="908f1-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="908f1-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="908f1-112">尚未记录</span><span class="sxs-lookup"><span data-stu-id="908f1-112">Not yet documented</span></span>|
|<span data-ttu-id="908f1-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="908f1-113">passwordRotationEnabled</span></span>|<span data-ttu-id="908f1-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="908f1-114">Boolean</span></span>|<span data-ttu-id="908f1-115">尚未记录</span><span class="sxs-lookup"><span data-stu-id="908f1-115">Not yet documented</span></span>|
|<span data-ttu-id="908f1-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="908f1-116">calendarSyncEnabled</span></span>|<span data-ttu-id="908f1-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="908f1-117">Boolean</span></span>|<span data-ttu-id="908f1-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="908f1-118">Not yet documented</span></span>|
|<span data-ttu-id="908f1-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="908f1-119">deviceAccountEmail</span></span>|<span data-ttu-id="908f1-120">String</span><span class="sxs-lookup"><span data-stu-id="908f1-120">String</span></span>|<span data-ttu-id="908f1-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="908f1-121">Not yet documented</span></span>|
|<span data-ttu-id="908f1-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="908f1-122">exchangeServer</span></span>|<span data-ttu-id="908f1-123">String</span><span class="sxs-lookup"><span data-stu-id="908f1-123">String</span></span>|<span data-ttu-id="908f1-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="908f1-124">Not yet documented</span></span>|
|<span data-ttu-id="908f1-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="908f1-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="908f1-126">String</span><span class="sxs-lookup"><span data-stu-id="908f1-126">String</span></span>|<span data-ttu-id="908f1-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="908f1-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="908f1-128">关系</span><span class="sxs-lookup"><span data-stu-id="908f1-128">Relationships</span></span>
<span data-ttu-id="908f1-129">无</span><span class="sxs-lookup"><span data-stu-id="908f1-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="908f1-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="908f1-130">JSON Representation</span></span>
<span data-ttu-id="908f1-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="908f1-131">Here is a JSON representation of the resource.</span></span>
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



