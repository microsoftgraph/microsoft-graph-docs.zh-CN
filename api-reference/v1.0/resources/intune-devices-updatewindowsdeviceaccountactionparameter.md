---
title: updateWindowsDeviceAccountActionParameter 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: cd69ffa01473a40228d53ad2f68f793cadf838d5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335460"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="2a379-103">updateWindowsDeviceAccountActionParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a379-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="2a379-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2a379-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a379-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2a379-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2a379-106">属性</span><span class="sxs-lookup"><span data-stu-id="2a379-106">Properties</span></span>
|<span data-ttu-id="2a379-107">属性</span><span class="sxs-lookup"><span data-stu-id="2a379-107">Property</span></span>|<span data-ttu-id="2a379-108">类型</span><span class="sxs-lookup"><span data-stu-id="2a379-108">Type</span></span>|<span data-ttu-id="2a379-109">说明</span><span class="sxs-lookup"><span data-stu-id="2a379-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a379-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="2a379-110">deviceAccount</span></span>|[<span data-ttu-id="2a379-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="2a379-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="2a379-112">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2a379-112">Not yet documented</span></span>|
|<span data-ttu-id="2a379-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="2a379-113">passwordRotationEnabled</span></span>|<span data-ttu-id="2a379-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="2a379-114">Boolean</span></span>|<span data-ttu-id="2a379-115">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2a379-115">Not yet documented</span></span>|
|<span data-ttu-id="2a379-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="2a379-116">calendarSyncEnabled</span></span>|<span data-ttu-id="2a379-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="2a379-117">Boolean</span></span>|<span data-ttu-id="2a379-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2a379-118">Not yet documented</span></span>|
|<span data-ttu-id="2a379-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="2a379-119">deviceAccountEmail</span></span>|<span data-ttu-id="2a379-120">String</span><span class="sxs-lookup"><span data-stu-id="2a379-120">String</span></span>|<span data-ttu-id="2a379-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2a379-121">Not yet documented</span></span>|
|<span data-ttu-id="2a379-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="2a379-122">exchangeServer</span></span>|<span data-ttu-id="2a379-123">String</span><span class="sxs-lookup"><span data-stu-id="2a379-123">String</span></span>|<span data-ttu-id="2a379-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2a379-124">Not yet documented</span></span>|
|<span data-ttu-id="2a379-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="2a379-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="2a379-126">String</span><span class="sxs-lookup"><span data-stu-id="2a379-126">String</span></span>|<span data-ttu-id="2a379-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2a379-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a379-128">关系</span><span class="sxs-lookup"><span data-stu-id="2a379-128">Relationships</span></span>
<span data-ttu-id="2a379-129">无</span><span class="sxs-lookup"><span data-stu-id="2a379-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2a379-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a379-130">JSON Representation</span></span>
<span data-ttu-id="2a379-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a379-131">Here is a JSON representation of the resource.</span></span>
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



