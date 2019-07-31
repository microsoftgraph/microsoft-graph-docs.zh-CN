---
title: iosNotificationSettings 资源类型
description: 说明通知设置的项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c0d656c7df770c59d0787dcf40ad1081bb8984cd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970414"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="774bc-103">iosNotificationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="774bc-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="774bc-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="774bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="774bc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="774bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="774bc-106">说明通知设置的项。</span><span class="sxs-lookup"><span data-stu-id="774bc-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="774bc-107">属性</span><span class="sxs-lookup"><span data-stu-id="774bc-107">Properties</span></span>
|<span data-ttu-id="774bc-108">属性</span><span class="sxs-lookup"><span data-stu-id="774bc-108">Property</span></span>|<span data-ttu-id="774bc-109">类型</span><span class="sxs-lookup"><span data-stu-id="774bc-109">Type</span></span>|<span data-ttu-id="774bc-110">说明</span><span class="sxs-lookup"><span data-stu-id="774bc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="774bc-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="774bc-111">bundleID</span></span>|<span data-ttu-id="774bc-112">String</span><span class="sxs-lookup"><span data-stu-id="774bc-112">String</span></span>|<span data-ttu-id="774bc-113">要向其应用这些通知设置的应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="774bc-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="774bc-114">appName</span><span class="sxs-lookup"><span data-stu-id="774bc-114">appName</span></span>|<span data-ttu-id="774bc-115">String</span><span class="sxs-lookup"><span data-stu-id="774bc-115">String</span></span>|<span data-ttu-id="774bc-116">要与 bundleID 关联的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="774bc-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="774bc-117">发布者</span><span class="sxs-lookup"><span data-stu-id="774bc-117">publisher</span></span>|<span data-ttu-id="774bc-118">String</span><span class="sxs-lookup"><span data-stu-id="774bc-118">String</span></span>|<span data-ttu-id="774bc-119">要与 bundleID 关联的发布者。</span><span class="sxs-lookup"><span data-stu-id="774bc-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="774bc-120">enabled</span><span class="sxs-lookup"><span data-stu-id="774bc-120">enabled</span></span>|<span data-ttu-id="774bc-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="774bc-121">Boolean</span></span>|<span data-ttu-id="774bc-122">指示是否允许此应用使用通知。</span><span class="sxs-lookup"><span data-stu-id="774bc-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="774bc-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="774bc-123">showInNotificationCenter</span></span>|<span data-ttu-id="774bc-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="774bc-124">Boolean</span></span>|<span data-ttu-id="774bc-125">指示是否可以在通知中心中显示通知。</span><span class="sxs-lookup"><span data-stu-id="774bc-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="774bc-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="774bc-126">showOnLockScreen</span></span>|<span data-ttu-id="774bc-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="774bc-127">Boolean</span></span>|<span data-ttu-id="774bc-128">指示是否可以在锁定屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="774bc-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="774bc-129">alertType</span><span class="sxs-lookup"><span data-stu-id="774bc-129">alertType</span></span>|[<span data-ttu-id="774bc-130">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="774bc-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="774bc-131">指示此应用的通知的警报类型。</span><span class="sxs-lookup"><span data-stu-id="774bc-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="774bc-132">可取值为：`deviceDefault`、`banner`、`modal`、`none`。</span><span class="sxs-lookup"><span data-stu-id="774bc-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="774bc-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="774bc-133">badgesEnabled</span></span>|<span data-ttu-id="774bc-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="774bc-134">Boolean</span></span>|<span data-ttu-id="774bc-135">指示是否允许此应用使用徽章。</span><span class="sxs-lookup"><span data-stu-id="774bc-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="774bc-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="774bc-136">soundsEnabled</span></span>|<span data-ttu-id="774bc-137">布尔值</span><span class="sxs-lookup"><span data-stu-id="774bc-137">Boolean</span></span>|<span data-ttu-id="774bc-138">指示是否允许此应用使用声音。</span><span class="sxs-lookup"><span data-stu-id="774bc-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="774bc-139">关系</span><span class="sxs-lookup"><span data-stu-id="774bc-139">Relationships</span></span>
<span data-ttu-id="774bc-140">无</span><span class="sxs-lookup"><span data-stu-id="774bc-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="774bc-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="774bc-141">JSON Representation</span></span>
<span data-ttu-id="774bc-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="774bc-142">Here is a JSON representation of the resource.</span></span>
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





