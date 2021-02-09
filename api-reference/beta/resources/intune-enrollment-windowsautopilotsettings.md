---
title: windowsAutopilotSettings 资源类型
description: windowsAutopilotSettings 资源表示一个 Windows Autopilot 帐户，用于将数据与 Windows 设备数据同步服务同步。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e49191d204a040327c510606c6ca8186644beb7
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159526"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="ebb87-103">windowsAutopilotSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="ebb87-103">windowsAutopilotSettings resource type</span></span>

<span data-ttu-id="ebb87-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebb87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebb87-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ebb87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebb87-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ebb87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebb87-107">windowsAutopilotSettings 资源表示一个 Windows Autopilot 帐户，用于将数据与 Windows 设备数据同步服务同步。</span><span class="sxs-lookup"><span data-stu-id="ebb87-107">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="ebb87-108">方法</span><span class="sxs-lookup"><span data-stu-id="ebb87-108">Methods</span></span>
|<span data-ttu-id="ebb87-109">方法</span><span class="sxs-lookup"><span data-stu-id="ebb87-109">Method</span></span>|<span data-ttu-id="ebb87-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ebb87-110">Return Type</span></span>|<span data-ttu-id="ebb87-111">说明</span><span class="sxs-lookup"><span data-stu-id="ebb87-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ebb87-112">获取 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="ebb87-112">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="ebb87-113">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="ebb87-113">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="ebb87-114">读取 [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ebb87-114">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="ebb87-115">更新 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="ebb87-115">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="ebb87-116">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="ebb87-116">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="ebb87-117">更新 [windowsAutopilotSettings 对象](../resources/intune-enrollment-windowsautopilotsettings.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="ebb87-117">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="ebb87-118">同步操作</span><span class="sxs-lookup"><span data-stu-id="ebb87-118">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="ebb87-119">无</span><span class="sxs-lookup"><span data-stu-id="ebb87-119">None</span></span>|<span data-ttu-id="ebb87-120">从适用于企业应用商店和其他门户启动所有 AutoPilot 注册设备的同步。</span><span class="sxs-lookup"><span data-stu-id="ebb87-120">Initiates a sync of all AutoPilot registered devices from Store for Business and other portals.</span></span> <span data-ttu-id="ebb87-121">如果同步成功，此操作将返回"204 无内容"响应代码。</span><span class="sxs-lookup"><span data-stu-id="ebb87-121">If the sync successful, this action returns a 204 No Content response code.</span></span> <span data-ttu-id="ebb87-122">如果同步正在进行，该操作将返回 409 冲突响应代码。</span><span class="sxs-lookup"><span data-stu-id="ebb87-122">If a sync is already in progress, the action returns a 409 Conflict response code.</span></span>  <span data-ttu-id="ebb87-123">如果在上一个同步的 10 分钟内调用此同步操作，该操作将返回 429"请求过多"响应代码。</span><span class="sxs-lookup"><span data-stu-id="ebb87-123">If this sync action is called within 10 minutes of the previous sync, the action returns a 429 Too Many Requests response code.</span></span>|

## <a name="properties"></a><span data-ttu-id="ebb87-124">属性</span><span class="sxs-lookup"><span data-stu-id="ebb87-124">Properties</span></span>
|<span data-ttu-id="ebb87-125">属性</span><span class="sxs-lookup"><span data-stu-id="ebb87-125">Property</span></span>|<span data-ttu-id="ebb87-126">类型</span><span class="sxs-lookup"><span data-stu-id="ebb87-126">Type</span></span>|<span data-ttu-id="ebb87-127">说明</span><span class="sxs-lookup"><span data-stu-id="ebb87-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebb87-128">id</span><span class="sxs-lookup"><span data-stu-id="ebb87-128">id</span></span>|<span data-ttu-id="ebb87-129">String</span><span class="sxs-lookup"><span data-stu-id="ebb87-129">String</span></span>|<span data-ttu-id="ebb87-130">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="ebb87-130">The GUID for the object</span></span>|
|<span data-ttu-id="ebb87-131">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ebb87-131">lastSyncDateTime</span></span>|<span data-ttu-id="ebb87-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebb87-132">DateTimeOffset</span></span>|<span data-ttu-id="ebb87-133">DDS 服务的上次数据同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="ebb87-133">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="ebb87-134">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="ebb87-134">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="ebb87-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebb87-135">DateTimeOffset</span></span>|<span data-ttu-id="ebb87-136">DDS 服务的上次数据同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="ebb87-136">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="ebb87-137">syncStatus</span><span class="sxs-lookup"><span data-stu-id="ebb87-137">syncStatus</span></span>|[<span data-ttu-id="ebb87-138">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ebb87-138">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="ebb87-139">指示与 DDS 服务的设备数据 (同步) 状态。</span><span class="sxs-lookup"><span data-stu-id="ebb87-139">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="ebb87-140">可取值为：`unknown`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="ebb87-140">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebb87-141">关系</span><span class="sxs-lookup"><span data-stu-id="ebb87-141">Relationships</span></span>
<span data-ttu-id="ebb87-142">无</span><span class="sxs-lookup"><span data-stu-id="ebb87-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebb87-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ebb87-143">JSON Representation</span></span>
<span data-ttu-id="ebb87-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebb87-144">Here is a JSON representation of the resource.</span></span>
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




