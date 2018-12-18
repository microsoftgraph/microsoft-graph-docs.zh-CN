---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: 4a8943fa0275d8b9e5a668be207c90304f22a327
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340913"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="c1619-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1619-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="c1619-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c1619-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1619-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c1619-105">Not yet documented</span></span>

<span data-ttu-id="c1619-106">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="c1619-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c1619-107">属性</span><span class="sxs-lookup"><span data-stu-id="c1619-107">Properties</span></span>
|<span data-ttu-id="c1619-108">属性</span><span class="sxs-lookup"><span data-stu-id="c1619-108">Property</span></span>|<span data-ttu-id="c1619-109">类型</span><span class="sxs-lookup"><span data-stu-id="c1619-109">Type</span></span>|<span data-ttu-id="c1619-110">说明</span><span class="sxs-lookup"><span data-stu-id="c1619-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1619-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="c1619-111">scheduledInstallDay</span></span>|[<span data-ttu-id="c1619-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="c1619-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="c1619-113">周中的计划安装一天。</span><span class="sxs-lookup"><span data-stu-id="c1619-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="c1619-114">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="c1619-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="c1619-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="c1619-115">scheduledInstallTime</span></span>|<span data-ttu-id="c1619-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c1619-116">TimeOfDay</span></span>|<span data-ttu-id="c1619-117">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="c1619-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1619-118">关系</span><span class="sxs-lookup"><span data-stu-id="c1619-118">Relationships</span></span>
<span data-ttu-id="c1619-119">无</span><span class="sxs-lookup"><span data-stu-id="c1619-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c1619-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1619-120">JSON Representation</span></span>
<span data-ttu-id="c1619-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1619-121">Here is a JSON representation of the resource.</span></span>
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



