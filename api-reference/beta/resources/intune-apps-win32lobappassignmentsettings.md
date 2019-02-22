---
title: win32LobAppAssignmentSettings 资源类型
description: 包含用于将 Win32 LOB 移动应用程序分配给组的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e98688a10c126ee6597f8d244e4a605a2addeaee
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172175"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="82bc0-103">win32LobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="82bc0-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="82bc0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="82bc0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82bc0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82bc0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82bc0-106">包含用于将 Win32 LOB 移动应用程序分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="82bc0-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="82bc0-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="82bc0-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="82bc0-108">属性</span><span class="sxs-lookup"><span data-stu-id="82bc0-108">Properties</span></span>
|<span data-ttu-id="82bc0-109">属性</span><span class="sxs-lookup"><span data-stu-id="82bc0-109">Property</span></span>|<span data-ttu-id="82bc0-110">类型</span><span class="sxs-lookup"><span data-stu-id="82bc0-110">Type</span></span>|<span data-ttu-id="82bc0-111">说明</span><span class="sxs-lookup"><span data-stu-id="82bc0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82bc0-112">通知</span><span class="sxs-lookup"><span data-stu-id="82bc0-112">notifications</span></span>|[<span data-ttu-id="82bc0-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="82bc0-113">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="82bc0-114">此应用程序分配的通知状态。</span><span class="sxs-lookup"><span data-stu-id="82bc0-114">The notification status this app assignment.</span></span> <span data-ttu-id="82bc0-115">可取值为：`showAll`、`showReboot`、`hideAll`。</span><span class="sxs-lookup"><span data-stu-id="82bc0-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82bc0-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="82bc0-116">Relationships</span></span>
<span data-ttu-id="82bc0-117">无</span><span class="sxs-lookup"><span data-stu-id="82bc0-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82bc0-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82bc0-118">JSON Representation</span></span>
<span data-ttu-id="82bc0-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82bc0-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppAssignmentSettings",
  "notifications": "String"
}
```




