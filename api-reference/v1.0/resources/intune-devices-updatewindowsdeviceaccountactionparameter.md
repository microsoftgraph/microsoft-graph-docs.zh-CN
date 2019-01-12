---
title: updateWindowsDeviceAccountActionParameter 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f62dce1364fca28e85b728e0b7571906488ebbee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986675"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="44ac1-103">updateWindowsDeviceAccountActionParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="44ac1-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="44ac1-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="44ac1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44ac1-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="44ac1-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="44ac1-106">属性</span><span class="sxs-lookup"><span data-stu-id="44ac1-106">Properties</span></span>
|<span data-ttu-id="44ac1-107">属性</span><span class="sxs-lookup"><span data-stu-id="44ac1-107">Property</span></span>|<span data-ttu-id="44ac1-108">类型</span><span class="sxs-lookup"><span data-stu-id="44ac1-108">Type</span></span>|<span data-ttu-id="44ac1-109">说明</span><span class="sxs-lookup"><span data-stu-id="44ac1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44ac1-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="44ac1-110">deviceAccount</span></span>|[<span data-ttu-id="44ac1-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="44ac1-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="44ac1-112">尚未记录</span><span class="sxs-lookup"><span data-stu-id="44ac1-112">Not yet documented</span></span>|
|<span data-ttu-id="44ac1-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="44ac1-113">passwordRotationEnabled</span></span>|<span data-ttu-id="44ac1-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="44ac1-114">Boolean</span></span>|<span data-ttu-id="44ac1-115">尚未记录</span><span class="sxs-lookup"><span data-stu-id="44ac1-115">Not yet documented</span></span>|
|<span data-ttu-id="44ac1-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="44ac1-116">calendarSyncEnabled</span></span>|<span data-ttu-id="44ac1-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="44ac1-117">Boolean</span></span>|<span data-ttu-id="44ac1-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="44ac1-118">Not yet documented</span></span>|
|<span data-ttu-id="44ac1-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="44ac1-119">deviceAccountEmail</span></span>|<span data-ttu-id="44ac1-120">String</span><span class="sxs-lookup"><span data-stu-id="44ac1-120">String</span></span>|<span data-ttu-id="44ac1-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="44ac1-121">Not yet documented</span></span>|
|<span data-ttu-id="44ac1-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="44ac1-122">exchangeServer</span></span>|<span data-ttu-id="44ac1-123">String</span><span class="sxs-lookup"><span data-stu-id="44ac1-123">String</span></span>|<span data-ttu-id="44ac1-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="44ac1-124">Not yet documented</span></span>|
|<span data-ttu-id="44ac1-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="44ac1-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="44ac1-126">String</span><span class="sxs-lookup"><span data-stu-id="44ac1-126">String</span></span>|<span data-ttu-id="44ac1-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="44ac1-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="44ac1-128">关系</span><span class="sxs-lookup"><span data-stu-id="44ac1-128">Relationships</span></span>
<span data-ttu-id="44ac1-129">无</span><span class="sxs-lookup"><span data-stu-id="44ac1-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="44ac1-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44ac1-130">JSON Representation</span></span>
<span data-ttu-id="44ac1-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44ac1-131">Here is a JSON representation of the resource.</span></span>
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



