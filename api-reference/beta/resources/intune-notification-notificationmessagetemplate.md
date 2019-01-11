---
title: notificationMessageTemplate 资源类型
description: " 部分。 使用 notificationMessageTemplate 对象创建自定义通知，以便管理员在配置非合规操作时进行选择。"
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 196f7809d288517807ef2b87bd8d577e902873d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844616"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="24a39-104">notificationMessageTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="24a39-104">notificationMessageTemplate resource type</span></span>

> <span data-ttu-id="24a39-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="24a39-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24a39-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="24a39-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24a39-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="24a39-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24a39-108">通知消息是要发送给最终用户的消息，这些最终用户被确定为不符合管理员定义的合规策略要求。</span><span class="sxs-lookup"><span data-stu-id="24a39-108">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="24a39-109">管理员会选择通知，并使用“非合规性操作”部分下的合规策略创建页面，在 Intune 管理控制台中进行配置。</span><span class="sxs-lookup"><span data-stu-id="24a39-109">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="24a39-110">使用 notificationMessageTemplate 对象创建自定义通知，以便管理员在配置非合规操作时进行选择。</span><span class="sxs-lookup"><span data-stu-id="24a39-110">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>
## <a name="methods"></a><span data-ttu-id="24a39-111">方法</span><span class="sxs-lookup"><span data-stu-id="24a39-111">Methods</span></span>
|<span data-ttu-id="24a39-112">方法</span><span class="sxs-lookup"><span data-stu-id="24a39-112">Method</span></span>|<span data-ttu-id="24a39-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="24a39-113">Return Type</span></span>|<span data-ttu-id="24a39-114">说明</span><span class="sxs-lookup"><span data-stu-id="24a39-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="24a39-115">List notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="24a39-115">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="24a39-116">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="24a39-116">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="24a39-117">列出 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="24a39-117">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="24a39-118">Get notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="24a39-118">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|[<span data-ttu-id="24a39-119">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="24a39-119">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="24a39-120">读取 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="24a39-120">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="24a39-121">创建 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="24a39-121">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|[<span data-ttu-id="24a39-122">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="24a39-122">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="24a39-123">创建新的 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="24a39-123">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="24a39-124">Delete notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="24a39-124">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="24a39-125">无</span><span class="sxs-lookup"><span data-stu-id="24a39-125">None</span></span>|<span data-ttu-id="24a39-126">删除 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="24a39-126">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="24a39-127">Update notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="24a39-127">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="24a39-128">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="24a39-128">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="24a39-129">更新 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="24a39-129">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="24a39-130">sendTestMessage 操作</span><span class="sxs-lookup"><span data-stu-id="24a39-130">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="24a39-131">无</span><span class="sxs-lookup"><span data-stu-id="24a39-131">None</span></span>|<span data-ttu-id="24a39-132">使用默认区域设置中指定的 notificationMessageTemplate 发送测试消息</span><span class="sxs-lookup"><span data-stu-id="24a39-132">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="24a39-133">属性</span><span class="sxs-lookup"><span data-stu-id="24a39-133">Properties</span></span>
|<span data-ttu-id="24a39-134">属性</span><span class="sxs-lookup"><span data-stu-id="24a39-134">Property</span></span>|<span data-ttu-id="24a39-135">类型</span><span class="sxs-lookup"><span data-stu-id="24a39-135">Type</span></span>|<span data-ttu-id="24a39-136">说明</span><span class="sxs-lookup"><span data-stu-id="24a39-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24a39-137">id</span><span class="sxs-lookup"><span data-stu-id="24a39-137">id</span></span>|<span data-ttu-id="24a39-138">String</span><span class="sxs-lookup"><span data-stu-id="24a39-138">String</span></span>|<span data-ttu-id="24a39-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="24a39-139">Key of the entity.</span></span>|
|<span data-ttu-id="24a39-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24a39-140">lastModifiedDateTime</span></span>|<span data-ttu-id="24a39-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24a39-141">DateTimeOffset</span></span>|<span data-ttu-id="24a39-142">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="24a39-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="24a39-143">displayName</span><span class="sxs-lookup"><span data-stu-id="24a39-143">displayName</span></span>|<span data-ttu-id="24a39-144">String</span><span class="sxs-lookup"><span data-stu-id="24a39-144">String</span></span>|<span data-ttu-id="24a39-145">通知消息模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="24a39-145">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="24a39-146">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="24a39-146">defaultLocale</span></span>|<span data-ttu-id="24a39-147">String</span><span class="sxs-lookup"><span data-stu-id="24a39-147">String</span></span>|<span data-ttu-id="24a39-148">请求的区域设置不可用时要回退到的默认区域设置。</span><span class="sxs-lookup"><span data-stu-id="24a39-148">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="24a39-149">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="24a39-149">brandingOptions</span></span>|[<span data-ttu-id="24a39-150">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="24a39-150">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="24a39-151">消息模板品牌选项。</span><span class="sxs-lookup"><span data-stu-id="24a39-151">The Message Template Branding Options.</span></span> <span data-ttu-id="24a39-152">已在 Intune 管理员控制台中定义品牌。</span><span class="sxs-lookup"><span data-stu-id="24a39-152">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="24a39-153">可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`。</span><span class="sxs-lookup"><span data-stu-id="24a39-153">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="24a39-154">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="24a39-154">roleScopeTagIds</span></span>|<span data-ttu-id="24a39-155">String 集合</span><span class="sxs-lookup"><span data-stu-id="24a39-155">String collection</span></span>|<span data-ttu-id="24a39-156">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="24a39-156">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24a39-157">Relationships</span><span class="sxs-lookup"><span data-stu-id="24a39-157">Relationships</span></span>
|<span data-ttu-id="24a39-158">关系</span><span class="sxs-lookup"><span data-stu-id="24a39-158">Relationship</span></span>|<span data-ttu-id="24a39-159">类型</span><span class="sxs-lookup"><span data-stu-id="24a39-159">Type</span></span>|<span data-ttu-id="24a39-160">说明</span><span class="sxs-lookup"><span data-stu-id="24a39-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24a39-161">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="24a39-161">localizedNotificationMessages</span></span>|<span data-ttu-id="24a39-162">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="24a39-162">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="24a39-163">此通知消息模板的本地化消息列表。</span><span class="sxs-lookup"><span data-stu-id="24a39-163">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24a39-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24a39-164">JSON Representation</span></span>
<span data-ttu-id="24a39-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24a39-165">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notificationMessageTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "defaultLocale": "String",
  "brandingOptions": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```





