---
title: windowsAutopilotSettings 资源类型
description: WindowsAutopilotSettings 资源表示用于将数据与 Windows 设备数据同步服务同步的 Windows Autopilot 帐户。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ceb420946d103ade52dd3ee5c13d007cc76092df
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524565"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="d30e2-103">windowsAutopilotSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d30e2-103">windowsAutopilotSettings resource type</span></span>

<span data-ttu-id="d30e2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d30e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d30e2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d30e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d30e2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d30e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d30e2-107">WindowsAutopilotSettings 资源表示用于将数据与 Windows 设备数据同步服务同步的 Windows Autopilot 帐户。</span><span class="sxs-lookup"><span data-stu-id="d30e2-107">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="d30e2-108">方法</span><span class="sxs-lookup"><span data-stu-id="d30e2-108">Methods</span></span>
|<span data-ttu-id="d30e2-109">方法</span><span class="sxs-lookup"><span data-stu-id="d30e2-109">Method</span></span>|<span data-ttu-id="d30e2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d30e2-110">Return Type</span></span>|<span data-ttu-id="d30e2-111">说明</span><span class="sxs-lookup"><span data-stu-id="d30e2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d30e2-112">获取 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="d30e2-112">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="d30e2-113">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="d30e2-113">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="d30e2-114">读取[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d30e2-114">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="d30e2-115">更新 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="d30e2-115">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="d30e2-116">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="d30e2-116">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="d30e2-117">更新[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d30e2-117">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="d30e2-118">同步操作</span><span class="sxs-lookup"><span data-stu-id="d30e2-118">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="d30e2-119">无</span><span class="sxs-lookup"><span data-stu-id="d30e2-119">None</span></span>|<span data-ttu-id="d30e2-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d30e2-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d30e2-121">属性</span><span class="sxs-lookup"><span data-stu-id="d30e2-121">Properties</span></span>
|<span data-ttu-id="d30e2-122">属性</span><span class="sxs-lookup"><span data-stu-id="d30e2-122">Property</span></span>|<span data-ttu-id="d30e2-123">类型</span><span class="sxs-lookup"><span data-stu-id="d30e2-123">Type</span></span>|<span data-ttu-id="d30e2-124">说明</span><span class="sxs-lookup"><span data-stu-id="d30e2-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d30e2-125">id</span><span class="sxs-lookup"><span data-stu-id="d30e2-125">id</span></span>|<span data-ttu-id="d30e2-126">String</span><span class="sxs-lookup"><span data-stu-id="d30e2-126">String</span></span>|<span data-ttu-id="d30e2-127">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="d30e2-127">The GUID for the object</span></span>|
|<span data-ttu-id="d30e2-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d30e2-128">lastSyncDateTime</span></span>|<span data-ttu-id="d30e2-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d30e2-129">DateTimeOffset</span></span>|<span data-ttu-id="d30e2-130">包含 DDS 服务的上次数据同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="d30e2-130">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="d30e2-131">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="d30e2-131">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="d30e2-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d30e2-132">DateTimeOffset</span></span>|<span data-ttu-id="d30e2-133">包含 DDS 服务的上次数据同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="d30e2-133">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="d30e2-134">syncStatus</span><span class="sxs-lookup"><span data-stu-id="d30e2-134">syncStatus</span></span>|[<span data-ttu-id="d30e2-135">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="d30e2-135">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="d30e2-136">指示与设备数据同步（DDS）服务同步的状态。</span><span class="sxs-lookup"><span data-stu-id="d30e2-136">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="d30e2-137">可取值为：`unknown`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="d30e2-137">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d30e2-138">关系</span><span class="sxs-lookup"><span data-stu-id="d30e2-138">Relationships</span></span>
<span data-ttu-id="d30e2-139">无</span><span class="sxs-lookup"><span data-stu-id="d30e2-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d30e2-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d30e2-140">JSON Representation</span></span>
<span data-ttu-id="d30e2-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d30e2-141">Here is a JSON representation of the resource.</span></span>
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



