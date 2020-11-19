---
title: iosNotificationSettings 资源类型
description: 说明通知设置的项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ca6c5cf968897d701870bc695dcce909c74f1fc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280135"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="87ff7-103">iosNotificationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="87ff7-103">iosNotificationSettings resource type</span></span>

<span data-ttu-id="87ff7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87ff7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87ff7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="87ff7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87ff7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="87ff7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87ff7-107">说明通知设置的项。</span><span class="sxs-lookup"><span data-stu-id="87ff7-107">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="87ff7-108">属性</span><span class="sxs-lookup"><span data-stu-id="87ff7-108">Properties</span></span>
|<span data-ttu-id="87ff7-109">属性</span><span class="sxs-lookup"><span data-stu-id="87ff7-109">Property</span></span>|<span data-ttu-id="87ff7-110">类型</span><span class="sxs-lookup"><span data-stu-id="87ff7-110">Type</span></span>|<span data-ttu-id="87ff7-111">说明</span><span class="sxs-lookup"><span data-stu-id="87ff7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87ff7-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="87ff7-112">bundleID</span></span>|<span data-ttu-id="87ff7-113">String</span><span class="sxs-lookup"><span data-stu-id="87ff7-113">String</span></span>|<span data-ttu-id="87ff7-114">要向其应用这些通知设置的应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="87ff7-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="87ff7-115">appName</span><span class="sxs-lookup"><span data-stu-id="87ff7-115">appName</span></span>|<span data-ttu-id="87ff7-116">String</span><span class="sxs-lookup"><span data-stu-id="87ff7-116">String</span></span>|<span data-ttu-id="87ff7-117">要与 bundleID 关联的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="87ff7-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="87ff7-118">发布者</span><span class="sxs-lookup"><span data-stu-id="87ff7-118">publisher</span></span>|<span data-ttu-id="87ff7-119">String</span><span class="sxs-lookup"><span data-stu-id="87ff7-119">String</span></span>|<span data-ttu-id="87ff7-120">要与 bundleID 关联的发布者。</span><span class="sxs-lookup"><span data-stu-id="87ff7-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="87ff7-121">enabled</span><span class="sxs-lookup"><span data-stu-id="87ff7-121">enabled</span></span>|<span data-ttu-id="87ff7-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="87ff7-122">Boolean</span></span>|<span data-ttu-id="87ff7-123">指示是否允许此应用使用通知。</span><span class="sxs-lookup"><span data-stu-id="87ff7-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="87ff7-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="87ff7-124">showInNotificationCenter</span></span>|<span data-ttu-id="87ff7-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="87ff7-125">Boolean</span></span>|<span data-ttu-id="87ff7-126">指示是否可以在通知中心中显示通知。</span><span class="sxs-lookup"><span data-stu-id="87ff7-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="87ff7-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="87ff7-127">showOnLockScreen</span></span>|<span data-ttu-id="87ff7-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="87ff7-128">Boolean</span></span>|<span data-ttu-id="87ff7-129">指示是否可以在锁定屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="87ff7-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="87ff7-130">alertType</span><span class="sxs-lookup"><span data-stu-id="87ff7-130">alertType</span></span>|[<span data-ttu-id="87ff7-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="87ff7-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="87ff7-132">指示此应用的通知的警报类型。</span><span class="sxs-lookup"><span data-stu-id="87ff7-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="87ff7-133">可取值为：`deviceDefault`、`banner`、`modal`、`none`。</span><span class="sxs-lookup"><span data-stu-id="87ff7-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="87ff7-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="87ff7-134">badgesEnabled</span></span>|<span data-ttu-id="87ff7-135">布尔值</span><span class="sxs-lookup"><span data-stu-id="87ff7-135">Boolean</span></span>|<span data-ttu-id="87ff7-136">指示是否允许此应用使用徽章。</span><span class="sxs-lookup"><span data-stu-id="87ff7-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="87ff7-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="87ff7-137">soundsEnabled</span></span>|<span data-ttu-id="87ff7-138">布尔值</span><span class="sxs-lookup"><span data-stu-id="87ff7-138">Boolean</span></span>|<span data-ttu-id="87ff7-139">指示是否允许此应用使用声音。</span><span class="sxs-lookup"><span data-stu-id="87ff7-139">Indicates whether sounds are allowed for this app.</span></span>|
|<span data-ttu-id="87ff7-140">previewVisibility</span><span class="sxs-lookup"><span data-stu-id="87ff7-140">previewVisibility</span></span>|[<span data-ttu-id="87ff7-141">iosNotificationPreviewVisibility</span><span class="sxs-lookup"><span data-stu-id="87ff7-141">iosNotificationPreviewVisibility</span></span>](../resources/intune-deviceconfig-iosnotificationpreviewvisibility.md)|<span data-ttu-id="87ff7-142">替代由用户在 iOS 设备上设置的通知预览策略。</span><span class="sxs-lookup"><span data-stu-id="87ff7-142">Overrides the notification preview policy set by the user on an iOS device.</span></span> <span data-ttu-id="87ff7-143">可取值为：`notConfigured`、`alwaysShow`、`hideWhenLocked`、`neverShow`。</span><span class="sxs-lookup"><span data-stu-id="87ff7-143">Possible values are: `notConfigured`, `alwaysShow`, `hideWhenLocked`, `neverShow`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87ff7-144">关系</span><span class="sxs-lookup"><span data-stu-id="87ff7-144">Relationships</span></span>
<span data-ttu-id="87ff7-145">无</span><span class="sxs-lookup"><span data-stu-id="87ff7-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87ff7-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87ff7-146">JSON Representation</span></span>
<span data-ttu-id="87ff7-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87ff7-147">Here is a JSON representation of the resource.</span></span>
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
  "soundsEnabled": true,
  "previewVisibility": "String"
}
```




