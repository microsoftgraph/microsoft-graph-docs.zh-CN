---
title: officeClientCheckinStatus 资源类型
description: 介绍租户中签入 stats 的实体。
author: tfitzmac
ms.openlocfilehash: 0c6359d3cb6c776d0f26fdaf88ce7f2f03e5f8c7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331715"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="38629-103">officeClientCheckinStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="38629-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="38629-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="38629-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38629-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="38629-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38629-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="38629-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38629-107">介绍租户中签入 stats 的实体。</span><span class="sxs-lookup"><span data-stu-id="38629-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="38629-108">属性</span><span class="sxs-lookup"><span data-stu-id="38629-108">Properties</span></span>
|<span data-ttu-id="38629-109">属性</span><span class="sxs-lookup"><span data-stu-id="38629-109">Property</span></span>|<span data-ttu-id="38629-110">类型</span><span class="sxs-lookup"><span data-stu-id="38629-110">Type</span></span>|<span data-ttu-id="38629-111">说明</span><span class="sxs-lookup"><span data-stu-id="38629-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38629-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="38629-112">userPrincipalName</span></span>|<span data-ttu-id="38629-113">字符串</span><span class="sxs-lookup"><span data-stu-id="38629-113">String</span></span>|<span data-ttu-id="38629-114">使用设备的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="38629-114">User principal name using the device.</span></span>|
|<span data-ttu-id="38629-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="38629-115">deviceName</span></span>|<span data-ttu-id="38629-116">String</span><span class="sxs-lookup"><span data-stu-id="38629-116">String</span></span>|<span data-ttu-id="38629-117">要签入的设备名称。</span><span class="sxs-lookup"><span data-stu-id="38629-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="38629-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="38629-118">devicePlatform</span></span>|<span data-ttu-id="38629-119">字符串</span><span class="sxs-lookup"><span data-stu-id="38629-119">String</span></span>|<span data-ttu-id="38629-120">要签入的设备平台。</span><span class="sxs-lookup"><span data-stu-id="38629-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="38629-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="38629-121">devicePlatformVersion</span></span>|<span data-ttu-id="38629-122">字符串</span><span class="sxs-lookup"><span data-stu-id="38629-122">String</span></span>|<span data-ttu-id="38629-123">要签入的设备平台版本。</span><span class="sxs-lookup"><span data-stu-id="38629-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="38629-124">准备成功</span><span class="sxs-lookup"><span data-stu-id="38629-124">wasSuccessful</span></span>|<span data-ttu-id="38629-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="38629-125">Boolean</span></span>|<span data-ttu-id="38629-126">如果上次签入已成功。</span><span class="sxs-lookup"><span data-stu-id="38629-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="38629-127">userId</span><span class="sxs-lookup"><span data-stu-id="38629-127">userId</span></span>|<span data-ttu-id="38629-128">String</span><span class="sxs-lookup"><span data-stu-id="38629-128">String</span></span>|<span data-ttu-id="38629-129">使用设备的用户标识符。</span><span class="sxs-lookup"><span data-stu-id="38629-129">User identifier using the device.</span></span>|
|<span data-ttu-id="38629-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="38629-130">checkinDateTime</span></span>|<span data-ttu-id="38629-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38629-131">DateTimeOffset</span></span>|<span data-ttu-id="38629-132">最后一个设备签入时间采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="38629-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="38629-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="38629-133">errorMessage</span></span>|<span data-ttu-id="38629-134">字符串</span><span class="sxs-lookup"><span data-stu-id="38629-134">String</span></span>|<span data-ttu-id="38629-135">如果有关联的最后一个签入的错误消息。</span><span class="sxs-lookup"><span data-stu-id="38629-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="38629-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="38629-136">appliedPolicies</span></span>|<span data-ttu-id="38629-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="38629-137">String collection</span></span>|<span data-ttu-id="38629-138">策略列表送达作为最后一个签入的设备。</span><span class="sxs-lookup"><span data-stu-id="38629-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38629-139">Relationships</span><span class="sxs-lookup"><span data-stu-id="38629-139">Relationships</span></span>
<span data-ttu-id="38629-140">无</span><span class="sxs-lookup"><span data-stu-id="38629-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="38629-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38629-141">JSON Representation</span></span>
<span data-ttu-id="38629-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38629-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
  "userPrincipalName": "String",
  "deviceName": "String",
  "devicePlatform": "String",
  "devicePlatformVersion": "String",
  "wasSuccessful": true,
  "userId": "String",
  "checkinDateTime": "String (timestamp)",
  "errorMessage": "String",
  "appliedPolicies": [
    "String"
  ]
}
```



