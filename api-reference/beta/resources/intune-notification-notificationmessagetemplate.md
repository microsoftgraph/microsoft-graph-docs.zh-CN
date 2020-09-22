---
title: notificationMessageTemplate 资源类型
description: 通知消息是要发送给最终用户的消息，这些最终用户被确定为不符合管理员定义的合规策略要求。 管理员会选择通知，并使用“非合规性操作”部分下的合规策略创建页面，在 Intune 管理控制台中进行配置。 使用 notificationMessageTemplate 对象创建自定义通知，以便管理员在配置非合规操作时进行选择。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9c4e0c2f7cfe723d8e8ac2ec5b583889aa2e6602
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029888"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="24c38-105">notificationMessageTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="24c38-105">notificationMessageTemplate resource type</span></span>

<span data-ttu-id="24c38-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24c38-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24c38-107">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="24c38-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24c38-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24c38-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24c38-109">通知消息是要发送给最终用户的消息，这些最终用户被确定为不符合管理员定义的合规策略要求。</span><span class="sxs-lookup"><span data-stu-id="24c38-109">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="24c38-110">管理员会选择通知，并使用“非合规性操作”部分下的合规策略创建页面，在 Intune 管理控制台中进行配置。</span><span class="sxs-lookup"><span data-stu-id="24c38-110">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="24c38-111">使用 notificationMessageTemplate 对象创建自定义通知，以便管理员在配置非合规操作时进行选择。</span><span class="sxs-lookup"><span data-stu-id="24c38-111">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>

## <a name="methods"></a><span data-ttu-id="24c38-112">方法</span><span class="sxs-lookup"><span data-stu-id="24c38-112">Methods</span></span>
|<span data-ttu-id="24c38-113">方法</span><span class="sxs-lookup"><span data-stu-id="24c38-113">Method</span></span>|<span data-ttu-id="24c38-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="24c38-114">Return Type</span></span>|<span data-ttu-id="24c38-115">说明</span><span class="sxs-lookup"><span data-stu-id="24c38-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="24c38-116">List notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="24c38-116">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="24c38-117">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="24c38-117">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="24c38-118">列出 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="24c38-118">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="24c38-119">Get notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="24c38-119">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|[<span data-ttu-id="24c38-120">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="24c38-120">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="24c38-121">读取 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="24c38-121">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="24c38-122">创建 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="24c38-122">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|[<span data-ttu-id="24c38-123">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="24c38-123">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="24c38-124">创建新的 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="24c38-124">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="24c38-125">Delete notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="24c38-125">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="24c38-126">无</span><span class="sxs-lookup"><span data-stu-id="24c38-126">None</span></span>|<span data-ttu-id="24c38-127">删除 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="24c38-127">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="24c38-128">Update notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="24c38-128">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="24c38-129">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="24c38-129">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="24c38-130">更新 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="24c38-130">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="24c38-131">sendTestMessage 操作</span><span class="sxs-lookup"><span data-stu-id="24c38-131">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="24c38-132">无</span><span class="sxs-lookup"><span data-stu-id="24c38-132">None</span></span>|<span data-ttu-id="24c38-133">使用默认区域设置中指定的 notificationMessageTemplate 发送测试消息</span><span class="sxs-lookup"><span data-stu-id="24c38-133">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="24c38-134">属性</span><span class="sxs-lookup"><span data-stu-id="24c38-134">Properties</span></span>
|<span data-ttu-id="24c38-135">属性</span><span class="sxs-lookup"><span data-stu-id="24c38-135">Property</span></span>|<span data-ttu-id="24c38-136">类型</span><span class="sxs-lookup"><span data-stu-id="24c38-136">Type</span></span>|<span data-ttu-id="24c38-137">说明</span><span class="sxs-lookup"><span data-stu-id="24c38-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24c38-138">id</span><span class="sxs-lookup"><span data-stu-id="24c38-138">id</span></span>|<span data-ttu-id="24c38-139">String</span><span class="sxs-lookup"><span data-stu-id="24c38-139">String</span></span>|<span data-ttu-id="24c38-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="24c38-140">Key of the entity.</span></span>|
|<span data-ttu-id="24c38-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24c38-141">lastModifiedDateTime</span></span>|<span data-ttu-id="24c38-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24c38-142">DateTimeOffset</span></span>|<span data-ttu-id="24c38-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="24c38-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="24c38-144">displayName</span><span class="sxs-lookup"><span data-stu-id="24c38-144">displayName</span></span>|<span data-ttu-id="24c38-145">String</span><span class="sxs-lookup"><span data-stu-id="24c38-145">String</span></span>|<span data-ttu-id="24c38-146">通知消息模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="24c38-146">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="24c38-147">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="24c38-147">defaultLocale</span></span>|<span data-ttu-id="24c38-148">String</span><span class="sxs-lookup"><span data-stu-id="24c38-148">String</span></span>|<span data-ttu-id="24c38-149">请求的区域设置不可用时要回退到的默认区域设置。</span><span class="sxs-lookup"><span data-stu-id="24c38-149">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="24c38-150">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="24c38-150">brandingOptions</span></span>|[<span data-ttu-id="24c38-151">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="24c38-151">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="24c38-152">消息模板品牌选项。</span><span class="sxs-lookup"><span data-stu-id="24c38-152">The Message Template Branding Options.</span></span> <span data-ttu-id="24c38-153">已在 Intune 管理员控制台中定义品牌。</span><span class="sxs-lookup"><span data-stu-id="24c38-153">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="24c38-154">可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`、`includeCompanyPortalLink`。</span><span class="sxs-lookup"><span data-stu-id="24c38-154">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.</span></span>|
|<span data-ttu-id="24c38-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="24c38-155">roleScopeTagIds</span></span>|<span data-ttu-id="24c38-156">String 集合</span><span class="sxs-lookup"><span data-stu-id="24c38-156">String collection</span></span>|<span data-ttu-id="24c38-157">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="24c38-157">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24c38-158">关系</span><span class="sxs-lookup"><span data-stu-id="24c38-158">Relationships</span></span>
|<span data-ttu-id="24c38-159">关系</span><span class="sxs-lookup"><span data-stu-id="24c38-159">Relationship</span></span>|<span data-ttu-id="24c38-160">类型</span><span class="sxs-lookup"><span data-stu-id="24c38-160">Type</span></span>|<span data-ttu-id="24c38-161">说明</span><span class="sxs-lookup"><span data-stu-id="24c38-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24c38-162">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="24c38-162">localizedNotificationMessages</span></span>|<span data-ttu-id="24c38-163">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="24c38-163">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="24c38-164">此通知消息模板的本地化消息列表。</span><span class="sxs-lookup"><span data-stu-id="24c38-164">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24c38-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24c38-165">JSON Representation</span></span>
<span data-ttu-id="24c38-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24c38-166">Here is a JSON representation of the resource.</span></span>
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






