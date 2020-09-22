---
title: iosNotificationSettings 资源类型
description: 说明通知设置的项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0e3dc929e96869475d4376c344bf08ff17ae7edd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074984"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="211ab-103">iosNotificationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="211ab-103">iosNotificationSettings resource type</span></span>

<span data-ttu-id="211ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="211ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="211ab-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="211ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="211ab-106">说明通知设置的项。</span><span class="sxs-lookup"><span data-stu-id="211ab-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="211ab-107">属性</span><span class="sxs-lookup"><span data-stu-id="211ab-107">Properties</span></span>
|<span data-ttu-id="211ab-108">属性</span><span class="sxs-lookup"><span data-stu-id="211ab-108">Property</span></span>|<span data-ttu-id="211ab-109">类型</span><span class="sxs-lookup"><span data-stu-id="211ab-109">Type</span></span>|<span data-ttu-id="211ab-110">说明</span><span class="sxs-lookup"><span data-stu-id="211ab-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="211ab-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="211ab-111">bundleID</span></span>|<span data-ttu-id="211ab-112">String</span><span class="sxs-lookup"><span data-stu-id="211ab-112">String</span></span>|<span data-ttu-id="211ab-113">要向其应用这些通知设置的应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="211ab-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="211ab-114">appName</span><span class="sxs-lookup"><span data-stu-id="211ab-114">appName</span></span>|<span data-ttu-id="211ab-115">String</span><span class="sxs-lookup"><span data-stu-id="211ab-115">String</span></span>|<span data-ttu-id="211ab-116">要与 bundleID 关联的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="211ab-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="211ab-117">发布者</span><span class="sxs-lookup"><span data-stu-id="211ab-117">publisher</span></span>|<span data-ttu-id="211ab-118">String</span><span class="sxs-lookup"><span data-stu-id="211ab-118">String</span></span>|<span data-ttu-id="211ab-119">要与 bundleID 关联的发布者。</span><span class="sxs-lookup"><span data-stu-id="211ab-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="211ab-120">enabled</span><span class="sxs-lookup"><span data-stu-id="211ab-120">enabled</span></span>|<span data-ttu-id="211ab-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="211ab-121">Boolean</span></span>|<span data-ttu-id="211ab-122">指示是否允许此应用使用通知。</span><span class="sxs-lookup"><span data-stu-id="211ab-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="211ab-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="211ab-123">showInNotificationCenter</span></span>|<span data-ttu-id="211ab-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="211ab-124">Boolean</span></span>|<span data-ttu-id="211ab-125">指示是否可以在通知中心中显示通知。</span><span class="sxs-lookup"><span data-stu-id="211ab-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="211ab-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="211ab-126">showOnLockScreen</span></span>|<span data-ttu-id="211ab-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="211ab-127">Boolean</span></span>|<span data-ttu-id="211ab-128">指示是否可以在锁定屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="211ab-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="211ab-129">alertType</span><span class="sxs-lookup"><span data-stu-id="211ab-129">alertType</span></span>|[<span data-ttu-id="211ab-130">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="211ab-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="211ab-131">指示此应用的通知的警报类型。</span><span class="sxs-lookup"><span data-stu-id="211ab-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="211ab-132">可取值为：`deviceDefault`、`banner`、`modal`、`none`。</span><span class="sxs-lookup"><span data-stu-id="211ab-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="211ab-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="211ab-133">badgesEnabled</span></span>|<span data-ttu-id="211ab-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="211ab-134">Boolean</span></span>|<span data-ttu-id="211ab-135">指示是否允许此应用使用徽章。</span><span class="sxs-lookup"><span data-stu-id="211ab-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="211ab-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="211ab-136">soundsEnabled</span></span>|<span data-ttu-id="211ab-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="211ab-137">Boolean</span></span>|<span data-ttu-id="211ab-138">指示是否允许此应用使用声音。</span><span class="sxs-lookup"><span data-stu-id="211ab-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="211ab-139">关系</span><span class="sxs-lookup"><span data-stu-id="211ab-139">Relationships</span></span>
<span data-ttu-id="211ab-140">无</span><span class="sxs-lookup"><span data-stu-id="211ab-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="211ab-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="211ab-141">JSON Representation</span></span>
<span data-ttu-id="211ab-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="211ab-142">Here is a JSON representation of the resource.</span></span>
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









