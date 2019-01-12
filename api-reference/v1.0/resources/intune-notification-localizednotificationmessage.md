---
title: localizedNotificationMessage 资源类型
description: 指定区域设置的通知消息模板的文本内容。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90a8212abc0ae1cd2f504ffb5419e16a713aa2aa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946957"
---
# <a name="localizednotificationmessage-resource-type"></a><span data-ttu-id="0349c-103">localizedNotificationMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="0349c-103">localizedNotificationMessage resource type</span></span>

> <span data-ttu-id="0349c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0349c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0349c-105">指定区域设置的通知消息模板的文本内容。</span><span class="sxs-lookup"><span data-stu-id="0349c-105">The text content of a Notification Message Template for the specified locale.</span></span>
## <a name="methods"></a><span data-ttu-id="0349c-106">方法</span><span class="sxs-lookup"><span data-stu-id="0349c-106">Methods</span></span>
|<span data-ttu-id="0349c-107">方法</span><span class="sxs-lookup"><span data-stu-id="0349c-107">Method</span></span>|<span data-ttu-id="0349c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="0349c-108">Return Type</span></span>|<span data-ttu-id="0349c-109">说明</span><span class="sxs-lookup"><span data-stu-id="0349c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0349c-110">列出 localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="0349c-110">List localizedNotificationMessages</span></span>](../api/intune-notification-localizednotificationmessage-list.md)|<span data-ttu-id="0349c-111">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0349c-111">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="0349c-112">列出 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0349c-112">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>|
|[<span data-ttu-id="0349c-113">获取 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="0349c-113">Get localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-get.md)|[<span data-ttu-id="0349c-114">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="0349c-114">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="0349c-115">读取 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0349c-115">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="0349c-116">创建 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="0349c-116">Create localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-create.md)|[<span data-ttu-id="0349c-117">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="0349c-117">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="0349c-118">创建新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0349c-118">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="0349c-119">删除 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="0349c-119">Delete localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-delete.md)|<span data-ttu-id="0349c-120">无</span><span class="sxs-lookup"><span data-stu-id="0349c-120">None</span></span>|<span data-ttu-id="0349c-121">删除 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="0349c-121">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>|
|[<span data-ttu-id="0349c-122">更新 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="0349c-122">Update localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-update.md)|[<span data-ttu-id="0349c-123">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="0349c-123">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="0349c-124">更新 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0349c-124">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0349c-125">属性</span><span class="sxs-lookup"><span data-stu-id="0349c-125">Properties</span></span>
|<span data-ttu-id="0349c-126">属性</span><span class="sxs-lookup"><span data-stu-id="0349c-126">Property</span></span>|<span data-ttu-id="0349c-127">类型</span><span class="sxs-lookup"><span data-stu-id="0349c-127">Type</span></span>|<span data-ttu-id="0349c-128">说明</span><span class="sxs-lookup"><span data-stu-id="0349c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0349c-129">id</span><span class="sxs-lookup"><span data-stu-id="0349c-129">id</span></span>|<span data-ttu-id="0349c-130">String</span><span class="sxs-lookup"><span data-stu-id="0349c-130">String</span></span>|<span data-ttu-id="0349c-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0349c-131">Key of the entity.</span></span>|
|<span data-ttu-id="0349c-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0349c-132">lastModifiedDateTime</span></span>|<span data-ttu-id="0349c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0349c-133">DateTimeOffset</span></span>|<span data-ttu-id="0349c-134">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0349c-134">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="0349c-135">locale</span><span class="sxs-lookup"><span data-stu-id="0349c-135">locale</span></span>|<span data-ttu-id="0349c-136">String</span><span class="sxs-lookup"><span data-stu-id="0349c-136">String</span></span>|<span data-ttu-id="0349c-137">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="0349c-137">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="0349c-138">subject</span><span class="sxs-lookup"><span data-stu-id="0349c-138">subject</span></span>|<span data-ttu-id="0349c-139">String</span><span class="sxs-lookup"><span data-stu-id="0349c-139">String</span></span>|<span data-ttu-id="0349c-140">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="0349c-140">The Message Template Subject.</span></span>|
|<span data-ttu-id="0349c-141">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="0349c-141">messageTemplate</span></span>|<span data-ttu-id="0349c-142">String</span><span class="sxs-lookup"><span data-stu-id="0349c-142">String</span></span>|<span data-ttu-id="0349c-143">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="0349c-143">The Message Template content.</span></span>|
|<span data-ttu-id="0349c-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="0349c-144">isDefault</span></span>|<span data-ttu-id="0349c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0349c-145">Boolean</span></span>|<span data-ttu-id="0349c-146">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="0349c-146">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="0349c-147">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="0349c-147">This flag can only be set.</span></span> <span data-ttu-id="0349c-148">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="0349c-148">To unset, set this property to true on another Localized Notification Message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0349c-149">关系</span><span class="sxs-lookup"><span data-stu-id="0349c-149">Relationships</span></span>
<span data-ttu-id="0349c-150">无</span><span class="sxs-lookup"><span data-stu-id="0349c-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0349c-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0349c-151">JSON Representation</span></span>
<span data-ttu-id="0349c-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0349c-152">Here is a JSON representation of the resource.</span></span>
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



