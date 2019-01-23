---
title: iosNotificationSettings 资源类型
description: 说明通知设置的项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7db0b6ba438522db0795f6897daba8b5c43258c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420498"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="7265f-103">iosNotificationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="7265f-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="7265f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="7265f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7265f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7265f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7265f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7265f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7265f-107">说明通知设置的项。</span><span class="sxs-lookup"><span data-stu-id="7265f-107">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="7265f-108">属性</span><span class="sxs-lookup"><span data-stu-id="7265f-108">Properties</span></span>
|<span data-ttu-id="7265f-109">属性</span><span class="sxs-lookup"><span data-stu-id="7265f-109">Property</span></span>|<span data-ttu-id="7265f-110">类型</span><span class="sxs-lookup"><span data-stu-id="7265f-110">Type</span></span>|<span data-ttu-id="7265f-111">说明</span><span class="sxs-lookup"><span data-stu-id="7265f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7265f-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="7265f-112">bundleID</span></span>|<span data-ttu-id="7265f-113">String</span><span class="sxs-lookup"><span data-stu-id="7265f-113">String</span></span>|<span data-ttu-id="7265f-114">要向其应用这些通知设置的应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="7265f-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="7265f-115">appName</span><span class="sxs-lookup"><span data-stu-id="7265f-115">appName</span></span>|<span data-ttu-id="7265f-116">String</span><span class="sxs-lookup"><span data-stu-id="7265f-116">String</span></span>|<span data-ttu-id="7265f-117">要与 bundleID 关联的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="7265f-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="7265f-118">发布者</span><span class="sxs-lookup"><span data-stu-id="7265f-118">publisher</span></span>|<span data-ttu-id="7265f-119">String</span><span class="sxs-lookup"><span data-stu-id="7265f-119">String</span></span>|<span data-ttu-id="7265f-120">要与 bundleID 关联的发布者。</span><span class="sxs-lookup"><span data-stu-id="7265f-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="7265f-121">enabled</span><span class="sxs-lookup"><span data-stu-id="7265f-121">enabled</span></span>|<span data-ttu-id="7265f-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="7265f-122">Boolean</span></span>|<span data-ttu-id="7265f-123">指示是否允许此应用使用通知。</span><span class="sxs-lookup"><span data-stu-id="7265f-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="7265f-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="7265f-124">showInNotificationCenter</span></span>|<span data-ttu-id="7265f-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="7265f-125">Boolean</span></span>|<span data-ttu-id="7265f-126">指示是否可以在通知中心中显示通知。</span><span class="sxs-lookup"><span data-stu-id="7265f-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="7265f-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="7265f-127">showOnLockScreen</span></span>|<span data-ttu-id="7265f-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="7265f-128">Boolean</span></span>|<span data-ttu-id="7265f-129">指示是否可以在锁定屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="7265f-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="7265f-130">alertType</span><span class="sxs-lookup"><span data-stu-id="7265f-130">alertType</span></span>|[<span data-ttu-id="7265f-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="7265f-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="7265f-132">指示此应用的通知的警报类型。</span><span class="sxs-lookup"><span data-stu-id="7265f-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="7265f-133">可取值为：`deviceDefault`、`banner`、`modal`、`none`。</span><span class="sxs-lookup"><span data-stu-id="7265f-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="7265f-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="7265f-134">badgesEnabled</span></span>|<span data-ttu-id="7265f-135">布尔值</span><span class="sxs-lookup"><span data-stu-id="7265f-135">Boolean</span></span>|<span data-ttu-id="7265f-136">指示是否允许此应用使用徽章。</span><span class="sxs-lookup"><span data-stu-id="7265f-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="7265f-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="7265f-137">soundsEnabled</span></span>|<span data-ttu-id="7265f-138">布尔值</span><span class="sxs-lookup"><span data-stu-id="7265f-138">Boolean</span></span>|<span data-ttu-id="7265f-139">指示是否允许此应用使用声音。</span><span class="sxs-lookup"><span data-stu-id="7265f-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7265f-140">关系</span><span class="sxs-lookup"><span data-stu-id="7265f-140">Relationships</span></span>
<span data-ttu-id="7265f-141">无</span><span class="sxs-lookup"><span data-stu-id="7265f-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7265f-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7265f-142">JSON Representation</span></span>
<span data-ttu-id="7265f-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7265f-143">Here is a JSON representation of the resource.</span></span>
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




