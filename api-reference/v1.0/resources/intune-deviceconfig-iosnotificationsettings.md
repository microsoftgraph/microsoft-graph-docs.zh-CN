---
title: iosNotificationSettings 资源类型
description: 说明通知设置的项。
author: tfitzmac
ms.openlocfilehash: 197de8b9cd59d1f6c998f92460e62aab480ef455
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307838"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="00b45-103">iosNotificationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="00b45-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="00b45-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="00b45-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00b45-105">说明通知设置的项。</span><span class="sxs-lookup"><span data-stu-id="00b45-105">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="00b45-106">属性</span><span class="sxs-lookup"><span data-stu-id="00b45-106">Properties</span></span>
|<span data-ttu-id="00b45-107">属性</span><span class="sxs-lookup"><span data-stu-id="00b45-107">Property</span></span>|<span data-ttu-id="00b45-108">类型</span><span class="sxs-lookup"><span data-stu-id="00b45-108">Type</span></span>|<span data-ttu-id="00b45-109">说明</span><span class="sxs-lookup"><span data-stu-id="00b45-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00b45-110">bundleID</span><span class="sxs-lookup"><span data-stu-id="00b45-110">bundleID</span></span>|<span data-ttu-id="00b45-111">String</span><span class="sxs-lookup"><span data-stu-id="00b45-111">String</span></span>|<span data-ttu-id="00b45-112">要向其应用这些通知设置的应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="00b45-112">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="00b45-113">appName</span><span class="sxs-lookup"><span data-stu-id="00b45-113">appName</span></span>|<span data-ttu-id="00b45-114">String</span><span class="sxs-lookup"><span data-stu-id="00b45-114">String</span></span>|<span data-ttu-id="00b45-115">要与 bundleID 关联的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="00b45-115">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="00b45-116">发布者</span><span class="sxs-lookup"><span data-stu-id="00b45-116">publisher</span></span>|<span data-ttu-id="00b45-117">String</span><span class="sxs-lookup"><span data-stu-id="00b45-117">String</span></span>|<span data-ttu-id="00b45-118">要与 bundleID 关联的发布者。</span><span class="sxs-lookup"><span data-stu-id="00b45-118">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="00b45-119">enabled</span><span class="sxs-lookup"><span data-stu-id="00b45-119">enabled</span></span>|<span data-ttu-id="00b45-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="00b45-120">Boolean</span></span>|<span data-ttu-id="00b45-121">指示是否允许此应用使用通知。</span><span class="sxs-lookup"><span data-stu-id="00b45-121">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="00b45-122">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="00b45-122">showInNotificationCenter</span></span>|<span data-ttu-id="00b45-123">布尔值</span><span class="sxs-lookup"><span data-stu-id="00b45-123">Boolean</span></span>|<span data-ttu-id="00b45-124">指示是否可以在通知中心中显示通知。</span><span class="sxs-lookup"><span data-stu-id="00b45-124">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="00b45-125">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="00b45-125">showOnLockScreen</span></span>|<span data-ttu-id="00b45-126">布尔值</span><span class="sxs-lookup"><span data-stu-id="00b45-126">Boolean</span></span>|<span data-ttu-id="00b45-127">指示是否可以在锁定屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="00b45-127">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="00b45-128">alertType</span><span class="sxs-lookup"><span data-stu-id="00b45-128">alertType</span></span>|[<span data-ttu-id="00b45-129">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="00b45-129">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="00b45-130">指示此应用的通知的警报类型。</span><span class="sxs-lookup"><span data-stu-id="00b45-130">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="00b45-131">可取值为：`deviceDefault`、`banner`、`modal`、`none`。</span><span class="sxs-lookup"><span data-stu-id="00b45-131">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="00b45-132">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="00b45-132">badgesEnabled</span></span>|<span data-ttu-id="00b45-133">布尔值</span><span class="sxs-lookup"><span data-stu-id="00b45-133">Boolean</span></span>|<span data-ttu-id="00b45-134">指示是否允许此应用使用徽章。</span><span class="sxs-lookup"><span data-stu-id="00b45-134">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="00b45-135">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="00b45-135">soundsEnabled</span></span>|<span data-ttu-id="00b45-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="00b45-136">Boolean</span></span>|<span data-ttu-id="00b45-137">指示是否允许此应用使用声音。</span><span class="sxs-lookup"><span data-stu-id="00b45-137">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00b45-138">关系</span><span class="sxs-lookup"><span data-stu-id="00b45-138">Relationships</span></span>
<span data-ttu-id="00b45-139">无</span><span class="sxs-lookup"><span data-stu-id="00b45-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="00b45-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00b45-140">JSON Representation</span></span>
<span data-ttu-id="00b45-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00b45-141">Here is a JSON representation of the resource.</span></span>
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



