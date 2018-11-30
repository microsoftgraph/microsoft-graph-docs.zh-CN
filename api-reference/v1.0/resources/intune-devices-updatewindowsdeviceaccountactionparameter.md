---
title: updateWindowsDeviceAccountActionParameter 资源类型
description: 尚未记录
ms.openlocfilehash: f6403e4c3b106b318b7d551796911f6bcc0253c2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010041"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="b529b-103">updateWindowsDeviceAccountActionParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="b529b-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="b529b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b529b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b529b-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b529b-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b529b-106">属性</span><span class="sxs-lookup"><span data-stu-id="b529b-106">Properties</span></span>
|<span data-ttu-id="b529b-107">属性</span><span class="sxs-lookup"><span data-stu-id="b529b-107">Property</span></span>|<span data-ttu-id="b529b-108">类型</span><span class="sxs-lookup"><span data-stu-id="b529b-108">Type</span></span>|<span data-ttu-id="b529b-109">说明</span><span class="sxs-lookup"><span data-stu-id="b529b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b529b-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="b529b-110">deviceAccount</span></span>|[<span data-ttu-id="b529b-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="b529b-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="b529b-112">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b529b-112">Not yet documented</span></span>|
|<span data-ttu-id="b529b-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="b529b-113">passwordRotationEnabled</span></span>|<span data-ttu-id="b529b-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="b529b-114">Boolean</span></span>|<span data-ttu-id="b529b-115">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b529b-115">Not yet documented</span></span>|
|<span data-ttu-id="b529b-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="b529b-116">calendarSyncEnabled</span></span>|<span data-ttu-id="b529b-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="b529b-117">Boolean</span></span>|<span data-ttu-id="b529b-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b529b-118">Not yet documented</span></span>|
|<span data-ttu-id="b529b-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="b529b-119">deviceAccountEmail</span></span>|<span data-ttu-id="b529b-120">String</span><span class="sxs-lookup"><span data-stu-id="b529b-120">String</span></span>|<span data-ttu-id="b529b-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b529b-121">Not yet documented</span></span>|
|<span data-ttu-id="b529b-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="b529b-122">exchangeServer</span></span>|<span data-ttu-id="b529b-123">String</span><span class="sxs-lookup"><span data-stu-id="b529b-123">String</span></span>|<span data-ttu-id="b529b-124">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b529b-124">Not yet documented</span></span>|
|<span data-ttu-id="b529b-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="b529b-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="b529b-126">String</span><span class="sxs-lookup"><span data-stu-id="b529b-126">String</span></span>|<span data-ttu-id="b529b-127">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b529b-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="b529b-128">关系</span><span class="sxs-lookup"><span data-stu-id="b529b-128">Relationships</span></span>
<span data-ttu-id="b529b-129">无</span><span class="sxs-lookup"><span data-stu-id="b529b-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b529b-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b529b-130">JSON Representation</span></span>
<span data-ttu-id="b529b-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b529b-131">Here is a JSON representation of the resource.</span></span>
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



