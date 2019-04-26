---
title: localizedNotificationMessage 资源类型
description: 指定区域设置的通知消息模板的文本内容。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92d4599504eba2e658131276d1a27ab9602025c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572085"
---
# <a name="localizednotificationmessage-resource-type"></a><span data-ttu-id="9e91f-103">localizedNotificationMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e91f-103">localizedNotificationMessage resource type</span></span>

> <span data-ttu-id="9e91f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9e91f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e91f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e91f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e91f-106">指定区域设置的通知消息模板的文本内容。</span><span class="sxs-lookup"><span data-stu-id="9e91f-106">The text content of a Notification Message Template for the specified locale.</span></span>

## <a name="methods"></a><span data-ttu-id="9e91f-107">方法</span><span class="sxs-lookup"><span data-stu-id="9e91f-107">Methods</span></span>
|<span data-ttu-id="9e91f-108">方法</span><span class="sxs-lookup"><span data-stu-id="9e91f-108">Method</span></span>|<span data-ttu-id="9e91f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9e91f-109">Return Type</span></span>|<span data-ttu-id="9e91f-110">说明</span><span class="sxs-lookup"><span data-stu-id="9e91f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9e91f-111">列出 localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="9e91f-111">List localizedNotificationMessages</span></span>](../api/intune-notification-localizednotificationmessage-list.md)|<span data-ttu-id="9e91f-112">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e91f-112">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="9e91f-113">列出 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9e91f-113">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>|
|[<span data-ttu-id="9e91f-114">获取 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="9e91f-114">Get localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-get.md)|[<span data-ttu-id="9e91f-115">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="9e91f-115">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="9e91f-116">读取 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9e91f-116">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="9e91f-117">创建 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="9e91f-117">Create localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-create.md)|[<span data-ttu-id="9e91f-118">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="9e91f-118">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="9e91f-119">创建新的 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9e91f-119">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="9e91f-120">删除 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="9e91f-120">Delete localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-delete.md)|<span data-ttu-id="9e91f-121">无</span><span class="sxs-lookup"><span data-stu-id="9e91f-121">None</span></span>|<span data-ttu-id="9e91f-122">删除 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="9e91f-122">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>|
|[<span data-ttu-id="9e91f-123">更新 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="9e91f-123">Update localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-update.md)|[<span data-ttu-id="9e91f-124">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="9e91f-124">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="9e91f-125">更新 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9e91f-125">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9e91f-126">属性</span><span class="sxs-lookup"><span data-stu-id="9e91f-126">Properties</span></span>
|<span data-ttu-id="9e91f-127">属性</span><span class="sxs-lookup"><span data-stu-id="9e91f-127">Property</span></span>|<span data-ttu-id="9e91f-128">类型</span><span class="sxs-lookup"><span data-stu-id="9e91f-128">Type</span></span>|<span data-ttu-id="9e91f-129">说明</span><span class="sxs-lookup"><span data-stu-id="9e91f-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e91f-130">id</span><span class="sxs-lookup"><span data-stu-id="9e91f-130">id</span></span>|<span data-ttu-id="9e91f-131">字符串</span><span class="sxs-lookup"><span data-stu-id="9e91f-131">String</span></span>|<span data-ttu-id="9e91f-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9e91f-132">Key of the entity.</span></span>|
|<span data-ttu-id="9e91f-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e91f-133">lastModifiedDateTime</span></span>|<span data-ttu-id="9e91f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e91f-134">DateTimeOffset</span></span>|<span data-ttu-id="9e91f-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9e91f-135">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="9e91f-136">locale</span><span class="sxs-lookup"><span data-stu-id="9e91f-136">locale</span></span>|<span data-ttu-id="9e91f-137">String</span><span class="sxs-lookup"><span data-stu-id="9e91f-137">String</span></span>|<span data-ttu-id="9e91f-138">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="9e91f-138">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="9e91f-139">主题</span><span class="sxs-lookup"><span data-stu-id="9e91f-139">subject</span></span>|<span data-ttu-id="9e91f-140">String</span><span class="sxs-lookup"><span data-stu-id="9e91f-140">String</span></span>|<span data-ttu-id="9e91f-141">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="9e91f-141">The Message Template Subject.</span></span>|
|<span data-ttu-id="9e91f-142">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="9e91f-142">messageTemplate</span></span>|<span data-ttu-id="9e91f-143">String</span><span class="sxs-lookup"><span data-stu-id="9e91f-143">String</span></span>|<span data-ttu-id="9e91f-144">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="9e91f-144">The Message Template content.</span></span>|
|<span data-ttu-id="9e91f-145">isDefault</span><span class="sxs-lookup"><span data-stu-id="9e91f-145">isDefault</span></span>|<span data-ttu-id="9e91f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e91f-146">Boolean</span></span>|<span data-ttu-id="9e91f-147">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="9e91f-147">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="9e91f-148">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="9e91f-148">This flag can only be set.</span></span> <span data-ttu-id="9e91f-149">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="9e91f-149">To unset, set this property to true on another Localized Notification Message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e91f-150">关系</span><span class="sxs-lookup"><span data-stu-id="9e91f-150">Relationships</span></span>
<span data-ttu-id="9e91f-151">无</span><span class="sxs-lookup"><span data-stu-id="9e91f-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e91f-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e91f-152">JSON Representation</span></span>
<span data-ttu-id="9e91f-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e91f-153">Here is a JSON representation of the resource.</span></span>
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





