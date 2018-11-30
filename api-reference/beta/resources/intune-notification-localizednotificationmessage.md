---
title: localizedNotificationMessage 资源类型
description: 指定区域设置的通知消息模板的文本内容。
ms.openlocfilehash: 34daebc90ca6a58d28b351eebcfcc3a29b8b5021
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046991"
---
# <a name="localizednotificationmessage-resource-type"></a><span data-ttu-id="1b3af-103">localizedNotificationMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b3af-103">localizedNotificationMessage resource type</span></span>

> <span data-ttu-id="1b3af-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1b3af-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b3af-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1b3af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b3af-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1b3af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b3af-107">指定区域设置的通知消息模板的文本内容。</span><span class="sxs-lookup"><span data-stu-id="1b3af-107">The text content of a Notification Message Template for the specified locale.</span></span>
## <a name="methods"></a><span data-ttu-id="1b3af-108">方法</span><span class="sxs-lookup"><span data-stu-id="1b3af-108">Methods</span></span>
|<span data-ttu-id="1b3af-109">方法</span><span class="sxs-lookup"><span data-stu-id="1b3af-109">Method</span></span>|<span data-ttu-id="1b3af-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1b3af-110">Return Type</span></span>|<span data-ttu-id="1b3af-111">说明</span><span class="sxs-lookup"><span data-stu-id="1b3af-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1b3af-112">列出 localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="1b3af-112">List localizedNotificationMessages</span></span>](../api/intune-notification-localizednotificationmessage-list.md)|<span data-ttu-id="1b3af-113">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1b3af-113">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="1b3af-114">列出 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1b3af-114">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>|
|[<span data-ttu-id="1b3af-115">获取 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="1b3af-115">Get localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-get.md)|[<span data-ttu-id="1b3af-116">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="1b3af-116">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="1b3af-117">读取 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1b3af-117">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="1b3af-118">创建 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="1b3af-118">Create localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-create.md)|[<span data-ttu-id="1b3af-119">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="1b3af-119">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="1b3af-120">创建新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1b3af-120">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="1b3af-121">删除 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="1b3af-121">Delete localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-delete.md)|<span data-ttu-id="1b3af-122">无</span><span class="sxs-lookup"><span data-stu-id="1b3af-122">None</span></span>|<span data-ttu-id="1b3af-123">删除 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="1b3af-123">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>|
|[<span data-ttu-id="1b3af-124">更新 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="1b3af-124">Update localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-update.md)|[<span data-ttu-id="1b3af-125">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="1b3af-125">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="1b3af-126">更新 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1b3af-126">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1b3af-127">属性</span><span class="sxs-lookup"><span data-stu-id="1b3af-127">Properties</span></span>
|<span data-ttu-id="1b3af-128">属性</span><span class="sxs-lookup"><span data-stu-id="1b3af-128">Property</span></span>|<span data-ttu-id="1b3af-129">类型</span><span class="sxs-lookup"><span data-stu-id="1b3af-129">Type</span></span>|<span data-ttu-id="1b3af-130">说明</span><span class="sxs-lookup"><span data-stu-id="1b3af-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b3af-131">id</span><span class="sxs-lookup"><span data-stu-id="1b3af-131">id</span></span>|<span data-ttu-id="1b3af-132">String</span><span class="sxs-lookup"><span data-stu-id="1b3af-132">String</span></span>|<span data-ttu-id="1b3af-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1b3af-133">Key of the entity.</span></span>|
|<span data-ttu-id="1b3af-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b3af-134">lastModifiedDateTime</span></span>|<span data-ttu-id="1b3af-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b3af-135">DateTimeOffset</span></span>|<span data-ttu-id="1b3af-136">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1b3af-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="1b3af-137">locale</span><span class="sxs-lookup"><span data-stu-id="1b3af-137">locale</span></span>|<span data-ttu-id="1b3af-138">String</span><span class="sxs-lookup"><span data-stu-id="1b3af-138">String</span></span>|<span data-ttu-id="1b3af-139">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="1b3af-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="1b3af-140">subject</span><span class="sxs-lookup"><span data-stu-id="1b3af-140">subject</span></span>|<span data-ttu-id="1b3af-141">String</span><span class="sxs-lookup"><span data-stu-id="1b3af-141">String</span></span>|<span data-ttu-id="1b3af-142">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="1b3af-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="1b3af-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="1b3af-143">messageTemplate</span></span>|<span data-ttu-id="1b3af-144">String</span><span class="sxs-lookup"><span data-stu-id="1b3af-144">String</span></span>|<span data-ttu-id="1b3af-145">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="1b3af-145">The Message Template content.</span></span>|
|<span data-ttu-id="1b3af-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="1b3af-146">isDefault</span></span>|<span data-ttu-id="1b3af-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b3af-147">Boolean</span></span>|<span data-ttu-id="1b3af-148">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="1b3af-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="1b3af-149">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="1b3af-149">This flag can only be set.</span></span> <span data-ttu-id="1b3af-150">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="1b3af-150">To unset, set this property to true on another Localized Notification Message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b3af-151">关系</span><span class="sxs-lookup"><span data-stu-id="1b3af-151">Relationships</span></span>
<span data-ttu-id="1b3af-152">无</span><span class="sxs-lookup"><span data-stu-id="1b3af-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1b3af-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b3af-153">JSON Representation</span></span>
<span data-ttu-id="1b3af-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b3af-154">Here is a JSON representation of the resource.</span></span>
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





