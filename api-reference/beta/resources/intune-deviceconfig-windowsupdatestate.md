---
title: windowsUpdateState 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 20387d9e1fd9b84853a7bc097dfa08d128809358
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429486"
---
# <a name="windowsupdatestate-resource-type"></a><span data-ttu-id="83386-103">windowsUpdateState 资源类型</span><span class="sxs-lookup"><span data-stu-id="83386-103">windowsUpdateState resource type</span></span>

> <span data-ttu-id="83386-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="83386-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="83386-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="83386-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83386-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83386-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83386-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="83386-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="83386-108">属性</span><span class="sxs-lookup"><span data-stu-id="83386-108">Properties</span></span>
|<span data-ttu-id="83386-109">属性</span><span class="sxs-lookup"><span data-stu-id="83386-109">Property</span></span>|<span data-ttu-id="83386-110">类型</span><span class="sxs-lookup"><span data-stu-id="83386-110">Type</span></span>|<span data-ttu-id="83386-111">说明</span><span class="sxs-lookup"><span data-stu-id="83386-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83386-112">id</span><span class="sxs-lookup"><span data-stu-id="83386-112">id</span></span>|<span data-ttu-id="83386-113">String</span><span class="sxs-lookup"><span data-stu-id="83386-113">String</span></span>|<span data-ttu-id="83386-114">这是实体的 Id。</span><span class="sxs-lookup"><span data-stu-id="83386-114">This is Id of the entity.</span></span>|
|<span data-ttu-id="83386-115">deviceId</span><span class="sxs-lookup"><span data-stu-id="83386-115">deviceId</span></span>|<span data-ttu-id="83386-116">String</span><span class="sxs-lookup"><span data-stu-id="83386-116">String</span></span>|<span data-ttu-id="83386-117">设备的 id。</span><span class="sxs-lookup"><span data-stu-id="83386-117">The id of the device.</span></span>|
|<span data-ttu-id="83386-118">userId</span><span class="sxs-lookup"><span data-stu-id="83386-118">userId</span></span>|<span data-ttu-id="83386-119">String</span><span class="sxs-lookup"><span data-stu-id="83386-119">String</span></span>|<span data-ttu-id="83386-120">用户的 id。</span><span class="sxs-lookup"><span data-stu-id="83386-120">The id of the user.</span></span>|
|<span data-ttu-id="83386-121">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="83386-121">deviceDisplayName</span></span>|<span data-ttu-id="83386-122">String</span><span class="sxs-lookup"><span data-stu-id="83386-122">String</span></span>|<span data-ttu-id="83386-123">设备的显示名称。</span><span class="sxs-lookup"><span data-stu-id="83386-123">Device display name.</span></span>|
|<span data-ttu-id="83386-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="83386-124">userPrincipalName</span></span>|<span data-ttu-id="83386-125">String</span><span class="sxs-lookup"><span data-stu-id="83386-125">String</span></span>|<span data-ttu-id="83386-126">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="83386-126">User principal name.</span></span>|
|<span data-ttu-id="83386-127">status</span><span class="sxs-lookup"><span data-stu-id="83386-127">status</span></span>|<span data-ttu-id="83386-128">[windowsUpdateStatus](../resources/intune-deviceconfig-windowsupdatestatus.md)</span><span class="sxs-lookup"><span data-stu-id="83386-128">[windowsUpdateStatus] (../resources/intune-deviceconfig-windowsupdatestatus.md)</span></span>|<span data-ttu-id="83386-129">Windows udpate 状态。</span><span class="sxs-lookup"><span data-stu-id="83386-129">Windows udpate status.</span></span>|
|<span data-ttu-id="83386-130">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="83386-130">qualityUpdateVersion</span></span>|<span data-ttu-id="83386-131">String</span><span class="sxs-lookup"><span data-stu-id="83386-131">String</span></span>|<span data-ttu-id="83386-132">设备质量更新版本。</span><span class="sxs-lookup"><span data-stu-id="83386-132">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="83386-133">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="83386-133">featureUpdateVersion</span></span>|<span data-ttu-id="83386-134">String</span><span class="sxs-lookup"><span data-stu-id="83386-134">String</span></span>|<span data-ttu-id="83386-135">设备的当前功能更新版本。</span><span class="sxs-lookup"><span data-stu-id="83386-135">The current feature update version of the device.</span></span>|
|<span data-ttu-id="83386-136">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="83386-136">lastScanDateTime</span></span>|<span data-ttu-id="83386-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83386-137">DateTimeOffset</span></span>|<span data-ttu-id="83386-138">显示日期时间的 Windows Update 代理未成功的扫描。</span><span class="sxs-lookup"><span data-stu-id="83386-138">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="83386-139">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="83386-139">lastSyncDateTime</span></span>|<span data-ttu-id="83386-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83386-140">DateTimeOffset</span></span>|<span data-ttu-id="83386-141">与 Microsoft Intune 与设备同步的最后一个日期时间。</span><span class="sxs-lookup"><span data-stu-id="83386-141">Last date time that the device sync with with Microsoft Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83386-142">关系</span><span class="sxs-lookup"><span data-stu-id="83386-142">Relationships</span></span>
<span data-ttu-id="83386-143">无</span><span class="sxs-lookup"><span data-stu-id="83386-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83386-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83386-144">JSON Representation</span></span>
<span data-ttu-id="83386-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83386-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.WindowsUpdateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.WindowsUpdateState",
  "id": "String (identifier)",
  "deviceId": "String (identifier)",
  "userId": "String (identifier)",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "status": "String",
  "qualityUpdateVersion": "String",
  "featureUpdateVersion": "String",
  "lastScanDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)"
}
```


