---
title: iosNotificationSettings 资源类型
description: 说明通知设置的项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 38ebee60ad5e4de642103a4cd72ae4f6cea0d9c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031477"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="22278-103">iosNotificationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="22278-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="22278-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22278-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22278-105">说明通知设置的项。</span><span class="sxs-lookup"><span data-stu-id="22278-105">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="22278-106">属性</span><span class="sxs-lookup"><span data-stu-id="22278-106">Properties</span></span>
|<span data-ttu-id="22278-107">属性</span><span class="sxs-lookup"><span data-stu-id="22278-107">Property</span></span>|<span data-ttu-id="22278-108">类型</span><span class="sxs-lookup"><span data-stu-id="22278-108">Type</span></span>|<span data-ttu-id="22278-109">说明</span><span class="sxs-lookup"><span data-stu-id="22278-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22278-110">bundleID</span><span class="sxs-lookup"><span data-stu-id="22278-110">bundleID</span></span>|<span data-ttu-id="22278-111">String</span><span class="sxs-lookup"><span data-stu-id="22278-111">String</span></span>|<span data-ttu-id="22278-112">要向其应用这些通知设置的应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="22278-112">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="22278-113">appName</span><span class="sxs-lookup"><span data-stu-id="22278-113">appName</span></span>|<span data-ttu-id="22278-114">String</span><span class="sxs-lookup"><span data-stu-id="22278-114">String</span></span>|<span data-ttu-id="22278-115">要与 bundleID 关联的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="22278-115">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="22278-116">发布者</span><span class="sxs-lookup"><span data-stu-id="22278-116">publisher</span></span>|<span data-ttu-id="22278-117">String</span><span class="sxs-lookup"><span data-stu-id="22278-117">String</span></span>|<span data-ttu-id="22278-118">要与 bundleID 关联的发布者。</span><span class="sxs-lookup"><span data-stu-id="22278-118">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="22278-119">enabled</span><span class="sxs-lookup"><span data-stu-id="22278-119">enabled</span></span>|<span data-ttu-id="22278-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="22278-120">Boolean</span></span>|<span data-ttu-id="22278-121">指示是否允许此应用使用通知。</span><span class="sxs-lookup"><span data-stu-id="22278-121">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="22278-122">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="22278-122">showInNotificationCenter</span></span>|<span data-ttu-id="22278-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="22278-123">Boolean</span></span>|<span data-ttu-id="22278-124">指示是否可以在通知中心中显示通知。</span><span class="sxs-lookup"><span data-stu-id="22278-124">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="22278-125">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="22278-125">showOnLockScreen</span></span>|<span data-ttu-id="22278-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="22278-126">Boolean</span></span>|<span data-ttu-id="22278-127">指示是否可以在锁定屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="22278-127">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="22278-128">alertType</span><span class="sxs-lookup"><span data-stu-id="22278-128">alertType</span></span>|[<span data-ttu-id="22278-129">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="22278-129">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="22278-130">指示此应用的通知的警报类型。</span><span class="sxs-lookup"><span data-stu-id="22278-130">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="22278-131">可取值为：`deviceDefault`、`banner`、`modal`、`none`。</span><span class="sxs-lookup"><span data-stu-id="22278-131">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="22278-132">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="22278-132">badgesEnabled</span></span>|<span data-ttu-id="22278-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="22278-133">Boolean</span></span>|<span data-ttu-id="22278-134">指示是否允许此应用使用徽章。</span><span class="sxs-lookup"><span data-stu-id="22278-134">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="22278-135">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="22278-135">soundsEnabled</span></span>|<span data-ttu-id="22278-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="22278-136">Boolean</span></span>|<span data-ttu-id="22278-137">指示是否允许此应用使用声音。</span><span class="sxs-lookup"><span data-stu-id="22278-137">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22278-138">关系</span><span class="sxs-lookup"><span data-stu-id="22278-138">Relationships</span></span>
<span data-ttu-id="22278-139">无</span><span class="sxs-lookup"><span data-stu-id="22278-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22278-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22278-140">JSON Representation</span></span>
<span data-ttu-id="22278-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22278-141">Here is a JSON representation of the resource.</span></span>
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



