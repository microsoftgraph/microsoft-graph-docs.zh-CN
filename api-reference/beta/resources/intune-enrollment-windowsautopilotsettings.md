---
title: windowsAutopilotSettings 资源类型
description: WindowsAutopilotSettings 资源表示用于将数据与 Windows 设备数据同步服务同步的 Windows Autopilot 帐户。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d5f7893b7a9dd01a3ea7c41875f235870a5ce27f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941434"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="3d724-103">windowsAutopilotSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d724-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="3d724-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3d724-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d724-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d724-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d724-106">WindowsAutopilotSettings 资源表示用于将数据与 Windows 设备数据同步服务同步的 Windows Autopilot 帐户。</span><span class="sxs-lookup"><span data-stu-id="3d724-106">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="3d724-107">方法</span><span class="sxs-lookup"><span data-stu-id="3d724-107">Methods</span></span>
|<span data-ttu-id="3d724-108">方法</span><span class="sxs-lookup"><span data-stu-id="3d724-108">Method</span></span>|<span data-ttu-id="3d724-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="3d724-109">Return Type</span></span>|<span data-ttu-id="3d724-110">说明</span><span class="sxs-lookup"><span data-stu-id="3d724-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3d724-111">获取 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="3d724-111">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="3d724-112">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="3d724-112">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="3d724-113">读取[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3d724-113">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="3d724-114">更新 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="3d724-114">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="3d724-115">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="3d724-115">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="3d724-116">更新[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3d724-116">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="3d724-117">同步操作</span><span class="sxs-lookup"><span data-stu-id="3d724-117">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="3d724-118">无</span><span class="sxs-lookup"><span data-stu-id="3d724-118">None</span></span>|<span data-ttu-id="3d724-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3d724-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3d724-120">属性</span><span class="sxs-lookup"><span data-stu-id="3d724-120">Properties</span></span>
|<span data-ttu-id="3d724-121">属性</span><span class="sxs-lookup"><span data-stu-id="3d724-121">Property</span></span>|<span data-ttu-id="3d724-122">类型</span><span class="sxs-lookup"><span data-stu-id="3d724-122">Type</span></span>|<span data-ttu-id="3d724-123">说明</span><span class="sxs-lookup"><span data-stu-id="3d724-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d724-124">id</span><span class="sxs-lookup"><span data-stu-id="3d724-124">id</span></span>|<span data-ttu-id="3d724-125">String</span><span class="sxs-lookup"><span data-stu-id="3d724-125">String</span></span>|<span data-ttu-id="3d724-126">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="3d724-126">The GUID for the object</span></span>|
|<span data-ttu-id="3d724-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3d724-127">lastSyncDateTime</span></span>|<span data-ttu-id="3d724-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d724-128">DateTimeOffset</span></span>|<span data-ttu-id="3d724-129">包含 DDS 服务的上次数据同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="3d724-129">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="3d724-130">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="3d724-130">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="3d724-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d724-131">DateTimeOffset</span></span>|<span data-ttu-id="3d724-132">包含 DDS 服务的上次数据同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="3d724-132">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="3d724-133">syncStatus</span><span class="sxs-lookup"><span data-stu-id="3d724-133">syncStatus</span></span>|[<span data-ttu-id="3d724-134">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="3d724-134">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="3d724-135">指示与设备数据同步 (DDS) 服务同步的状态。</span><span class="sxs-lookup"><span data-stu-id="3d724-135">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="3d724-136">可取值为：`unknown`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="3d724-136">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d724-137">关系</span><span class="sxs-lookup"><span data-stu-id="3d724-137">Relationships</span></span>
<span data-ttu-id="3d724-138">无</span><span class="sxs-lookup"><span data-stu-id="3d724-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d724-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d724-139">JSON Representation</span></span>
<span data-ttu-id="3d724-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d724-140">Here is a JSON representation of the resource.</span></span>
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




