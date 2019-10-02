---
title: notificationMessageTemplate 资源类型
description: 通知消息是要发送给最终用户的消息，这些最终用户被确定为不符合管理员定义的合规策略要求。 管理员会选择通知，并使用“非合规性操作”部分下的合规策略创建页面，在 Intune 管理控制台中进行配置。 使用 notificationMessageTemplate 对象创建自定义通知，以便管理员在配置非合规操作时进行选择。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2fc108e02500c5e61871eea098b894b0903a6557
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360557"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="d3636-105">notificationMessageTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3636-105">notificationMessageTemplate resource type</span></span>

> <span data-ttu-id="d3636-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3636-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3636-107">通知消息是要发送给最终用户的消息，这些最终用户被确定为不符合管理员定义的合规策略要求。</span><span class="sxs-lookup"><span data-stu-id="d3636-107">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="d3636-108">管理员会选择通知，并使用“非合规性操作”部分下的合规策略创建页面，在 Intune 管理控制台中进行配置。</span><span class="sxs-lookup"><span data-stu-id="d3636-108">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="d3636-109">使用 notificationMessageTemplate 对象创建自定义通知，以便管理员在配置非合规操作时进行选择。</span><span class="sxs-lookup"><span data-stu-id="d3636-109">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>

## <a name="methods"></a><span data-ttu-id="d3636-110">方法</span><span class="sxs-lookup"><span data-stu-id="d3636-110">Methods</span></span>
|<span data-ttu-id="d3636-111">方法</span><span class="sxs-lookup"><span data-stu-id="d3636-111">Method</span></span>|<span data-ttu-id="d3636-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="d3636-112">Return Type</span></span>|<span data-ttu-id="d3636-113">说明</span><span class="sxs-lookup"><span data-stu-id="d3636-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d3636-114">List notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="d3636-114">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="d3636-115">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3636-115">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="d3636-116">列出 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d3636-116">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="d3636-117">Get notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d3636-117">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|[<span data-ttu-id="d3636-118">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d3636-118">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="d3636-119">读取 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d3636-119">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="d3636-120">创建 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d3636-120">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|[<span data-ttu-id="d3636-121">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d3636-121">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="d3636-122">创建新的 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d3636-122">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="d3636-123">Delete notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d3636-123">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="d3636-124">无</span><span class="sxs-lookup"><span data-stu-id="d3636-124">None</span></span>|<span data-ttu-id="d3636-125">删除 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="d3636-125">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="d3636-126">Update notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d3636-126">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="d3636-127">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="d3636-127">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="d3636-128">更新 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d3636-128">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="d3636-129">sendTestMessage 操作</span><span class="sxs-lookup"><span data-stu-id="d3636-129">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="d3636-130">无</span><span class="sxs-lookup"><span data-stu-id="d3636-130">None</span></span>|<span data-ttu-id="d3636-131">使用默认区域设置中指定的 notificationMessageTemplate 发送测试消息</span><span class="sxs-lookup"><span data-stu-id="d3636-131">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="d3636-132">属性</span><span class="sxs-lookup"><span data-stu-id="d3636-132">Properties</span></span>
|<span data-ttu-id="d3636-133">属性</span><span class="sxs-lookup"><span data-stu-id="d3636-133">Property</span></span>|<span data-ttu-id="d3636-134">类型</span><span class="sxs-lookup"><span data-stu-id="d3636-134">Type</span></span>|<span data-ttu-id="d3636-135">说明</span><span class="sxs-lookup"><span data-stu-id="d3636-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3636-136">id</span><span class="sxs-lookup"><span data-stu-id="d3636-136">id</span></span>|<span data-ttu-id="d3636-137">String</span><span class="sxs-lookup"><span data-stu-id="d3636-137">String</span></span>|<span data-ttu-id="d3636-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d3636-138">Key of the entity.</span></span>|
|<span data-ttu-id="d3636-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3636-139">lastModifiedDateTime</span></span>|<span data-ttu-id="d3636-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3636-140">DateTimeOffset</span></span>|<span data-ttu-id="d3636-141">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d3636-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d3636-142">displayName</span><span class="sxs-lookup"><span data-stu-id="d3636-142">displayName</span></span>|<span data-ttu-id="d3636-143">字符串</span><span class="sxs-lookup"><span data-stu-id="d3636-143">String</span></span>|<span data-ttu-id="d3636-144">通知消息模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d3636-144">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="d3636-145">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="d3636-145">defaultLocale</span></span>|<span data-ttu-id="d3636-146">String</span><span class="sxs-lookup"><span data-stu-id="d3636-146">String</span></span>|<span data-ttu-id="d3636-147">请求的区域设置不可用时要回退到的默认区域设置。</span><span class="sxs-lookup"><span data-stu-id="d3636-147">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="d3636-148">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="d3636-148">brandingOptions</span></span>|[<span data-ttu-id="d3636-149">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="d3636-149">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="d3636-150">消息模板品牌选项。</span><span class="sxs-lookup"><span data-stu-id="d3636-150">The Message Template Branding Options.</span></span> <span data-ttu-id="d3636-151">已在 Intune 管理员控制台中定义品牌。</span><span class="sxs-lookup"><span data-stu-id="d3636-151">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="d3636-152">可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`。</span><span class="sxs-lookup"><span data-stu-id="d3636-152">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3636-153">关系</span><span class="sxs-lookup"><span data-stu-id="d3636-153">Relationships</span></span>
|<span data-ttu-id="d3636-154">关系</span><span class="sxs-lookup"><span data-stu-id="d3636-154">Relationship</span></span>|<span data-ttu-id="d3636-155">类型</span><span class="sxs-lookup"><span data-stu-id="d3636-155">Type</span></span>|<span data-ttu-id="d3636-156">说明</span><span class="sxs-lookup"><span data-stu-id="d3636-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3636-157">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="d3636-157">localizedNotificationMessages</span></span>|<span data-ttu-id="d3636-158">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3636-158">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="d3636-159">此通知消息模板的本地化消息列表。</span><span class="sxs-lookup"><span data-stu-id="d3636-159">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3636-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3636-160">JSON Representation</span></span>
<span data-ttu-id="d3636-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3636-161">Here is a JSON representation of the resource.</span></span>
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




