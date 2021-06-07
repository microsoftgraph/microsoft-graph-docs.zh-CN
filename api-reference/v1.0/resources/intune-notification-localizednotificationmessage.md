---
title: localizedNotificationMessage 资源类型
description: 指定区域设置的通知消息模板的文本内容。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 403952300d9072072b99f0dd58aa56e32ca22d69
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755712"
---
# <a name="localizednotificationmessage-resource-type"></a><span data-ttu-id="b77ef-103">localizedNotificationMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="b77ef-103">localizedNotificationMessage resource type</span></span>

<span data-ttu-id="b77ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b77ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b77ef-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b77ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b77ef-106">指定区域设置的通知消息模板的文本内容。</span><span class="sxs-lookup"><span data-stu-id="b77ef-106">The text content of a Notification Message Template for the specified locale.</span></span>

## <a name="methods"></a><span data-ttu-id="b77ef-107">Methods</span><span class="sxs-lookup"><span data-stu-id="b77ef-107">Methods</span></span>
|<span data-ttu-id="b77ef-108">方法</span><span class="sxs-lookup"><span data-stu-id="b77ef-108">Method</span></span>|<span data-ttu-id="b77ef-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b77ef-109">Return Type</span></span>|<span data-ttu-id="b77ef-110">Description</span><span class="sxs-lookup"><span data-stu-id="b77ef-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b77ef-111">列出 localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="b77ef-111">List localizedNotificationMessages</span></span>](../api/intune-notification-localizednotificationmessage-list.md)|<span data-ttu-id="b77ef-112">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b77ef-112">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="b77ef-113">列出 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b77ef-113">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>|
|[<span data-ttu-id="b77ef-114">获取 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="b77ef-114">Get localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-get.md)|[<span data-ttu-id="b77ef-115">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="b77ef-115">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="b77ef-116">读取 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b77ef-116">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="b77ef-117">创建 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="b77ef-117">Create localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-create.md)|[<span data-ttu-id="b77ef-118">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="b77ef-118">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="b77ef-119">创建新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b77ef-119">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="b77ef-120">删除 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="b77ef-120">Delete localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-delete.md)|<span data-ttu-id="b77ef-121">无</span><span class="sxs-lookup"><span data-stu-id="b77ef-121">None</span></span>|<span data-ttu-id="b77ef-122">删除 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="b77ef-122">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>|
|[<span data-ttu-id="b77ef-123">更新 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="b77ef-123">Update localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-update.md)|[<span data-ttu-id="b77ef-124">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="b77ef-124">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="b77ef-125">更新 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b77ef-125">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b77ef-126">属性</span><span class="sxs-lookup"><span data-stu-id="b77ef-126">Properties</span></span>
|<span data-ttu-id="b77ef-127">属性</span><span class="sxs-lookup"><span data-stu-id="b77ef-127">Property</span></span>|<span data-ttu-id="b77ef-128">类型</span><span class="sxs-lookup"><span data-stu-id="b77ef-128">Type</span></span>|<span data-ttu-id="b77ef-129">说明</span><span class="sxs-lookup"><span data-stu-id="b77ef-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b77ef-130">id</span><span class="sxs-lookup"><span data-stu-id="b77ef-130">id</span></span>|<span data-ttu-id="b77ef-131">String</span><span class="sxs-lookup"><span data-stu-id="b77ef-131">String</span></span>|<span data-ttu-id="b77ef-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b77ef-132">Key of the entity.</span></span>|
|<span data-ttu-id="b77ef-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b77ef-133">lastModifiedDateTime</span></span>|<span data-ttu-id="b77ef-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b77ef-134">DateTimeOffset</span></span>|<span data-ttu-id="b77ef-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b77ef-135">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="b77ef-136">locale</span><span class="sxs-lookup"><span data-stu-id="b77ef-136">locale</span></span>|<span data-ttu-id="b77ef-137">String</span><span class="sxs-lookup"><span data-stu-id="b77ef-137">String</span></span>|<span data-ttu-id="b77ef-138">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="b77ef-138">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="b77ef-139">subject</span><span class="sxs-lookup"><span data-stu-id="b77ef-139">subject</span></span>|<span data-ttu-id="b77ef-140">String</span><span class="sxs-lookup"><span data-stu-id="b77ef-140">String</span></span>|<span data-ttu-id="b77ef-141">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="b77ef-141">The Message Template Subject.</span></span>|
|<span data-ttu-id="b77ef-142">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="b77ef-142">messageTemplate</span></span>|<span data-ttu-id="b77ef-143">String</span><span class="sxs-lookup"><span data-stu-id="b77ef-143">String</span></span>|<span data-ttu-id="b77ef-144">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="b77ef-144">The Message Template content.</span></span>|
|<span data-ttu-id="b77ef-145">isDefault</span><span class="sxs-lookup"><span data-stu-id="b77ef-145">isDefault</span></span>|<span data-ttu-id="b77ef-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b77ef-146">Boolean</span></span>|<span data-ttu-id="b77ef-147">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="b77ef-147">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="b77ef-148">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="b77ef-148">This flag can only be set.</span></span> <span data-ttu-id="b77ef-149">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="b77ef-149">To unset, set this property to true on another Localized Notification Message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b77ef-150">关系</span><span class="sxs-lookup"><span data-stu-id="b77ef-150">Relationships</span></span>
<span data-ttu-id="b77ef-151">无</span><span class="sxs-lookup"><span data-stu-id="b77ef-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b77ef-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b77ef-152">JSON Representation</span></span>
<span data-ttu-id="b77ef-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b77ef-153">Here is a JSON representation of the resource.</span></span>
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




