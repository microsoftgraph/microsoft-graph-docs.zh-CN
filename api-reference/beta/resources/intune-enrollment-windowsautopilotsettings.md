---
title: windowsAutopilotSettings 资源类型
description: WindowsAutopilotSettings 资源表示为与 Windows 设备数据同步服务的同步数据的 Windows 自动执行某些操作帐户。
ms.openlocfilehash: 41caab7578be08a56ecad94bbae11c43945037c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045515"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="bc225-103">windowsAutopilotSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc225-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="bc225-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bc225-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc225-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bc225-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc225-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bc225-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc225-107">WindowsAutopilotSettings 资源表示为与 Windows 设备数据同步服务的同步数据的 Windows 自动执行某些操作帐户。</span><span class="sxs-lookup"><span data-stu-id="bc225-107">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>
## <a name="methods"></a><span data-ttu-id="bc225-108">方法</span><span class="sxs-lookup"><span data-stu-id="bc225-108">Methods</span></span>
|<span data-ttu-id="bc225-109">方法</span><span class="sxs-lookup"><span data-stu-id="bc225-109">Method</span></span>|<span data-ttu-id="bc225-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="bc225-110">Return Type</span></span>|<span data-ttu-id="bc225-111">说明</span><span class="sxs-lookup"><span data-stu-id="bc225-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc225-112">获取 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="bc225-112">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="bc225-113">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="bc225-113">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="bc225-114">读取属性和[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="bc225-114">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="bc225-115">更新 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="bc225-115">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="bc225-116">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="bc225-116">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="bc225-117">更新[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bc225-117">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="bc225-118">同步操作</span><span class="sxs-lookup"><span data-stu-id="bc225-118">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="bc225-119">无</span><span class="sxs-lookup"><span data-stu-id="bc225-119">None</span></span>|<span data-ttu-id="bc225-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bc225-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="bc225-121">属性</span><span class="sxs-lookup"><span data-stu-id="bc225-121">Properties</span></span>
|<span data-ttu-id="bc225-122">属性</span><span class="sxs-lookup"><span data-stu-id="bc225-122">Property</span></span>|<span data-ttu-id="bc225-123">类型</span><span class="sxs-lookup"><span data-stu-id="bc225-123">Type</span></span>|<span data-ttu-id="bc225-124">说明</span><span class="sxs-lookup"><span data-stu-id="bc225-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc225-125">id</span><span class="sxs-lookup"><span data-stu-id="bc225-125">id</span></span>|<span data-ttu-id="bc225-126">字符串</span><span class="sxs-lookup"><span data-stu-id="bc225-126">String</span></span>|<span data-ttu-id="bc225-127">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="bc225-127">The GUID for the object</span></span>|
|<span data-ttu-id="bc225-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bc225-128">lastSyncDateTime</span></span>|<span data-ttu-id="bc225-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc225-129">DateTimeOffset</span></span>|<span data-ttu-id="bc225-130">最后一个数据同步与 DD 服务的日期时间。</span><span class="sxs-lookup"><span data-stu-id="bc225-130">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="bc225-131">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="bc225-131">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="bc225-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc225-132">DateTimeOffset</span></span>|<span data-ttu-id="bc225-133">最后一个数据同步与 DD 服务的日期时间。</span><span class="sxs-lookup"><span data-stu-id="bc225-133">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="bc225-134">syncStatus</span><span class="sxs-lookup"><span data-stu-id="bc225-134">syncStatus</span></span>|[<span data-ttu-id="bc225-135">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="bc225-135">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="bc225-136">指示与设备数据同步 (DD) 服务的同步状态。</span><span class="sxs-lookup"><span data-stu-id="bc225-136">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="bc225-137">可取值为：`unknown`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="bc225-137">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc225-138">Relationships</span><span class="sxs-lookup"><span data-stu-id="bc225-138">Relationships</span></span>
<span data-ttu-id="bc225-139">无</span><span class="sxs-lookup"><span data-stu-id="bc225-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bc225-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc225-140">JSON Representation</span></span>
<span data-ttu-id="bc225-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc225-141">Here is a JSON representation of the resource.</span></span>
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





