---
title: iosNotificationSettings 资源类型
description: 说明通知设置的项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d2fbc197f858b595bfe8572badddef9dadf6b3c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521416"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="13ce1-103">iosNotificationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="13ce1-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="13ce1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13ce1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13ce1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13ce1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13ce1-106">说明通知设置的项。</span><span class="sxs-lookup"><span data-stu-id="13ce1-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="13ce1-107">属性</span><span class="sxs-lookup"><span data-stu-id="13ce1-107">Properties</span></span>
|<span data-ttu-id="13ce1-108">属性</span><span class="sxs-lookup"><span data-stu-id="13ce1-108">Property</span></span>|<span data-ttu-id="13ce1-109">类型</span><span class="sxs-lookup"><span data-stu-id="13ce1-109">Type</span></span>|<span data-ttu-id="13ce1-110">说明</span><span class="sxs-lookup"><span data-stu-id="13ce1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13ce1-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="13ce1-111">bundleID</span></span>|<span data-ttu-id="13ce1-112">String</span><span class="sxs-lookup"><span data-stu-id="13ce1-112">String</span></span>|<span data-ttu-id="13ce1-113">要向其应用这些通知设置的应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="13ce1-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="13ce1-114">appName</span><span class="sxs-lookup"><span data-stu-id="13ce1-114">appName</span></span>|<span data-ttu-id="13ce1-115">String</span><span class="sxs-lookup"><span data-stu-id="13ce1-115">String</span></span>|<span data-ttu-id="13ce1-116">要与 bundleID 关联的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="13ce1-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="13ce1-117">发布者</span><span class="sxs-lookup"><span data-stu-id="13ce1-117">publisher</span></span>|<span data-ttu-id="13ce1-118">String</span><span class="sxs-lookup"><span data-stu-id="13ce1-118">String</span></span>|<span data-ttu-id="13ce1-119">要与 bundleID 关联的发布者。</span><span class="sxs-lookup"><span data-stu-id="13ce1-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="13ce1-120">enabled</span><span class="sxs-lookup"><span data-stu-id="13ce1-120">enabled</span></span>|<span data-ttu-id="13ce1-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="13ce1-121">Boolean</span></span>|<span data-ttu-id="13ce1-122">指示是否允许此应用使用通知。</span><span class="sxs-lookup"><span data-stu-id="13ce1-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="13ce1-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="13ce1-123">showInNotificationCenter</span></span>|<span data-ttu-id="13ce1-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="13ce1-124">Boolean</span></span>|<span data-ttu-id="13ce1-125">指示是否可以在通知中心中显示通知。</span><span class="sxs-lookup"><span data-stu-id="13ce1-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="13ce1-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="13ce1-126">showOnLockScreen</span></span>|<span data-ttu-id="13ce1-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="13ce1-127">Boolean</span></span>|<span data-ttu-id="13ce1-128">指示是否可以在锁定屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="13ce1-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="13ce1-129">alertType</span><span class="sxs-lookup"><span data-stu-id="13ce1-129">alertType</span></span>|[<span data-ttu-id="13ce1-130">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="13ce1-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="13ce1-131">指示此应用的通知的警报类型。</span><span class="sxs-lookup"><span data-stu-id="13ce1-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="13ce1-132">可取值为：`deviceDefault`、`banner`、`modal`、`none`。</span><span class="sxs-lookup"><span data-stu-id="13ce1-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="13ce1-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="13ce1-133">badgesEnabled</span></span>|<span data-ttu-id="13ce1-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="13ce1-134">Boolean</span></span>|<span data-ttu-id="13ce1-135">指示是否允许此应用使用徽章。</span><span class="sxs-lookup"><span data-stu-id="13ce1-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="13ce1-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="13ce1-136">soundsEnabled</span></span>|<span data-ttu-id="13ce1-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="13ce1-137">Boolean</span></span>|<span data-ttu-id="13ce1-138">指示是否允许此应用使用声音。</span><span class="sxs-lookup"><span data-stu-id="13ce1-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13ce1-139">关系</span><span class="sxs-lookup"><span data-stu-id="13ce1-139">Relationships</span></span>
<span data-ttu-id="13ce1-140">无</span><span class="sxs-lookup"><span data-stu-id="13ce1-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13ce1-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13ce1-141">JSON Representation</span></span>
<span data-ttu-id="13ce1-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13ce1-142">Here is a JSON representation of the resource.</span></span>
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





