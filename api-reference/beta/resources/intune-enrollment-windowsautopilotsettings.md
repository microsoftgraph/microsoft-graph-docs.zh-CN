---
title: windowsAutopilotSettings 资源类型
description: windowsAutopilotSettings 资源表示用于将数据与 windows 设备数据同步服务同步的 Windows Autopilot 帐户。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b34d6edbed5bc98989ea70186b081d5c88a1c1b6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140514"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="34b69-103">windowsAutopilotSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="34b69-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="34b69-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34b69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34b69-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34b69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34b69-106">windowsAutopilotSettings 资源表示用于将数据与 windows 设备数据同步服务同步的 Windows Autopilot 帐户。</span><span class="sxs-lookup"><span data-stu-id="34b69-106">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="34b69-107">方法</span><span class="sxs-lookup"><span data-stu-id="34b69-107">Methods</span></span>
|<span data-ttu-id="34b69-108">方法</span><span class="sxs-lookup"><span data-stu-id="34b69-108">Method</span></span>|<span data-ttu-id="34b69-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="34b69-109">Return Type</span></span>|<span data-ttu-id="34b69-110">说明</span><span class="sxs-lookup"><span data-stu-id="34b69-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="34b69-111">获取 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="34b69-111">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="34b69-112">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="34b69-112">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="34b69-113">读取[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="34b69-113">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="34b69-114">更新 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="34b69-114">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="34b69-115">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="34b69-115">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="34b69-116">更新[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="34b69-116">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="34b69-117">同步操作</span><span class="sxs-lookup"><span data-stu-id="34b69-117">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="34b69-118">无</span><span class="sxs-lookup"><span data-stu-id="34b69-118">None</span></span>|<span data-ttu-id="34b69-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="34b69-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="34b69-120">属性</span><span class="sxs-lookup"><span data-stu-id="34b69-120">Properties</span></span>
|<span data-ttu-id="34b69-121">属性</span><span class="sxs-lookup"><span data-stu-id="34b69-121">Property</span></span>|<span data-ttu-id="34b69-122">类型</span><span class="sxs-lookup"><span data-stu-id="34b69-122">Type</span></span>|<span data-ttu-id="34b69-123">说明</span><span class="sxs-lookup"><span data-stu-id="34b69-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34b69-124">id</span><span class="sxs-lookup"><span data-stu-id="34b69-124">id</span></span>|<span data-ttu-id="34b69-125">字符串</span><span class="sxs-lookup"><span data-stu-id="34b69-125">String</span></span>|<span data-ttu-id="34b69-126">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="34b69-126">The GUID for the object</span></span>|
|<span data-ttu-id="34b69-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="34b69-127">lastSyncDateTime</span></span>|<span data-ttu-id="34b69-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34b69-128">DateTimeOffset</span></span>|<span data-ttu-id="34b69-129">包含 DDS 服务的上次数据同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="34b69-129">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="34b69-130">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="34b69-130">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="34b69-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34b69-131">DateTimeOffset</span></span>|<span data-ttu-id="34b69-132">包含 DDS 服务的上次数据同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="34b69-132">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="34b69-133">syncStatus</span><span class="sxs-lookup"><span data-stu-id="34b69-133">syncStatus</span></span>|[<span data-ttu-id="34b69-134">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="34b69-134">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="34b69-135">指示与设备数据同步 (DDS) 服务同步的状态。</span><span class="sxs-lookup"><span data-stu-id="34b69-135">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="34b69-136">可取值为：`unknown`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="34b69-136">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34b69-137">Relationships</span><span class="sxs-lookup"><span data-stu-id="34b69-137">Relationships</span></span>
<span data-ttu-id="34b69-138">无</span><span class="sxs-lookup"><span data-stu-id="34b69-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34b69-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34b69-139">JSON Representation</span></span>
<span data-ttu-id="34b69-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34b69-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "lastManualSyncTriggerDateTime": "String (timestamp)",
  "syncStatus": "String"
}
```




