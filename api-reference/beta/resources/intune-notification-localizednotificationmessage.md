---
title: localizedNotificationMessage 资源类型
description: 指定区域设置的通知消息模板的文本内容。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91d737c999baf0f0268ba60ae1fa6c71c4539d22
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43419182"
---
# <a name="localizednotificationmessage-resource-type"></a><span data-ttu-id="bb4e3-103">localizedNotificationMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb4e3-103">localizedNotificationMessage resource type</span></span>

<span data-ttu-id="bb4e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb4e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb4e3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb4e3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb4e3-107">指定区域设置的通知消息模板的文本内容。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-107">The text content of a Notification Message Template for the specified locale.</span></span>

## <a name="methods"></a><span data-ttu-id="bb4e3-108">方法</span><span class="sxs-lookup"><span data-stu-id="bb4e3-108">Methods</span></span>
|<span data-ttu-id="bb4e3-109">方法</span><span class="sxs-lookup"><span data-stu-id="bb4e3-109">Method</span></span>|<span data-ttu-id="bb4e3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="bb4e3-110">Return Type</span></span>|<span data-ttu-id="bb4e3-111">说明</span><span class="sxs-lookup"><span data-stu-id="bb4e3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb4e3-112">列出 localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="bb4e3-112">List localizedNotificationMessages</span></span>](../api/intune-notification-localizednotificationmessage-list.md)|<span data-ttu-id="bb4e3-113">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bb4e3-113">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="bb4e3-114">列出 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-114">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>|
|[<span data-ttu-id="bb4e3-115">获取 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="bb4e3-115">Get localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-get.md)|[<span data-ttu-id="bb4e3-116">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="bb4e3-116">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="bb4e3-117">读取 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-117">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="bb4e3-118">创建 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="bb4e3-118">Create localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-create.md)|[<span data-ttu-id="bb4e3-119">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="bb4e3-119">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="bb4e3-120">创建新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-120">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="bb4e3-121">删除 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="bb4e3-121">Delete localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-delete.md)|<span data-ttu-id="bb4e3-122">无</span><span class="sxs-lookup"><span data-stu-id="bb4e3-122">None</span></span>|<span data-ttu-id="bb4e3-123">删除 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-123">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>|
|[<span data-ttu-id="bb4e3-124">更新 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="bb4e3-124">Update localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-update.md)|[<span data-ttu-id="bb4e3-125">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="bb4e3-125">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="bb4e3-126">更新 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-126">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bb4e3-127">属性</span><span class="sxs-lookup"><span data-stu-id="bb4e3-127">Properties</span></span>
|<span data-ttu-id="bb4e3-128">属性</span><span class="sxs-lookup"><span data-stu-id="bb4e3-128">Property</span></span>|<span data-ttu-id="bb4e3-129">类型</span><span class="sxs-lookup"><span data-stu-id="bb4e3-129">Type</span></span>|<span data-ttu-id="bb4e3-130">说明</span><span class="sxs-lookup"><span data-stu-id="bb4e3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb4e3-131">id</span><span class="sxs-lookup"><span data-stu-id="bb4e3-131">id</span></span>|<span data-ttu-id="bb4e3-132">字符串</span><span class="sxs-lookup"><span data-stu-id="bb4e3-132">String</span></span>|<span data-ttu-id="bb4e3-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-133">Key of the entity.</span></span>|
|<span data-ttu-id="bb4e3-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb4e3-134">lastModifiedDateTime</span></span>|<span data-ttu-id="bb4e3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb4e3-135">DateTimeOffset</span></span>|<span data-ttu-id="bb4e3-136">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="bb4e3-137">locale</span><span class="sxs-lookup"><span data-stu-id="bb4e3-137">locale</span></span>|<span data-ttu-id="bb4e3-138">String</span><span class="sxs-lookup"><span data-stu-id="bb4e3-138">String</span></span>|<span data-ttu-id="bb4e3-139">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="bb4e3-140">subject</span><span class="sxs-lookup"><span data-stu-id="bb4e3-140">subject</span></span>|<span data-ttu-id="bb4e3-141">String</span><span class="sxs-lookup"><span data-stu-id="bb4e3-141">String</span></span>|<span data-ttu-id="bb4e3-142">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="bb4e3-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="bb4e3-143">messageTemplate</span></span>|<span data-ttu-id="bb4e3-144">String</span><span class="sxs-lookup"><span data-stu-id="bb4e3-144">String</span></span>|<span data-ttu-id="bb4e3-145">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-145">The Message Template content.</span></span>|
|<span data-ttu-id="bb4e3-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="bb4e3-146">isDefault</span></span>|<span data-ttu-id="bb4e3-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb4e3-147">Boolean</span></span>|<span data-ttu-id="bb4e3-148">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="bb4e3-149">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-149">This flag can only be set.</span></span> <span data-ttu-id="bb4e3-150">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-150">To unset, set this property to true on another Localized Notification Message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb4e3-151">关系</span><span class="sxs-lookup"><span data-stu-id="bb4e3-151">Relationships</span></span>
<span data-ttu-id="bb4e3-152">无</span><span class="sxs-lookup"><span data-stu-id="bb4e3-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb4e3-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb4e3-153">JSON Representation</span></span>
<span data-ttu-id="bb4e3-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb4e3-154">Here is a JSON representation of the resource.</span></span>
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



