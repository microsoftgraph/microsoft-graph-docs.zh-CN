---
title: localizedNotificationMessage 资源类型
description: 指定区域设置的通知消息模板的文本内容。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec08211781dc5fb1ae499d7a4fd8436660cc4e84
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251494"
---
# <a name="localizednotificationmessage-resource-type"></a><span data-ttu-id="8dcae-103">localizedNotificationMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="8dcae-103">localizedNotificationMessage resource type</span></span>

> <span data-ttu-id="8dcae-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8dcae-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dcae-105">指定区域设置的通知消息模板的文本内容。</span><span class="sxs-lookup"><span data-stu-id="8dcae-105">The text content of a Notification Message Template for the specified locale.</span></span>

## <a name="methods"></a><span data-ttu-id="8dcae-106">方法</span><span class="sxs-lookup"><span data-stu-id="8dcae-106">Methods</span></span>
|<span data-ttu-id="8dcae-107">方法</span><span class="sxs-lookup"><span data-stu-id="8dcae-107">Method</span></span>|<span data-ttu-id="8dcae-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8dcae-108">Return Type</span></span>|<span data-ttu-id="8dcae-109">说明</span><span class="sxs-lookup"><span data-stu-id="8dcae-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8dcae-110">列出 localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="8dcae-110">List localizedNotificationMessages</span></span>](../api/intune-notification-localizednotificationmessage-list.md)|<span data-ttu-id="8dcae-111">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8dcae-111">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="8dcae-112">列出 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8dcae-112">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>|
|[<span data-ttu-id="8dcae-113">获取 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="8dcae-113">Get localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-get.md)|[<span data-ttu-id="8dcae-114">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="8dcae-114">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="8dcae-115">读取 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8dcae-115">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="8dcae-116">创建 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="8dcae-116">Create localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-create.md)|[<span data-ttu-id="8dcae-117">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="8dcae-117">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="8dcae-118">创建新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8dcae-118">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="8dcae-119">删除 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="8dcae-119">Delete localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-delete.md)|<span data-ttu-id="8dcae-120">无</span><span class="sxs-lookup"><span data-stu-id="8dcae-120">None</span></span>|<span data-ttu-id="8dcae-121">删除 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="8dcae-121">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>|
|[<span data-ttu-id="8dcae-122">更新 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="8dcae-122">Update localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-update.md)|[<span data-ttu-id="8dcae-123">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="8dcae-123">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="8dcae-124">更新 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8dcae-124">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8dcae-125">属性</span><span class="sxs-lookup"><span data-stu-id="8dcae-125">Properties</span></span>
|<span data-ttu-id="8dcae-126">属性</span><span class="sxs-lookup"><span data-stu-id="8dcae-126">Property</span></span>|<span data-ttu-id="8dcae-127">类型</span><span class="sxs-lookup"><span data-stu-id="8dcae-127">Type</span></span>|<span data-ttu-id="8dcae-128">说明</span><span class="sxs-lookup"><span data-stu-id="8dcae-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8dcae-129">id</span><span class="sxs-lookup"><span data-stu-id="8dcae-129">id</span></span>|<span data-ttu-id="8dcae-130">String</span><span class="sxs-lookup"><span data-stu-id="8dcae-130">String</span></span>|<span data-ttu-id="8dcae-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8dcae-131">Key of the entity.</span></span>|
|<span data-ttu-id="8dcae-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8dcae-132">lastModifiedDateTime</span></span>|<span data-ttu-id="8dcae-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dcae-133">DateTimeOffset</span></span>|<span data-ttu-id="8dcae-134">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8dcae-134">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8dcae-135">locale</span><span class="sxs-lookup"><span data-stu-id="8dcae-135">locale</span></span>|<span data-ttu-id="8dcae-136">String</span><span class="sxs-lookup"><span data-stu-id="8dcae-136">String</span></span>|<span data-ttu-id="8dcae-137">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="8dcae-137">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="8dcae-138">subject</span><span class="sxs-lookup"><span data-stu-id="8dcae-138">subject</span></span>|<span data-ttu-id="8dcae-139">String</span><span class="sxs-lookup"><span data-stu-id="8dcae-139">String</span></span>|<span data-ttu-id="8dcae-140">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="8dcae-140">The Message Template Subject.</span></span>|
|<span data-ttu-id="8dcae-141">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="8dcae-141">messageTemplate</span></span>|<span data-ttu-id="8dcae-142">String</span><span class="sxs-lookup"><span data-stu-id="8dcae-142">String</span></span>|<span data-ttu-id="8dcae-143">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="8dcae-143">The Message Template content.</span></span>|
|<span data-ttu-id="8dcae-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="8dcae-144">isDefault</span></span>|<span data-ttu-id="8dcae-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8dcae-145">Boolean</span></span>|<span data-ttu-id="8dcae-146">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="8dcae-146">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="8dcae-147">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="8dcae-147">This flag can only be set.</span></span> <span data-ttu-id="8dcae-148">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="8dcae-148">To unset, set this property to true on another Localized Notification Message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8dcae-149">关系</span><span class="sxs-lookup"><span data-stu-id="8dcae-149">Relationships</span></span>
<span data-ttu-id="8dcae-150">无</span><span class="sxs-lookup"><span data-stu-id="8dcae-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8dcae-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8dcae-151">JSON Representation</span></span>
<span data-ttu-id="8dcae-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8dcae-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.localizedNotificationMessage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "locale": "String",
  "subject": "String",
  "messageTemplate": "String",
  "isDefault": true
}
```



