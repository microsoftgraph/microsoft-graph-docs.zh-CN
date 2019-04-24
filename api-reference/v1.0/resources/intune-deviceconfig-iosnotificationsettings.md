---
title: iosNotificationSettings 资源类型
description: 说明通知设置的项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ce016579729353f69f2e7671ff67b5da0004536
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464587"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="fc30e-103">iosNotificationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc30e-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="fc30e-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc30e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc30e-105">说明通知设置的项。</span><span class="sxs-lookup"><span data-stu-id="fc30e-105">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="fc30e-106">属性</span><span class="sxs-lookup"><span data-stu-id="fc30e-106">Properties</span></span>
|<span data-ttu-id="fc30e-107">属性</span><span class="sxs-lookup"><span data-stu-id="fc30e-107">Property</span></span>|<span data-ttu-id="fc30e-108">类型</span><span class="sxs-lookup"><span data-stu-id="fc30e-108">Type</span></span>|<span data-ttu-id="fc30e-109">说明</span><span class="sxs-lookup"><span data-stu-id="fc30e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc30e-110">bundleID</span><span class="sxs-lookup"><span data-stu-id="fc30e-110">bundleID</span></span>|<span data-ttu-id="fc30e-111">字符串</span><span class="sxs-lookup"><span data-stu-id="fc30e-111">String</span></span>|<span data-ttu-id="fc30e-112">要向其应用这些通知设置的应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="fc30e-112">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="fc30e-113">appName</span><span class="sxs-lookup"><span data-stu-id="fc30e-113">appName</span></span>|<span data-ttu-id="fc30e-114">String</span><span class="sxs-lookup"><span data-stu-id="fc30e-114">String</span></span>|<span data-ttu-id="fc30e-115">要与 bundleID 关联的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="fc30e-115">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="fc30e-116">发布者</span><span class="sxs-lookup"><span data-stu-id="fc30e-116">publisher</span></span>|<span data-ttu-id="fc30e-117">String</span><span class="sxs-lookup"><span data-stu-id="fc30e-117">String</span></span>|<span data-ttu-id="fc30e-118">要与 bundleID 关联的发布者。</span><span class="sxs-lookup"><span data-stu-id="fc30e-118">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="fc30e-119">enabled</span><span class="sxs-lookup"><span data-stu-id="fc30e-119">enabled</span></span>|<span data-ttu-id="fc30e-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc30e-120">Boolean</span></span>|<span data-ttu-id="fc30e-121">指示是否允许此应用使用通知。</span><span class="sxs-lookup"><span data-stu-id="fc30e-121">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="fc30e-122">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="fc30e-122">showInNotificationCenter</span></span>|<span data-ttu-id="fc30e-123">布尔</span><span class="sxs-lookup"><span data-stu-id="fc30e-123">Boolean</span></span>|<span data-ttu-id="fc30e-124">指示是否可以在通知中心中显示通知。</span><span class="sxs-lookup"><span data-stu-id="fc30e-124">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="fc30e-125">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="fc30e-125">showOnLockScreen</span></span>|<span data-ttu-id="fc30e-126">布尔</span><span class="sxs-lookup"><span data-stu-id="fc30e-126">Boolean</span></span>|<span data-ttu-id="fc30e-127">指示是否可以在锁定屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="fc30e-127">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="fc30e-128">alertType</span><span class="sxs-lookup"><span data-stu-id="fc30e-128">alertType</span></span>|[<span data-ttu-id="fc30e-129">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="fc30e-129">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="fc30e-130">指示此应用的通知的警报类型。</span><span class="sxs-lookup"><span data-stu-id="fc30e-130">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="fc30e-131">可取值为：`deviceDefault`、`banner`、`modal`、`none`。</span><span class="sxs-lookup"><span data-stu-id="fc30e-131">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="fc30e-132">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="fc30e-132">badgesEnabled</span></span>|<span data-ttu-id="fc30e-133">布尔</span><span class="sxs-lookup"><span data-stu-id="fc30e-133">Boolean</span></span>|<span data-ttu-id="fc30e-134">指示是否允许此应用使用徽章。</span><span class="sxs-lookup"><span data-stu-id="fc30e-134">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="fc30e-135">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="fc30e-135">soundsEnabled</span></span>|<span data-ttu-id="fc30e-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="fc30e-136">Boolean</span></span>|<span data-ttu-id="fc30e-137">指示是否允许此应用使用声音。</span><span class="sxs-lookup"><span data-stu-id="fc30e-137">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc30e-138">关系</span><span class="sxs-lookup"><span data-stu-id="fc30e-138">Relationships</span></span>
<span data-ttu-id="fc30e-139">无</span><span class="sxs-lookup"><span data-stu-id="fc30e-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc30e-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc30e-140">JSON Representation</span></span>
<span data-ttu-id="fc30e-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc30e-141">Here is a JSON representation of the resource.</span></span>
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



