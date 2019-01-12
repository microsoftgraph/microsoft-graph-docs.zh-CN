---
title: windowsUpdateScheduledInstall 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3c0a58bf0bb6bc95c0208e1195566d5fc125073d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971849"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="cb875-103">windowsUpdateScheduledInstall 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb875-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="cb875-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cb875-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cb875-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cb875-105">Not yet documented</span></span>

<span data-ttu-id="cb875-106">继承自 [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="cb875-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cb875-107">属性</span><span class="sxs-lookup"><span data-stu-id="cb875-107">Properties</span></span>
|<span data-ttu-id="cb875-108">属性</span><span class="sxs-lookup"><span data-stu-id="cb875-108">Property</span></span>|<span data-ttu-id="cb875-109">类型</span><span class="sxs-lookup"><span data-stu-id="cb875-109">Type</span></span>|<span data-ttu-id="cb875-110">说明</span><span class="sxs-lookup"><span data-stu-id="cb875-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb875-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="cb875-111">scheduledInstallDay</span></span>|[<span data-ttu-id="cb875-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="cb875-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="cb875-113">周中的计划安装一天。</span><span class="sxs-lookup"><span data-stu-id="cb875-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="cb875-114">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="cb875-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="cb875-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="cb875-115">scheduledInstallTime</span></span>|<span data-ttu-id="cb875-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="cb875-116">TimeOfDay</span></span>|<span data-ttu-id="cb875-117">一天中的计划安装时间</span><span class="sxs-lookup"><span data-stu-id="cb875-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb875-118">关系</span><span class="sxs-lookup"><span data-stu-id="cb875-118">Relationships</span></span>
<span data-ttu-id="cb875-119">无</span><span class="sxs-lookup"><span data-stu-id="cb875-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cb875-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb875-120">JSON Representation</span></span>
<span data-ttu-id="cb875-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb875-121">Here is a JSON representation of the resource.</span></span>
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



