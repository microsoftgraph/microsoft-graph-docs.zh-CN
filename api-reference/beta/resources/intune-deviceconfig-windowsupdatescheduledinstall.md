---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
ms.openlocfilehash: 9f39a9716efed39529c54eaddc62cde075b51954
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043538"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="4597e-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="4597e-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="4597e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4597e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4597e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4597e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4597e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4597e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4597e-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4597e-107">Not yet documented</span></span>

<span data-ttu-id="4597e-108">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="4597e-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4597e-109">属性</span><span class="sxs-lookup"><span data-stu-id="4597e-109">Properties</span></span>
|<span data-ttu-id="4597e-110">属性</span><span class="sxs-lookup"><span data-stu-id="4597e-110">Property</span></span>|<span data-ttu-id="4597e-111">类型</span><span class="sxs-lookup"><span data-stu-id="4597e-111">Type</span></span>|<span data-ttu-id="4597e-112">说明</span><span class="sxs-lookup"><span data-stu-id="4597e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4597e-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="4597e-113">scheduledInstallDay</span></span>|[<span data-ttu-id="4597e-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="4597e-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="4597e-115">周中的计划安装一天。</span><span class="sxs-lookup"><span data-stu-id="4597e-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="4597e-116">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="4597e-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="4597e-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="4597e-117">scheduledInstallTime</span></span>|<span data-ttu-id="4597e-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4597e-118">TimeOfDay</span></span>|<span data-ttu-id="4597e-119">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="4597e-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="4597e-120">关系</span><span class="sxs-lookup"><span data-stu-id="4597e-120">Relationships</span></span>
<span data-ttu-id="4597e-121">无</span><span class="sxs-lookup"><span data-stu-id="4597e-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4597e-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4597e-122">JSON Representation</span></span>
<span data-ttu-id="4597e-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4597e-123">Here is a JSON representation of the resource.</span></span>
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





