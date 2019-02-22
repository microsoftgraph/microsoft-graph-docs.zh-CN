---
title: notificationMessageTemplate 资源类型
description: 通知消息是要发送给最终用户的消息，这些最终用户被确定为不符合管理员定义的合规策略要求。 管理员会选择通知，并使用“非合规性操作”部分下的合规策略创建页面，在 Intune 管理控制台中进行配置。 使用 notificationMessageTemplate 对象创建自定义通知，以便管理员在配置非合规操作时进行选择。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 487b536b8e957ff695899ce4b22e11d11088e06f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143370"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="13398-105">notificationMessageTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="13398-105">notificationMessageTemplate resource type</span></span>

> <span data-ttu-id="13398-106">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13398-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13398-107">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13398-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13398-108">通知消息是要发送给最终用户的消息，这些最终用户被确定为不符合管理员定义的合规策略要求。</span><span class="sxs-lookup"><span data-stu-id="13398-108">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="13398-109">管理员会选择通知，并使用“非合规性操作”部分下的合规策略创建页面，在 Intune 管理控制台中进行配置。</span><span class="sxs-lookup"><span data-stu-id="13398-109">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="13398-110">使用 notificationMessageTemplate 对象创建自定义通知，以便管理员在配置非合规操作时进行选择。</span><span class="sxs-lookup"><span data-stu-id="13398-110">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>

## <a name="methods"></a><span data-ttu-id="13398-111">方法</span><span class="sxs-lookup"><span data-stu-id="13398-111">Methods</span></span>
|<span data-ttu-id="13398-112">方法</span><span class="sxs-lookup"><span data-stu-id="13398-112">Method</span></span>|<span data-ttu-id="13398-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="13398-113">Return Type</span></span>|<span data-ttu-id="13398-114">说明</span><span class="sxs-lookup"><span data-stu-id="13398-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="13398-115">List notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="13398-115">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="13398-116">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="13398-116">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="13398-117">列出 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13398-117">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="13398-118">Get notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="13398-118">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|[<span data-ttu-id="13398-119">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="13398-119">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="13398-120">读取 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13398-120">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="13398-121">创建 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="13398-121">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|[<span data-ttu-id="13398-122">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="13398-122">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="13398-123">创建新的 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="13398-123">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="13398-124">Delete notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="13398-124">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="13398-125">无</span><span class="sxs-lookup"><span data-stu-id="13398-125">None</span></span>|<span data-ttu-id="13398-126">删除 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="13398-126">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="13398-127">Update notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="13398-127">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="13398-128">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="13398-128">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="13398-129">更新 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="13398-129">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="13398-130">sendTestMessage 操作</span><span class="sxs-lookup"><span data-stu-id="13398-130">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="13398-131">无</span><span class="sxs-lookup"><span data-stu-id="13398-131">None</span></span>|<span data-ttu-id="13398-132">使用默认区域设置中指定的 notificationMessageTemplate 发送测试消息</span><span class="sxs-lookup"><span data-stu-id="13398-132">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="13398-133">属性</span><span class="sxs-lookup"><span data-stu-id="13398-133">Properties</span></span>
|<span data-ttu-id="13398-134">属性</span><span class="sxs-lookup"><span data-stu-id="13398-134">Property</span></span>|<span data-ttu-id="13398-135">类型</span><span class="sxs-lookup"><span data-stu-id="13398-135">Type</span></span>|<span data-ttu-id="13398-136">说明</span><span class="sxs-lookup"><span data-stu-id="13398-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13398-137">id</span><span class="sxs-lookup"><span data-stu-id="13398-137">id</span></span>|<span data-ttu-id="13398-138">字符串</span><span class="sxs-lookup"><span data-stu-id="13398-138">String</span></span>|<span data-ttu-id="13398-139">实体的键。</span><span class="sxs-lookup"><span data-stu-id="13398-139">Key of the entity.</span></span>|
|<span data-ttu-id="13398-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13398-140">lastModifiedDateTime</span></span>|<span data-ttu-id="13398-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13398-141">DateTimeOffset</span></span>|<span data-ttu-id="13398-142">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="13398-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="13398-143">displayName</span><span class="sxs-lookup"><span data-stu-id="13398-143">displayName</span></span>|<span data-ttu-id="13398-144">String</span><span class="sxs-lookup"><span data-stu-id="13398-144">String</span></span>|<span data-ttu-id="13398-145">通知消息模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="13398-145">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="13398-146">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="13398-146">defaultLocale</span></span>|<span data-ttu-id="13398-147">String</span><span class="sxs-lookup"><span data-stu-id="13398-147">String</span></span>|<span data-ttu-id="13398-148">请求的区域设置不可用时要回退到的默认区域设置。</span><span class="sxs-lookup"><span data-stu-id="13398-148">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="13398-149">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="13398-149">brandingOptions</span></span>|[<span data-ttu-id="13398-150">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="13398-150">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="13398-151">消息模板品牌选项。</span><span class="sxs-lookup"><span data-stu-id="13398-151">The Message Template Branding Options.</span></span> <span data-ttu-id="13398-152">已在 Intune 管理员控制台中定义品牌。</span><span class="sxs-lookup"><span data-stu-id="13398-152">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="13398-153">可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`。</span><span class="sxs-lookup"><span data-stu-id="13398-153">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="13398-154">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="13398-154">roleScopeTagIds</span></span>|<span data-ttu-id="13398-155">String collection</span><span class="sxs-lookup"><span data-stu-id="13398-155">String collection</span></span>|<span data-ttu-id="13398-156">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="13398-156">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13398-157">关系</span><span class="sxs-lookup"><span data-stu-id="13398-157">Relationships</span></span>
|<span data-ttu-id="13398-158">关系</span><span class="sxs-lookup"><span data-stu-id="13398-158">Relationship</span></span>|<span data-ttu-id="13398-159">类型</span><span class="sxs-lookup"><span data-stu-id="13398-159">Type</span></span>|<span data-ttu-id="13398-160">说明</span><span class="sxs-lookup"><span data-stu-id="13398-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13398-161">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="13398-161">localizedNotificationMessages</span></span>|<span data-ttu-id="13398-162">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="13398-162">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="13398-163">此通知消息模板的本地化消息列表。</span><span class="sxs-lookup"><span data-stu-id="13398-163">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13398-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13398-164">JSON Representation</span></span>
<span data-ttu-id="13398-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13398-165">Here is a JSON representation of the resource.</span></span>
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




