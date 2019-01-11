---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 47518277f54526e84cc3152a96ba3b49ec8a199e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835999"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="fc727-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc727-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="fc727-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fc727-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc727-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fc727-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc727-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fc727-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc727-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fc727-107">Not yet documented</span></span>

<span data-ttu-id="fc727-108">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="fc727-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fc727-109">属性</span><span class="sxs-lookup"><span data-stu-id="fc727-109">Properties</span></span>
|<span data-ttu-id="fc727-110">属性</span><span class="sxs-lookup"><span data-stu-id="fc727-110">Property</span></span>|<span data-ttu-id="fc727-111">类型</span><span class="sxs-lookup"><span data-stu-id="fc727-111">Type</span></span>|<span data-ttu-id="fc727-112">说明</span><span class="sxs-lookup"><span data-stu-id="fc727-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc727-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="fc727-113">scheduledInstallDay</span></span>|[<span data-ttu-id="fc727-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="fc727-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="fc727-115">周中的计划安装一天。</span><span class="sxs-lookup"><span data-stu-id="fc727-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="fc727-116">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="fc727-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="fc727-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="fc727-117">scheduledInstallTime</span></span>|<span data-ttu-id="fc727-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fc727-118">TimeOfDay</span></span>|<span data-ttu-id="fc727-119">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="fc727-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc727-120">关系</span><span class="sxs-lookup"><span data-stu-id="fc727-120">Relationships</span></span>
<span data-ttu-id="fc727-121">无</span><span class="sxs-lookup"><span data-stu-id="fc727-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fc727-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc727-122">JSON Representation</span></span>
<span data-ttu-id="fc727-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc727-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```





