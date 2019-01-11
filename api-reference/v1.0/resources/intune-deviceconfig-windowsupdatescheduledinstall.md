---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 19e0ced371108103398e26c6067f4ce3b3ab67e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806403"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="8d264-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d264-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="8d264-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8d264-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d264-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8d264-105">Not yet documented</span></span>

<span data-ttu-id="8d264-106">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="8d264-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8d264-107">属性</span><span class="sxs-lookup"><span data-stu-id="8d264-107">Properties</span></span>
|<span data-ttu-id="8d264-108">属性</span><span class="sxs-lookup"><span data-stu-id="8d264-108">Property</span></span>|<span data-ttu-id="8d264-109">类型</span><span class="sxs-lookup"><span data-stu-id="8d264-109">Type</span></span>|<span data-ttu-id="8d264-110">说明</span><span class="sxs-lookup"><span data-stu-id="8d264-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d264-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="8d264-111">scheduledInstallDay</span></span>|[<span data-ttu-id="8d264-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="8d264-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="8d264-113">周中的计划安装一天。</span><span class="sxs-lookup"><span data-stu-id="8d264-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="8d264-114">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="8d264-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="8d264-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="8d264-115">scheduledInstallTime</span></span>|<span data-ttu-id="8d264-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8d264-116">TimeOfDay</span></span>|<span data-ttu-id="8d264-117">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="8d264-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d264-118">关系</span><span class="sxs-lookup"><span data-stu-id="8d264-118">Relationships</span></span>
<span data-ttu-id="8d264-119">无</span><span class="sxs-lookup"><span data-stu-id="8d264-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8d264-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d264-120">JSON Representation</span></span>
<span data-ttu-id="8d264-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d264-121">Here is a JSON representation of the resource.</span></span>
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



