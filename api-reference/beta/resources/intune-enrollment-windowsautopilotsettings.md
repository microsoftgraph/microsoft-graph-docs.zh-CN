---
title: windowsAutopilotSettings 资源类型
description: WindowsAutopilotSettings 资源表示为与 Windows 设备数据同步服务的同步数据的 Windows 自动执行某些操作帐户。
author: tfitzmac
ms.openlocfilehash: d502af67cc1a68c56e1bdd74965e77224947b5d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344630"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="9535a-103">windowsAutopilotSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="9535a-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="9535a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9535a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9535a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9535a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9535a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9535a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9535a-107">WindowsAutopilotSettings 资源表示为与 Windows 设备数据同步服务的同步数据的 Windows 自动执行某些操作帐户。</span><span class="sxs-lookup"><span data-stu-id="9535a-107">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>
## <a name="methods"></a><span data-ttu-id="9535a-108">方法</span><span class="sxs-lookup"><span data-stu-id="9535a-108">Methods</span></span>
|<span data-ttu-id="9535a-109">方法</span><span class="sxs-lookup"><span data-stu-id="9535a-109">Method</span></span>|<span data-ttu-id="9535a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9535a-110">Return Type</span></span>|<span data-ttu-id="9535a-111">说明</span><span class="sxs-lookup"><span data-stu-id="9535a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9535a-112">获取 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="9535a-112">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="9535a-113">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="9535a-113">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="9535a-114">读取属性和[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="9535a-114">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="9535a-115">更新 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="9535a-115">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="9535a-116">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="9535a-116">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="9535a-117">更新[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9535a-117">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="9535a-118">同步操作</span><span class="sxs-lookup"><span data-stu-id="9535a-118">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="9535a-119">无</span><span class="sxs-lookup"><span data-stu-id="9535a-119">None</span></span>|<span data-ttu-id="9535a-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9535a-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9535a-121">属性</span><span class="sxs-lookup"><span data-stu-id="9535a-121">Properties</span></span>
|<span data-ttu-id="9535a-122">属性</span><span class="sxs-lookup"><span data-stu-id="9535a-122">Property</span></span>|<span data-ttu-id="9535a-123">类型</span><span class="sxs-lookup"><span data-stu-id="9535a-123">Type</span></span>|<span data-ttu-id="9535a-124">说明</span><span class="sxs-lookup"><span data-stu-id="9535a-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9535a-125">id</span><span class="sxs-lookup"><span data-stu-id="9535a-125">id</span></span>|<span data-ttu-id="9535a-126">字符串</span><span class="sxs-lookup"><span data-stu-id="9535a-126">String</span></span>|<span data-ttu-id="9535a-127">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="9535a-127">The GUID for the object</span></span>|
|<span data-ttu-id="9535a-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="9535a-128">lastSyncDateTime</span></span>|<span data-ttu-id="9535a-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9535a-129">DateTimeOffset</span></span>|<span data-ttu-id="9535a-130">最后一个数据同步与 DD 服务的日期时间。</span><span class="sxs-lookup"><span data-stu-id="9535a-130">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="9535a-131">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="9535a-131">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="9535a-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9535a-132">DateTimeOffset</span></span>|<span data-ttu-id="9535a-133">最后一个数据同步与 DD 服务的日期时间。</span><span class="sxs-lookup"><span data-stu-id="9535a-133">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="9535a-134">syncStatus</span><span class="sxs-lookup"><span data-stu-id="9535a-134">syncStatus</span></span>|[<span data-ttu-id="9535a-135">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="9535a-135">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="9535a-136">指示与设备数据同步 (DD) 服务的同步状态。</span><span class="sxs-lookup"><span data-stu-id="9535a-136">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="9535a-137">可取值为：`unknown`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="9535a-137">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9535a-138">Relationships</span><span class="sxs-lookup"><span data-stu-id="9535a-138">Relationships</span></span>
<span data-ttu-id="9535a-139">无</span><span class="sxs-lookup"><span data-stu-id="9535a-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9535a-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9535a-140">JSON Representation</span></span>
<span data-ttu-id="9535a-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9535a-141">Here is a JSON representation of the resource.</span></span>
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





