---
title: notificationMessageTemplate 资源类型
description: " 部分。 使用 notificationMessageTemplate 对象创建自定义通知，以便管理员在配置非合规操作时进行选择。"
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5b9f298da4a4f37cde60ddc93402bf6d08d3f4f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912433"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="5dc52-104">notificationMessageTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="5dc52-104">notificationMessageTemplate resource type</span></span>

> <span data-ttu-id="5dc52-105">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5dc52-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5dc52-106">通知消息是要发送给最终用户的消息，这些最终用户被确定为不符合管理员定义的合规策略要求。</span><span class="sxs-lookup"><span data-stu-id="5dc52-106">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="5dc52-107">管理员会选择通知，并使用“非合规性操作”部分下的合规策略创建页面，在 Intune 管理控制台中进行配置。</span><span class="sxs-lookup"><span data-stu-id="5dc52-107">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="5dc52-108">使用 notificationMessageTemplate 对象创建自定义通知，以便管理员在配置非合规操作时进行选择。</span><span class="sxs-lookup"><span data-stu-id="5dc52-108">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>
## <a name="methods"></a><span data-ttu-id="5dc52-109">方法</span><span class="sxs-lookup"><span data-stu-id="5dc52-109">Methods</span></span>
|<span data-ttu-id="5dc52-110">方法</span><span class="sxs-lookup"><span data-stu-id="5dc52-110">Method</span></span>|<span data-ttu-id="5dc52-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="5dc52-111">Return Type</span></span>|<span data-ttu-id="5dc52-112">说明</span><span class="sxs-lookup"><span data-stu-id="5dc52-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5dc52-113">List notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="5dc52-113">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="5dc52-114">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5dc52-114">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="5dc52-115">列出 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5dc52-115">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="5dc52-116">Get notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="5dc52-116">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|[<span data-ttu-id="5dc52-117">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="5dc52-117">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="5dc52-118">读取 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5dc52-118">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="5dc52-119">创建 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="5dc52-119">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|[<span data-ttu-id="5dc52-120">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="5dc52-120">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="5dc52-121">创建新的 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5dc52-121">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="5dc52-122">Delete notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="5dc52-122">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="5dc52-123">无</span><span class="sxs-lookup"><span data-stu-id="5dc52-123">None</span></span>|<span data-ttu-id="5dc52-124">删除 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="5dc52-124">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="5dc52-125">Update notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="5dc52-125">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="5dc52-126">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="5dc52-126">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="5dc52-127">更新 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5dc52-127">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="5dc52-128">sendTestMessage 操作</span><span class="sxs-lookup"><span data-stu-id="5dc52-128">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="5dc52-129">无</span><span class="sxs-lookup"><span data-stu-id="5dc52-129">None</span></span>|<span data-ttu-id="5dc52-130">使用默认区域设置中指定的 notificationMessageTemplate 发送测试消息</span><span class="sxs-lookup"><span data-stu-id="5dc52-130">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="5dc52-131">属性</span><span class="sxs-lookup"><span data-stu-id="5dc52-131">Properties</span></span>
|<span data-ttu-id="5dc52-132">属性</span><span class="sxs-lookup"><span data-stu-id="5dc52-132">Property</span></span>|<span data-ttu-id="5dc52-133">类型</span><span class="sxs-lookup"><span data-stu-id="5dc52-133">Type</span></span>|<span data-ttu-id="5dc52-134">说明</span><span class="sxs-lookup"><span data-stu-id="5dc52-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dc52-135">id</span><span class="sxs-lookup"><span data-stu-id="5dc52-135">id</span></span>|<span data-ttu-id="5dc52-136">String</span><span class="sxs-lookup"><span data-stu-id="5dc52-136">String</span></span>|<span data-ttu-id="5dc52-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5dc52-137">Key of the entity.</span></span>|
|<span data-ttu-id="5dc52-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5dc52-138">lastModifiedDateTime</span></span>|<span data-ttu-id="5dc52-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dc52-139">DateTimeOffset</span></span>|<span data-ttu-id="5dc52-140">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5dc52-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="5dc52-141">displayName</span><span class="sxs-lookup"><span data-stu-id="5dc52-141">displayName</span></span>|<span data-ttu-id="5dc52-142">String</span><span class="sxs-lookup"><span data-stu-id="5dc52-142">String</span></span>|<span data-ttu-id="5dc52-143">通知消息模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5dc52-143">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="5dc52-144">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="5dc52-144">defaultLocale</span></span>|<span data-ttu-id="5dc52-145">String</span><span class="sxs-lookup"><span data-stu-id="5dc52-145">String</span></span>|<span data-ttu-id="5dc52-146">请求的区域设置不可用时要回退到的默认区域设置。</span><span class="sxs-lookup"><span data-stu-id="5dc52-146">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="5dc52-147">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="5dc52-147">brandingOptions</span></span>|[<span data-ttu-id="5dc52-148">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="5dc52-148">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="5dc52-149">消息模板品牌选项。</span><span class="sxs-lookup"><span data-stu-id="5dc52-149">The Message Template Branding Options.</span></span> <span data-ttu-id="5dc52-150">已在 Intune 管理员控制台中定义品牌。</span><span class="sxs-lookup"><span data-stu-id="5dc52-150">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="5dc52-151">可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`。</span><span class="sxs-lookup"><span data-stu-id="5dc52-151">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5dc52-152">Relationships</span><span class="sxs-lookup"><span data-stu-id="5dc52-152">Relationships</span></span>
|<span data-ttu-id="5dc52-153">关系</span><span class="sxs-lookup"><span data-stu-id="5dc52-153">Relationship</span></span>|<span data-ttu-id="5dc52-154">类型</span><span class="sxs-lookup"><span data-stu-id="5dc52-154">Type</span></span>|<span data-ttu-id="5dc52-155">说明</span><span class="sxs-lookup"><span data-stu-id="5dc52-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dc52-156">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="5dc52-156">localizedNotificationMessages</span></span>|<span data-ttu-id="5dc52-157">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5dc52-157">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="5dc52-158">此通知消息模板的本地化消息列表。</span><span class="sxs-lookup"><span data-stu-id="5dc52-158">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5dc52-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5dc52-159">JSON Representation</span></span>
<span data-ttu-id="5dc52-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5dc52-160">Here is a JSON representation of the resource.</span></span>
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



