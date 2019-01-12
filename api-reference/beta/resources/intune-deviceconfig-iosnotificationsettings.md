---
title: iosNotificationSettings 资源类型
description: 说明通知设置的项。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 242a15d4b636cf73f0e9a9f29a3f53ce17f2fd00
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972976"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="6b178-103">iosNotificationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b178-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="6b178-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6b178-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b178-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6b178-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b178-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6b178-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b178-107">说明通知设置的项。</span><span class="sxs-lookup"><span data-stu-id="6b178-107">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="6b178-108">属性</span><span class="sxs-lookup"><span data-stu-id="6b178-108">Properties</span></span>
|<span data-ttu-id="6b178-109">属性</span><span class="sxs-lookup"><span data-stu-id="6b178-109">Property</span></span>|<span data-ttu-id="6b178-110">类型</span><span class="sxs-lookup"><span data-stu-id="6b178-110">Type</span></span>|<span data-ttu-id="6b178-111">说明</span><span class="sxs-lookup"><span data-stu-id="6b178-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b178-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="6b178-112">bundleID</span></span>|<span data-ttu-id="6b178-113">String</span><span class="sxs-lookup"><span data-stu-id="6b178-113">String</span></span>|<span data-ttu-id="6b178-114">要向其应用这些通知设置的应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="6b178-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="6b178-115">appName</span><span class="sxs-lookup"><span data-stu-id="6b178-115">appName</span></span>|<span data-ttu-id="6b178-116">String</span><span class="sxs-lookup"><span data-stu-id="6b178-116">String</span></span>|<span data-ttu-id="6b178-117">要与 bundleID 关联的应用程序名称。</span><span class="sxs-lookup"><span data-stu-id="6b178-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="6b178-118">发布者</span><span class="sxs-lookup"><span data-stu-id="6b178-118">publisher</span></span>|<span data-ttu-id="6b178-119">String</span><span class="sxs-lookup"><span data-stu-id="6b178-119">String</span></span>|<span data-ttu-id="6b178-120">要与 bundleID 关联的发布者。</span><span class="sxs-lookup"><span data-stu-id="6b178-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="6b178-121">enabled</span><span class="sxs-lookup"><span data-stu-id="6b178-121">enabled</span></span>|<span data-ttu-id="6b178-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="6b178-122">Boolean</span></span>|<span data-ttu-id="6b178-123">指示是否允许此应用使用通知。</span><span class="sxs-lookup"><span data-stu-id="6b178-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="6b178-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="6b178-124">showInNotificationCenter</span></span>|<span data-ttu-id="6b178-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="6b178-125">Boolean</span></span>|<span data-ttu-id="6b178-126">指示是否可以在通知中心中显示通知。</span><span class="sxs-lookup"><span data-stu-id="6b178-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="6b178-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="6b178-127">showOnLockScreen</span></span>|<span data-ttu-id="6b178-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="6b178-128">Boolean</span></span>|<span data-ttu-id="6b178-129">指示是否可以在锁定屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="6b178-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="6b178-130">alertType</span><span class="sxs-lookup"><span data-stu-id="6b178-130">alertType</span></span>|[<span data-ttu-id="6b178-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="6b178-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="6b178-132">指示此应用的通知的警报类型。</span><span class="sxs-lookup"><span data-stu-id="6b178-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="6b178-133">可取值为：`deviceDefault`、`banner`、`modal`、`none`。</span><span class="sxs-lookup"><span data-stu-id="6b178-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="6b178-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="6b178-134">badgesEnabled</span></span>|<span data-ttu-id="6b178-135">布尔值</span><span class="sxs-lookup"><span data-stu-id="6b178-135">Boolean</span></span>|<span data-ttu-id="6b178-136">指示是否允许此应用使用徽章。</span><span class="sxs-lookup"><span data-stu-id="6b178-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="6b178-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="6b178-137">soundsEnabled</span></span>|<span data-ttu-id="6b178-138">布尔值</span><span class="sxs-lookup"><span data-stu-id="6b178-138">Boolean</span></span>|<span data-ttu-id="6b178-139">指示是否允许此应用使用声音。</span><span class="sxs-lookup"><span data-stu-id="6b178-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b178-140">关系</span><span class="sxs-lookup"><span data-stu-id="6b178-140">Relationships</span></span>
<span data-ttu-id="6b178-141">无</span><span class="sxs-lookup"><span data-stu-id="6b178-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6b178-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b178-142">JSON Representation</span></span>
<span data-ttu-id="6b178-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b178-143">Here is a JSON representation of the resource.</span></span>
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





