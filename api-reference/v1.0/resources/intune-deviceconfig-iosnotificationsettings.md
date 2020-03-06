---
title: iosNotificationSettings 资源类型
description: 说明通知设置的项。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 309bc8ce2211f4b2abfb1e72a01c857b9221ae4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530657"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="edf58-103">iosNotificationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="edf58-103">iosNotificationSettings resource type</span></span>

<span data-ttu-id="edf58-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edf58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edf58-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="edf58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edf58-106">说明通知设置的项。</span><span class="sxs-lookup"><span data-stu-id="edf58-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="edf58-107">属性</span><span class="sxs-lookup"><span data-stu-id="edf58-107">Properties</span></span>
|<span data-ttu-id="edf58-108">属性</span><span class="sxs-lookup"><span data-stu-id="edf58-108">Property</span></span>|<span data-ttu-id="edf58-109">类型</span><span class="sxs-lookup"><span data-stu-id="edf58-109">Type</span></span>|<span data-ttu-id="edf58-110">说明</span><span class="sxs-lookup"><span data-stu-id="edf58-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edf58-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="edf58-111">bundleID</span></span>|<span data-ttu-id="edf58-112">字符串</span><span class="sxs-lookup"><span data-stu-id="edf58-112">String</span></span>|<span data-ttu-id="edf58-113">要向其应用这些通知设置的应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="edf58-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="edf58-114">appName</span><span class="sxs-lookup"><span data-stu-id="edf58-114">appName</span></span>|<span data-ttu-id="edf58-115">String</span><span class="sxs-lookup"><span data-stu-id="edf58-115">String</span></span>|<span data-ttu-id="edf58-116">要与 bundleID 关联的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="edf58-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="edf58-117">发布者</span><span class="sxs-lookup"><span data-stu-id="edf58-117">publisher</span></span>|<span data-ttu-id="edf58-118">String</span><span class="sxs-lookup"><span data-stu-id="edf58-118">String</span></span>|<span data-ttu-id="edf58-119">要与 bundleID 关联的发布者。</span><span class="sxs-lookup"><span data-stu-id="edf58-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="edf58-120">enabled</span><span class="sxs-lookup"><span data-stu-id="edf58-120">enabled</span></span>|<span data-ttu-id="edf58-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="edf58-121">Boolean</span></span>|<span data-ttu-id="edf58-122">指示是否允许此应用使用通知。</span><span class="sxs-lookup"><span data-stu-id="edf58-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="edf58-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="edf58-123">showInNotificationCenter</span></span>|<span data-ttu-id="edf58-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="edf58-124">Boolean</span></span>|<span data-ttu-id="edf58-125">指示是否可以在通知中心中显示通知。</span><span class="sxs-lookup"><span data-stu-id="edf58-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="edf58-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="edf58-126">showOnLockScreen</span></span>|<span data-ttu-id="edf58-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="edf58-127">Boolean</span></span>|<span data-ttu-id="edf58-128">指示是否可以在锁定屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="edf58-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="edf58-129">alertType</span><span class="sxs-lookup"><span data-stu-id="edf58-129">alertType</span></span>|[<span data-ttu-id="edf58-130">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="edf58-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="edf58-131">指示此应用的通知的警报类型。</span><span class="sxs-lookup"><span data-stu-id="edf58-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="edf58-132">可取值为：`deviceDefault`、`banner`、`modal`、`none`。</span><span class="sxs-lookup"><span data-stu-id="edf58-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="edf58-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="edf58-133">badgesEnabled</span></span>|<span data-ttu-id="edf58-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="edf58-134">Boolean</span></span>|<span data-ttu-id="edf58-135">指示是否允许此应用使用徽章。</span><span class="sxs-lookup"><span data-stu-id="edf58-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="edf58-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="edf58-136">soundsEnabled</span></span>|<span data-ttu-id="edf58-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="edf58-137">Boolean</span></span>|<span data-ttu-id="edf58-138">指示是否允许此应用使用声音。</span><span class="sxs-lookup"><span data-stu-id="edf58-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="edf58-139">关系</span><span class="sxs-lookup"><span data-stu-id="edf58-139">Relationships</span></span>
<span data-ttu-id="edf58-140">无</span><span class="sxs-lookup"><span data-stu-id="edf58-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="edf58-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edf58-141">JSON Representation</span></span>
<span data-ttu-id="edf58-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edf58-142">Here is a JSON representation of the resource.</span></span>
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




