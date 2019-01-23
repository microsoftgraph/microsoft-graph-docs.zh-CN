---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ee91ed2541c02adbb7a130f0a9de869d86044632
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395627"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="343d0-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="343d0-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="343d0-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="343d0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="343d0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="343d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="343d0-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="343d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="343d0-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="343d0-107">Not yet documented</span></span>


<span data-ttu-id="343d0-108">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="343d0-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="343d0-109">属性</span><span class="sxs-lookup"><span data-stu-id="343d0-109">Properties</span></span>
|<span data-ttu-id="343d0-110">属性</span><span class="sxs-lookup"><span data-stu-id="343d0-110">Property</span></span>|<span data-ttu-id="343d0-111">类型</span><span class="sxs-lookup"><span data-stu-id="343d0-111">Type</span></span>|<span data-ttu-id="343d0-112">说明</span><span class="sxs-lookup"><span data-stu-id="343d0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="343d0-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="343d0-113">scheduledInstallDay</span></span>|[<span data-ttu-id="343d0-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="343d0-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="343d0-115">周中的计划安装一天。</span><span class="sxs-lookup"><span data-stu-id="343d0-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="343d0-116">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="343d0-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="343d0-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="343d0-117">scheduledInstallTime</span></span>|<span data-ttu-id="343d0-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="343d0-118">TimeOfDay</span></span>|<span data-ttu-id="343d0-119">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="343d0-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="343d0-120">关系</span><span class="sxs-lookup"><span data-stu-id="343d0-120">Relationships</span></span>
<span data-ttu-id="343d0-121">无</span><span class="sxs-lookup"><span data-stu-id="343d0-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="343d0-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="343d0-122">JSON Representation</span></span>
<span data-ttu-id="343d0-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="343d0-123">Here is a JSON representation of the resource.</span></span>
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




