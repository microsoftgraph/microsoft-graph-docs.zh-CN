---
title: notificationMessageTemplate 资源类型
description: 通知消息是要发送给最终用户的消息，这些最终用户被确定为不符合管理员定义的合规策略要求。 管理员会选择通知，并使用“非合规性操作”部分下的合规策略创建页面，在 Intune 管理控制台中进行配置。 使用 notificationMessageTemplate 对象创建自定义通知，以便管理员在配置非合规操作时进行选择。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4dc7cb92cfbe87cd98b24614cd9fa31f4f81bb38
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574475"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="ec663-105">notificationMessageTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec663-105">notificationMessageTemplate resource type</span></span>

> <span data-ttu-id="ec663-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ec663-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec663-107">通知消息是要发送给最终用户的消息，这些最终用户被确定为不符合管理员定义的合规策略要求。</span><span class="sxs-lookup"><span data-stu-id="ec663-107">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="ec663-108">管理员会选择通知，并使用“非合规性操作”部分下的合规策略创建页面，在 Intune 管理控制台中进行配置。</span><span class="sxs-lookup"><span data-stu-id="ec663-108">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="ec663-109">使用 notificationMessageTemplate 对象创建自定义通知，以便管理员在配置非合规操作时进行选择。</span><span class="sxs-lookup"><span data-stu-id="ec663-109">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>

## <a name="methods"></a><span data-ttu-id="ec663-110">方法</span><span class="sxs-lookup"><span data-stu-id="ec663-110">Methods</span></span>
|<span data-ttu-id="ec663-111">方法</span><span class="sxs-lookup"><span data-stu-id="ec663-111">Method</span></span>|<span data-ttu-id="ec663-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="ec663-112">Return Type</span></span>|<span data-ttu-id="ec663-113">说明</span><span class="sxs-lookup"><span data-stu-id="ec663-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ec663-114">List notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="ec663-114">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="ec663-115">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ec663-115">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="ec663-116">列出 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ec663-116">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="ec663-117">Get notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ec663-117">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|[<span data-ttu-id="ec663-118">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ec663-118">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="ec663-119">读取 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ec663-119">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="ec663-120">创建 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ec663-120">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|[<span data-ttu-id="ec663-121">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ec663-121">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="ec663-122">创建新的 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ec663-122">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="ec663-123">Delete notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ec663-123">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="ec663-124">无</span><span class="sxs-lookup"><span data-stu-id="ec663-124">None</span></span>|<span data-ttu-id="ec663-125">删除 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="ec663-125">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="ec663-126">Update notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ec663-126">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="ec663-127">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="ec663-127">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="ec663-128">更新 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ec663-128">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="ec663-129">sendTestMessage 操作</span><span class="sxs-lookup"><span data-stu-id="ec663-129">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="ec663-130">无</span><span class="sxs-lookup"><span data-stu-id="ec663-130">None</span></span>|<span data-ttu-id="ec663-131">使用默认区域设置中指定的 notificationMessageTemplate 发送测试消息</span><span class="sxs-lookup"><span data-stu-id="ec663-131">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="ec663-132">属性</span><span class="sxs-lookup"><span data-stu-id="ec663-132">Properties</span></span>
|<span data-ttu-id="ec663-133">属性</span><span class="sxs-lookup"><span data-stu-id="ec663-133">Property</span></span>|<span data-ttu-id="ec663-134">类型</span><span class="sxs-lookup"><span data-stu-id="ec663-134">Type</span></span>|<span data-ttu-id="ec663-135">说明</span><span class="sxs-lookup"><span data-stu-id="ec663-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec663-136">id</span><span class="sxs-lookup"><span data-stu-id="ec663-136">id</span></span>|<span data-ttu-id="ec663-137">String</span><span class="sxs-lookup"><span data-stu-id="ec663-137">String</span></span>|<span data-ttu-id="ec663-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ec663-138">Key of the entity.</span></span>|
|<span data-ttu-id="ec663-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec663-139">lastModifiedDateTime</span></span>|<span data-ttu-id="ec663-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec663-140">DateTimeOffset</span></span>|<span data-ttu-id="ec663-141">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ec663-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ec663-142">displayName</span><span class="sxs-lookup"><span data-stu-id="ec663-142">displayName</span></span>|<span data-ttu-id="ec663-143">字符串</span><span class="sxs-lookup"><span data-stu-id="ec663-143">String</span></span>|<span data-ttu-id="ec663-144">通知消息模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ec663-144">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="ec663-145">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="ec663-145">defaultLocale</span></span>|<span data-ttu-id="ec663-146">String</span><span class="sxs-lookup"><span data-stu-id="ec663-146">String</span></span>|<span data-ttu-id="ec663-147">请求的区域设置不可用时要回退到的默认区域设置。</span><span class="sxs-lookup"><span data-stu-id="ec663-147">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="ec663-148">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="ec663-148">brandingOptions</span></span>|[<span data-ttu-id="ec663-149">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="ec663-149">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="ec663-150">消息模板品牌选项。</span><span class="sxs-lookup"><span data-stu-id="ec663-150">The Message Template Branding Options.</span></span> <span data-ttu-id="ec663-151">已在 Intune 管理员控制台中定义品牌。</span><span class="sxs-lookup"><span data-stu-id="ec663-151">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="ec663-152">可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`。</span><span class="sxs-lookup"><span data-stu-id="ec663-152">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec663-153">关系</span><span class="sxs-lookup"><span data-stu-id="ec663-153">Relationships</span></span>
|<span data-ttu-id="ec663-154">关系</span><span class="sxs-lookup"><span data-stu-id="ec663-154">Relationship</span></span>|<span data-ttu-id="ec663-155">类型</span><span class="sxs-lookup"><span data-stu-id="ec663-155">Type</span></span>|<span data-ttu-id="ec663-156">说明</span><span class="sxs-lookup"><span data-stu-id="ec663-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec663-157">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="ec663-157">localizedNotificationMessages</span></span>|<span data-ttu-id="ec663-158">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ec663-158">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="ec663-159">此通知消息模板的本地化消息列表。</span><span class="sxs-lookup"><span data-stu-id="ec663-159">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec663-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec663-160">JSON Representation</span></span>
<span data-ttu-id="ec663-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec663-161">Here is a JSON representation of the resource.</span></span>
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
  "brandingOptions": "String"
}
```



