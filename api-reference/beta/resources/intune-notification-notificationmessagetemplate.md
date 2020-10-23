---
title: notificationMessageTemplate 资源类型
description: 通知消息是要发送给最终用户的消息，这些最终用户被确定为不符合管理员定义的合规策略要求。 管理员会选择通知，并使用“非合规性操作”部分下的合规策略创建页面，在 Intune 管理控制台中进行配置。 使用 notificationMessageTemplate 对象创建自定义通知，以便管理员在配置非合规操作时进行选择。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ab977ad5a3d21c6cc0154053063e78fea06cf347
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691195"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="893d0-105">notificationMessageTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="893d0-105">notificationMessageTemplate resource type</span></span>

<span data-ttu-id="893d0-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="893d0-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="893d0-107">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="893d0-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="893d0-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="893d0-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="893d0-109">通知消息是要发送给最终用户的消息，这些最终用户被确定为不符合管理员定义的合规策略要求。</span><span class="sxs-lookup"><span data-stu-id="893d0-109">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="893d0-110">管理员会选择通知，并使用“非合规性操作”部分下的合规策略创建页面，在 Intune 管理控制台中进行配置。</span><span class="sxs-lookup"><span data-stu-id="893d0-110">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="893d0-111">使用 notificationMessageTemplate 对象创建自定义通知，以便管理员在配置非合规操作时进行选择。</span><span class="sxs-lookup"><span data-stu-id="893d0-111">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>

## <a name="methods"></a><span data-ttu-id="893d0-112">Methods</span><span class="sxs-lookup"><span data-stu-id="893d0-112">Methods</span></span>
|<span data-ttu-id="893d0-113">方法</span><span class="sxs-lookup"><span data-stu-id="893d0-113">Method</span></span>|<span data-ttu-id="893d0-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="893d0-114">Return Type</span></span>|<span data-ttu-id="893d0-115">说明</span><span class="sxs-lookup"><span data-stu-id="893d0-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="893d0-116">List notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="893d0-116">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="893d0-117">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="893d0-117">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="893d0-118">列出 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="893d0-118">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="893d0-119">Get notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="893d0-119">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|[<span data-ttu-id="893d0-120">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="893d0-120">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="893d0-121">读取 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="893d0-121">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="893d0-122">创建 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="893d0-122">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|[<span data-ttu-id="893d0-123">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="893d0-123">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="893d0-124">创建新的 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="893d0-124">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="893d0-125">Delete notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="893d0-125">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="893d0-126">无</span><span class="sxs-lookup"><span data-stu-id="893d0-126">None</span></span>|<span data-ttu-id="893d0-127">删除 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="893d0-127">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="893d0-128">Update notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="893d0-128">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="893d0-129">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="893d0-129">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="893d0-130">更新 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="893d0-130">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="893d0-131">sendTestMessage 操作</span><span class="sxs-lookup"><span data-stu-id="893d0-131">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="893d0-132">无</span><span class="sxs-lookup"><span data-stu-id="893d0-132">None</span></span>|<span data-ttu-id="893d0-133">使用默认区域设置中指定的 notificationMessageTemplate 发送测试消息</span><span class="sxs-lookup"><span data-stu-id="893d0-133">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="893d0-134">属性</span><span class="sxs-lookup"><span data-stu-id="893d0-134">Properties</span></span>
|<span data-ttu-id="893d0-135">属性</span><span class="sxs-lookup"><span data-stu-id="893d0-135">Property</span></span>|<span data-ttu-id="893d0-136">类型</span><span class="sxs-lookup"><span data-stu-id="893d0-136">Type</span></span>|<span data-ttu-id="893d0-137">说明</span><span class="sxs-lookup"><span data-stu-id="893d0-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="893d0-138">id</span><span class="sxs-lookup"><span data-stu-id="893d0-138">id</span></span>|<span data-ttu-id="893d0-139">String</span><span class="sxs-lookup"><span data-stu-id="893d0-139">String</span></span>|<span data-ttu-id="893d0-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="893d0-140">Key of the entity.</span></span>|
|<span data-ttu-id="893d0-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="893d0-141">lastModifiedDateTime</span></span>|<span data-ttu-id="893d0-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="893d0-142">DateTimeOffset</span></span>|<span data-ttu-id="893d0-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="893d0-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="893d0-144">displayName</span><span class="sxs-lookup"><span data-stu-id="893d0-144">displayName</span></span>|<span data-ttu-id="893d0-145">String</span><span class="sxs-lookup"><span data-stu-id="893d0-145">String</span></span>|<span data-ttu-id="893d0-146">通知消息模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="893d0-146">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="893d0-147">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="893d0-147">defaultLocale</span></span>|<span data-ttu-id="893d0-148">String</span><span class="sxs-lookup"><span data-stu-id="893d0-148">String</span></span>|<span data-ttu-id="893d0-149">请求的区域设置不可用时要回退到的默认区域设置。</span><span class="sxs-lookup"><span data-stu-id="893d0-149">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="893d0-150">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="893d0-150">brandingOptions</span></span>|[<span data-ttu-id="893d0-151">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="893d0-151">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="893d0-152">消息模板品牌选项。</span><span class="sxs-lookup"><span data-stu-id="893d0-152">The Message Template Branding Options.</span></span> <span data-ttu-id="893d0-153">已在 Intune 管理员控制台中定义品牌。</span><span class="sxs-lookup"><span data-stu-id="893d0-153">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="893d0-154">可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`、`includeCompanyPortalLink`。</span><span class="sxs-lookup"><span data-stu-id="893d0-154">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`.</span></span>|
|<span data-ttu-id="893d0-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="893d0-155">roleScopeTagIds</span></span>|<span data-ttu-id="893d0-156">String collection</span><span class="sxs-lookup"><span data-stu-id="893d0-156">String collection</span></span>|<span data-ttu-id="893d0-157">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="893d0-157">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="893d0-158">关系</span><span class="sxs-lookup"><span data-stu-id="893d0-158">Relationships</span></span>
|<span data-ttu-id="893d0-159">关系</span><span class="sxs-lookup"><span data-stu-id="893d0-159">Relationship</span></span>|<span data-ttu-id="893d0-160">类型</span><span class="sxs-lookup"><span data-stu-id="893d0-160">Type</span></span>|<span data-ttu-id="893d0-161">说明</span><span class="sxs-lookup"><span data-stu-id="893d0-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="893d0-162">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="893d0-162">localizedNotificationMessages</span></span>|<span data-ttu-id="893d0-163">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="893d0-163">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="893d0-164">此通知消息模板的本地化消息列表。</span><span class="sxs-lookup"><span data-stu-id="893d0-164">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="893d0-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="893d0-165">JSON Representation</span></span>
<span data-ttu-id="893d0-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="893d0-166">Here is a JSON representation of the resource.</span></span>
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





