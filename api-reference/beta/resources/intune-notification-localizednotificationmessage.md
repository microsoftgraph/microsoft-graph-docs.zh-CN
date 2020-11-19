---
title: localizedNotificationMessage 资源类型
description: 指定区域设置的通知消息模板的文本内容。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8ca80cccd82fefe9946027bdd8b52a6a63925322
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302416"
---
# <a name="localizednotificationmessage-resource-type"></a><span data-ttu-id="95d87-103">localizedNotificationMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="95d87-103">localizedNotificationMessage resource type</span></span>

<span data-ttu-id="95d87-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95d87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95d87-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95d87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95d87-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95d87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95d87-107">指定区域设置的通知消息模板的文本内容。</span><span class="sxs-lookup"><span data-stu-id="95d87-107">The text content of a Notification Message Template for the specified locale.</span></span>

## <a name="methods"></a><span data-ttu-id="95d87-108">Methods</span><span class="sxs-lookup"><span data-stu-id="95d87-108">Methods</span></span>
|<span data-ttu-id="95d87-109">方法</span><span class="sxs-lookup"><span data-stu-id="95d87-109">Method</span></span>|<span data-ttu-id="95d87-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="95d87-110">Return Type</span></span>|<span data-ttu-id="95d87-111">Description</span><span class="sxs-lookup"><span data-stu-id="95d87-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="95d87-112">列出 localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="95d87-112">List localizedNotificationMessages</span></span>](../api/intune-notification-localizednotificationmessage-list.md)|<span data-ttu-id="95d87-113">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="95d87-113">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="95d87-114">列出 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="95d87-114">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>|
|[<span data-ttu-id="95d87-115">获取 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="95d87-115">Get localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-get.md)|[<span data-ttu-id="95d87-116">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="95d87-116">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="95d87-117">读取 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="95d87-117">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="95d87-118">创建 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="95d87-118">Create localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-create.md)|[<span data-ttu-id="95d87-119">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="95d87-119">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="95d87-120">创建新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="95d87-120">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="95d87-121">删除 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="95d87-121">Delete localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-delete.md)|<span data-ttu-id="95d87-122">无</span><span class="sxs-lookup"><span data-stu-id="95d87-122">None</span></span>|<span data-ttu-id="95d87-123">删除 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="95d87-123">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>|
|[<span data-ttu-id="95d87-124">更新 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="95d87-124">Update localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-update.md)|[<span data-ttu-id="95d87-125">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="95d87-125">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="95d87-126">更新 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="95d87-126">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="95d87-127">属性</span><span class="sxs-lookup"><span data-stu-id="95d87-127">Properties</span></span>
|<span data-ttu-id="95d87-128">属性</span><span class="sxs-lookup"><span data-stu-id="95d87-128">Property</span></span>|<span data-ttu-id="95d87-129">类型</span><span class="sxs-lookup"><span data-stu-id="95d87-129">Type</span></span>|<span data-ttu-id="95d87-130">说明</span><span class="sxs-lookup"><span data-stu-id="95d87-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95d87-131">id</span><span class="sxs-lookup"><span data-stu-id="95d87-131">id</span></span>|<span data-ttu-id="95d87-132">字符串</span><span class="sxs-lookup"><span data-stu-id="95d87-132">String</span></span>|<span data-ttu-id="95d87-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="95d87-133">Key of the entity.</span></span>|
|<span data-ttu-id="95d87-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95d87-134">lastModifiedDateTime</span></span>|<span data-ttu-id="95d87-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95d87-135">DateTimeOffset</span></span>|<span data-ttu-id="95d87-136">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="95d87-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="95d87-137">locale</span><span class="sxs-lookup"><span data-stu-id="95d87-137">locale</span></span>|<span data-ttu-id="95d87-138">String</span><span class="sxs-lookup"><span data-stu-id="95d87-138">String</span></span>|<span data-ttu-id="95d87-139">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="95d87-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="95d87-140">subject</span><span class="sxs-lookup"><span data-stu-id="95d87-140">subject</span></span>|<span data-ttu-id="95d87-141">String</span><span class="sxs-lookup"><span data-stu-id="95d87-141">String</span></span>|<span data-ttu-id="95d87-142">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="95d87-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="95d87-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="95d87-143">messageTemplate</span></span>|<span data-ttu-id="95d87-144">String</span><span class="sxs-lookup"><span data-stu-id="95d87-144">String</span></span>|<span data-ttu-id="95d87-145">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="95d87-145">The Message Template content.</span></span>|
|<span data-ttu-id="95d87-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="95d87-146">isDefault</span></span>|<span data-ttu-id="95d87-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="95d87-147">Boolean</span></span>|<span data-ttu-id="95d87-148">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="95d87-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="95d87-149">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="95d87-149">This flag can only be set.</span></span> <span data-ttu-id="95d87-150">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="95d87-150">To unset, set this property to true on another Localized Notification Message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95d87-151">关系</span><span class="sxs-lookup"><span data-stu-id="95d87-151">Relationships</span></span>
<span data-ttu-id="95d87-152">无</span><span class="sxs-lookup"><span data-stu-id="95d87-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95d87-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95d87-153">JSON Representation</span></span>
<span data-ttu-id="95d87-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95d87-154">Here is a JSON representation of the resource.</span></span>
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




