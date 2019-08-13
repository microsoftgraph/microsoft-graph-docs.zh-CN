---
title: windowsAutopilotSettings 资源类型
description: WindowsAutopilotSettings 资源表示用于将数据与 Windows 设备数据同步服务同步的 Windows Autopilot 帐户。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f242bd184737daea34446d345eb39c4c2a9027f7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327680"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="c977f-103">windowsAutopilotSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="c977f-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="c977f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c977f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c977f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c977f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c977f-106">WindowsAutopilotSettings 资源表示用于将数据与 Windows 设备数据同步服务同步的 Windows Autopilot 帐户。</span><span class="sxs-lookup"><span data-stu-id="c977f-106">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="c977f-107">方法</span><span class="sxs-lookup"><span data-stu-id="c977f-107">Methods</span></span>
|<span data-ttu-id="c977f-108">方法</span><span class="sxs-lookup"><span data-stu-id="c977f-108">Method</span></span>|<span data-ttu-id="c977f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c977f-109">Return Type</span></span>|<span data-ttu-id="c977f-110">说明</span><span class="sxs-lookup"><span data-stu-id="c977f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c977f-111">获取 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="c977f-111">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="c977f-112">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="c977f-112">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="c977f-113">读取[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c977f-113">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="c977f-114">更新 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="c977f-114">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="c977f-115">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="c977f-115">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="c977f-116">更新[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c977f-116">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="c977f-117">同步操作</span><span class="sxs-lookup"><span data-stu-id="c977f-117">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="c977f-118">无</span><span class="sxs-lookup"><span data-stu-id="c977f-118">None</span></span>|<span data-ttu-id="c977f-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c977f-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c977f-120">属性</span><span class="sxs-lookup"><span data-stu-id="c977f-120">Properties</span></span>
|<span data-ttu-id="c977f-121">属性</span><span class="sxs-lookup"><span data-stu-id="c977f-121">Property</span></span>|<span data-ttu-id="c977f-122">类型</span><span class="sxs-lookup"><span data-stu-id="c977f-122">Type</span></span>|<span data-ttu-id="c977f-123">说明</span><span class="sxs-lookup"><span data-stu-id="c977f-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c977f-124">id</span><span class="sxs-lookup"><span data-stu-id="c977f-124">id</span></span>|<span data-ttu-id="c977f-125">String</span><span class="sxs-lookup"><span data-stu-id="c977f-125">String</span></span>|<span data-ttu-id="c977f-126">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="c977f-126">The GUID for the object</span></span>|
|<span data-ttu-id="c977f-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c977f-127">lastSyncDateTime</span></span>|<span data-ttu-id="c977f-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c977f-128">DateTimeOffset</span></span>|<span data-ttu-id="c977f-129">包含 DDS 服务的上次数据同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="c977f-129">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="c977f-130">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="c977f-130">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="c977f-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c977f-131">DateTimeOffset</span></span>|<span data-ttu-id="c977f-132">包含 DDS 服务的上次数据同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="c977f-132">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="c977f-133">syncStatus</span><span class="sxs-lookup"><span data-stu-id="c977f-133">syncStatus</span></span>|[<span data-ttu-id="c977f-134">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="c977f-134">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="c977f-135">指示与设备数据同步 (DDS) 服务同步的状态。</span><span class="sxs-lookup"><span data-stu-id="c977f-135">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="c977f-136">可取值为：`unknown`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="c977f-136">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c977f-137">关系</span><span class="sxs-lookup"><span data-stu-id="c977f-137">Relationships</span></span>
<span data-ttu-id="c977f-138">无</span><span class="sxs-lookup"><span data-stu-id="c977f-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c977f-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c977f-139">JSON Representation</span></span>
<span data-ttu-id="c977f-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c977f-140">Here is a JSON representation of the resource.</span></span>
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



