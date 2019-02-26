---
title: iosNotificationSettings 资源类型
description: 说明通知设置的项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ce016579729353f69f2e7671ff67b5da0004536
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260380"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="d3177-103">iosNotificationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3177-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="d3177-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3177-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3177-105">说明通知设置的项。</span><span class="sxs-lookup"><span data-stu-id="d3177-105">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="d3177-106">属性</span><span class="sxs-lookup"><span data-stu-id="d3177-106">Properties</span></span>
|<span data-ttu-id="d3177-107">属性</span><span class="sxs-lookup"><span data-stu-id="d3177-107">Property</span></span>|<span data-ttu-id="d3177-108">类型</span><span class="sxs-lookup"><span data-stu-id="d3177-108">Type</span></span>|<span data-ttu-id="d3177-109">说明</span><span class="sxs-lookup"><span data-stu-id="d3177-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3177-110">bundleID</span><span class="sxs-lookup"><span data-stu-id="d3177-110">bundleID</span></span>|<span data-ttu-id="d3177-111">String</span><span class="sxs-lookup"><span data-stu-id="d3177-111">String</span></span>|<span data-ttu-id="d3177-112">要向其应用这些通知设置的应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="d3177-112">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="d3177-113">appName</span><span class="sxs-lookup"><span data-stu-id="d3177-113">appName</span></span>|<span data-ttu-id="d3177-114">String</span><span class="sxs-lookup"><span data-stu-id="d3177-114">String</span></span>|<span data-ttu-id="d3177-115">要与 bundleID 关联的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="d3177-115">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="d3177-116">发布者</span><span class="sxs-lookup"><span data-stu-id="d3177-116">publisher</span></span>|<span data-ttu-id="d3177-117">String</span><span class="sxs-lookup"><span data-stu-id="d3177-117">String</span></span>|<span data-ttu-id="d3177-118">要与 bundleID 关联的发布者。</span><span class="sxs-lookup"><span data-stu-id="d3177-118">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="d3177-119">enabled</span><span class="sxs-lookup"><span data-stu-id="d3177-119">enabled</span></span>|<span data-ttu-id="d3177-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3177-120">Boolean</span></span>|<span data-ttu-id="d3177-121">指示是否允许此应用使用通知。</span><span class="sxs-lookup"><span data-stu-id="d3177-121">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="d3177-122">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="d3177-122">showInNotificationCenter</span></span>|<span data-ttu-id="d3177-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3177-123">Boolean</span></span>|<span data-ttu-id="d3177-124">指示是否可以在通知中心中显示通知。</span><span class="sxs-lookup"><span data-stu-id="d3177-124">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="d3177-125">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="d3177-125">showOnLockScreen</span></span>|<span data-ttu-id="d3177-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3177-126">Boolean</span></span>|<span data-ttu-id="d3177-127">指示是否可以在锁定屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="d3177-127">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="d3177-128">alertType</span><span class="sxs-lookup"><span data-stu-id="d3177-128">alertType</span></span>|[<span data-ttu-id="d3177-129">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="d3177-129">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="d3177-130">指示此应用的通知的警报类型。</span><span class="sxs-lookup"><span data-stu-id="d3177-130">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="d3177-131">可取值为：`deviceDefault`、`banner`、`modal`、`none`。</span><span class="sxs-lookup"><span data-stu-id="d3177-131">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="d3177-132">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="d3177-132">badgesEnabled</span></span>|<span data-ttu-id="d3177-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3177-133">Boolean</span></span>|<span data-ttu-id="d3177-134">指示是否允许此应用使用徽章。</span><span class="sxs-lookup"><span data-stu-id="d3177-134">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="d3177-135">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="d3177-135">soundsEnabled</span></span>|<span data-ttu-id="d3177-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="d3177-136">Boolean</span></span>|<span data-ttu-id="d3177-137">指示是否允许此应用使用声音。</span><span class="sxs-lookup"><span data-stu-id="d3177-137">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3177-138">关系</span><span class="sxs-lookup"><span data-stu-id="d3177-138">Relationships</span></span>
<span data-ttu-id="d3177-139">无</span><span class="sxs-lookup"><span data-stu-id="d3177-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3177-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3177-140">JSON Representation</span></span>
<span data-ttu-id="d3177-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3177-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```



