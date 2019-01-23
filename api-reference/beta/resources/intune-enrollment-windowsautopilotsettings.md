---
title: windowsAutopilotSettings 资源类型
description: WindowsAutopilotSettings 资源表示为与 Windows 设备数据同步服务的同步数据的 Windows 自动执行某些操作帐户。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cd4641258dbc02829d4b06817467a652de2cb583
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393737"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="f5239-103">windowsAutopilotSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5239-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="f5239-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f5239-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f5239-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f5239-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5239-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5239-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5239-107">WindowsAutopilotSettings 资源表示为与 Windows 设备数据同步服务的同步数据的 Windows 自动执行某些操作帐户。</span><span class="sxs-lookup"><span data-stu-id="f5239-107">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="f5239-108">方法</span><span class="sxs-lookup"><span data-stu-id="f5239-108">Methods</span></span>
|<span data-ttu-id="f5239-109">方法</span><span class="sxs-lookup"><span data-stu-id="f5239-109">Method</span></span>|<span data-ttu-id="f5239-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f5239-110">Return Type</span></span>|<span data-ttu-id="f5239-111">说明</span><span class="sxs-lookup"><span data-stu-id="f5239-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f5239-112">获取 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="f5239-112">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="f5239-113">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="f5239-113">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="f5239-114">读取属性和[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="f5239-114">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="f5239-115">更新 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="f5239-115">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="f5239-116">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="f5239-116">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="f5239-117">更新[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f5239-117">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="f5239-118">同步操作</span><span class="sxs-lookup"><span data-stu-id="f5239-118">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="f5239-119">无</span><span class="sxs-lookup"><span data-stu-id="f5239-119">None</span></span>|<span data-ttu-id="f5239-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f5239-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f5239-121">属性</span><span class="sxs-lookup"><span data-stu-id="f5239-121">Properties</span></span>
|<span data-ttu-id="f5239-122">属性</span><span class="sxs-lookup"><span data-stu-id="f5239-122">Property</span></span>|<span data-ttu-id="f5239-123">类型</span><span class="sxs-lookup"><span data-stu-id="f5239-123">Type</span></span>|<span data-ttu-id="f5239-124">说明</span><span class="sxs-lookup"><span data-stu-id="f5239-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5239-125">id</span><span class="sxs-lookup"><span data-stu-id="f5239-125">id</span></span>|<span data-ttu-id="f5239-126">String</span><span class="sxs-lookup"><span data-stu-id="f5239-126">String</span></span>|<span data-ttu-id="f5239-127">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="f5239-127">The GUID for the object</span></span>|
|<span data-ttu-id="f5239-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f5239-128">lastSyncDateTime</span></span>|<span data-ttu-id="f5239-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5239-129">DateTimeOffset</span></span>|<span data-ttu-id="f5239-130">最后一个数据同步与 DD 服务的日期时间。</span><span class="sxs-lookup"><span data-stu-id="f5239-130">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="f5239-131">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="f5239-131">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="f5239-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5239-132">DateTimeOffset</span></span>|<span data-ttu-id="f5239-133">最后一个数据同步与 DD 服务的日期时间。</span><span class="sxs-lookup"><span data-stu-id="f5239-133">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="f5239-134">syncStatus</span><span class="sxs-lookup"><span data-stu-id="f5239-134">syncStatus</span></span>|[<span data-ttu-id="f5239-135">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="f5239-135">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="f5239-136">指示与设备数据同步 (DD) 服务的同步状态。</span><span class="sxs-lookup"><span data-stu-id="f5239-136">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="f5239-137">可取值为：`unknown`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="f5239-137">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5239-138">Relationships</span><span class="sxs-lookup"><span data-stu-id="f5239-138">Relationships</span></span>
<span data-ttu-id="f5239-139">无</span><span class="sxs-lookup"><span data-stu-id="f5239-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5239-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5239-140">JSON Representation</span></span>
<span data-ttu-id="f5239-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5239-141">Here is a JSON representation of the resource.</span></span>
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




