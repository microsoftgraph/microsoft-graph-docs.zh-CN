---
title: win32LobAppAssignmentSettings 资源类型
description: 包含用于将 Win32 LOB 移动应用程序分配给组的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 445cd1a03a7495d4946f600dea3773d7bd9e2249
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774237"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="79e89-103">win32LobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="79e89-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="79e89-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="79e89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79e89-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79e89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79e89-106">包含用于将 Win32 LOB 移动应用程序分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="79e89-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="79e89-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="79e89-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="79e89-108">属性</span><span class="sxs-lookup"><span data-stu-id="79e89-108">Properties</span></span>
|<span data-ttu-id="79e89-109">属性</span><span class="sxs-lookup"><span data-stu-id="79e89-109">Property</span></span>|<span data-ttu-id="79e89-110">类型</span><span class="sxs-lookup"><span data-stu-id="79e89-110">Type</span></span>|<span data-ttu-id="79e89-111">说明</span><span class="sxs-lookup"><span data-stu-id="79e89-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79e89-112">通知</span><span class="sxs-lookup"><span data-stu-id="79e89-112">notifications</span></span>|[<span data-ttu-id="79e89-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="79e89-113">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="79e89-114">此应用程序分配的通知状态。</span><span class="sxs-lookup"><span data-stu-id="79e89-114">The notification status this app assignment.</span></span> <span data-ttu-id="79e89-115">可取值为：`showAll`、`showReboot`、`hideAll`。</span><span class="sxs-lookup"><span data-stu-id="79e89-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79e89-116">关系</span><span class="sxs-lookup"><span data-stu-id="79e89-116">Relationships</span></span>
<span data-ttu-id="79e89-117">无</span><span class="sxs-lookup"><span data-stu-id="79e89-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79e89-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79e89-118">JSON Representation</span></span>
<span data-ttu-id="79e89-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79e89-119">Here is a JSON representation of the resource.</span></span>
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





