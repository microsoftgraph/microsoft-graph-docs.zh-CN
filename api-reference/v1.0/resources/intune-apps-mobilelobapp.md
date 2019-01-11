---
title: mobileLobApp 资源类型
description: 包含所有移动业务线应用的属性的抽象基类。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4c36fbccf3549367cb0f6d58c5b50d6fc46a018a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860758"
---
# <a name="mobilelobapp-resource-type"></a><span data-ttu-id="640f2-103">mobileLobApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="640f2-103">mobileLobApp resource type</span></span>

> <span data-ttu-id="640f2-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="640f2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="640f2-105">包含所有移动业务线应用的属性的抽象基类。</span><span class="sxs-lookup"><span data-stu-id="640f2-105">An abstract base class containing properties for all mobile line of business apps.</span></span>

<span data-ttu-id="640f2-106">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-106">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="640f2-107">方法</span><span class="sxs-lookup"><span data-stu-id="640f2-107">Methods</span></span>
|<span data-ttu-id="640f2-108">方法</span><span class="sxs-lookup"><span data-stu-id="640f2-108">Method</span></span>|<span data-ttu-id="640f2-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="640f2-109">Return Type</span></span>|<span data-ttu-id="640f2-110">说明</span><span class="sxs-lookup"><span data-stu-id="640f2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="640f2-111">List mobileLobApps</span><span class="sxs-lookup"><span data-stu-id="640f2-111">List mobileLobApps</span></span>](../api/intune-apps-mobilelobapp-list.md)|<span data-ttu-id="640f2-112">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="640f2-112">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) collection</span></span>|<span data-ttu-id="640f2-113">列出 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="640f2-113">List properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects.</span></span>|
|[<span data-ttu-id="640f2-114">Get mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="640f2-114">Get mobileLobApp</span></span>](../api/intune-apps-mobilelobapp-get.md)|[<span data-ttu-id="640f2-115">mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="640f2-115">mobileLobApp</span></span>](../resources/intune-apps-mobilelobapp.md)|<span data-ttu-id="640f2-116">读取 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="640f2-116">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="640f2-117">属性</span><span class="sxs-lookup"><span data-stu-id="640f2-117">Properties</span></span>
|<span data-ttu-id="640f2-118">属性</span><span class="sxs-lookup"><span data-stu-id="640f2-118">Property</span></span>|<span data-ttu-id="640f2-119">类型</span><span class="sxs-lookup"><span data-stu-id="640f2-119">Type</span></span>|<span data-ttu-id="640f2-120">说明</span><span class="sxs-lookup"><span data-stu-id="640f2-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="640f2-121">id</span><span class="sxs-lookup"><span data-stu-id="640f2-121">id</span></span>|<span data-ttu-id="640f2-122">String</span><span class="sxs-lookup"><span data-stu-id="640f2-122">String</span></span>|<span data-ttu-id="640f2-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="640f2-123">Key of the entity.</span></span> <span data-ttu-id="640f2-124">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-124">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="640f2-125">displayName</span><span class="sxs-lookup"><span data-stu-id="640f2-125">displayName</span></span>|<span data-ttu-id="640f2-126">String</span><span class="sxs-lookup"><span data-stu-id="640f2-126">String</span></span>|<span data-ttu-id="640f2-127">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="640f2-127">The admin provided or imported title of the app.</span></span> <span data-ttu-id="640f2-128">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-128">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="640f2-129">description</span><span class="sxs-lookup"><span data-stu-id="640f2-129">description</span></span>|<span data-ttu-id="640f2-130">String</span><span class="sxs-lookup"><span data-stu-id="640f2-130">String</span></span>|<span data-ttu-id="640f2-131">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="640f2-131">The description of the app.</span></span> <span data-ttu-id="640f2-132">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-132">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="640f2-133">publisher</span><span class="sxs-lookup"><span data-stu-id="640f2-133">publisher</span></span>|<span data-ttu-id="640f2-134">String</span><span class="sxs-lookup"><span data-stu-id="640f2-134">String</span></span>|<span data-ttu-id="640f2-135">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="640f2-135">The publisher of the app.</span></span> <span data-ttu-id="640f2-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="640f2-137">largeIcon</span><span class="sxs-lookup"><span data-stu-id="640f2-137">largeIcon</span></span>|[<span data-ttu-id="640f2-138">mimeContent</span><span class="sxs-lookup"><span data-stu-id="640f2-138">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="640f2-139">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="640f2-139">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="640f2-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="640f2-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="640f2-141">createdDateTime</span></span>|<span data-ttu-id="640f2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="640f2-142">DateTimeOffset</span></span>|<span data-ttu-id="640f2-143">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="640f2-143">The date and time the app was created.</span></span> <span data-ttu-id="640f2-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="640f2-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="640f2-145">lastModifiedDateTime</span></span>|<span data-ttu-id="640f2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="640f2-146">DateTimeOffset</span></span>|<span data-ttu-id="640f2-147">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="640f2-147">The date and time the app was last modified.</span></span> <span data-ttu-id="640f2-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="640f2-149">isFeatured</span><span class="sxs-lookup"><span data-stu-id="640f2-149">isFeatured</span></span>|<span data-ttu-id="640f2-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="640f2-150">Boolean</span></span>|<span data-ttu-id="640f2-151">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-151">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="640f2-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="640f2-152">privacyInformationUrl</span></span>|<span data-ttu-id="640f2-153">String</span><span class="sxs-lookup"><span data-stu-id="640f2-153">String</span></span>|<span data-ttu-id="640f2-154">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="640f2-154">The privacy statement Url.</span></span> <span data-ttu-id="640f2-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="640f2-156">informationUrl</span><span class="sxs-lookup"><span data-stu-id="640f2-156">informationUrl</span></span>|<span data-ttu-id="640f2-157">String</span><span class="sxs-lookup"><span data-stu-id="640f2-157">String</span></span>|<span data-ttu-id="640f2-158">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="640f2-158">The more information Url.</span></span> <span data-ttu-id="640f2-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="640f2-160">owner</span><span class="sxs-lookup"><span data-stu-id="640f2-160">owner</span></span>|<span data-ttu-id="640f2-161">String</span><span class="sxs-lookup"><span data-stu-id="640f2-161">String</span></span>|<span data-ttu-id="640f2-162">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="640f2-162">The owner of the app.</span></span> <span data-ttu-id="640f2-163">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-163">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="640f2-164">developer</span><span class="sxs-lookup"><span data-stu-id="640f2-164">developer</span></span>|<span data-ttu-id="640f2-165">String</span><span class="sxs-lookup"><span data-stu-id="640f2-165">String</span></span>|<span data-ttu-id="640f2-166">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="640f2-166">The developer of the app.</span></span> <span data-ttu-id="640f2-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="640f2-168">notes</span><span class="sxs-lookup"><span data-stu-id="640f2-168">notes</span></span>|<span data-ttu-id="640f2-169">String</span><span class="sxs-lookup"><span data-stu-id="640f2-169">String</span></span>|<span data-ttu-id="640f2-170">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="640f2-170">Notes for the app.</span></span> <span data-ttu-id="640f2-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="640f2-172">publishingState</span><span class="sxs-lookup"><span data-stu-id="640f2-172">publishingState</span></span>|[<span data-ttu-id="640f2-173">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="640f2-173">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="640f2-174">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="640f2-174">The publishing state for the app.</span></span> <span data-ttu-id="640f2-175">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="640f2-175">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="640f2-176">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="640f2-176">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="640f2-177">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="640f2-177">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="640f2-178">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="640f2-178">committedContentVersion</span></span>|<span data-ttu-id="640f2-179">String</span><span class="sxs-lookup"><span data-stu-id="640f2-179">String</span></span>|<span data-ttu-id="640f2-180">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="640f2-180">The internal committed content version.</span></span>|
|<span data-ttu-id="640f2-181">fileName</span><span class="sxs-lookup"><span data-stu-id="640f2-181">fileName</span></span>|<span data-ttu-id="640f2-182">String</span><span class="sxs-lookup"><span data-stu-id="640f2-182">String</span></span>|<span data-ttu-id="640f2-183">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="640f2-183">The name of the main Lob application file.</span></span>|
|<span data-ttu-id="640f2-184">size</span><span class="sxs-lookup"><span data-stu-id="640f2-184">size</span></span>|<span data-ttu-id="640f2-185">Int64</span><span class="sxs-lookup"><span data-stu-id="640f2-185">Int64</span></span>|<span data-ttu-id="640f2-186">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="640f2-186">The total size, including all uploaded files.</span></span>|

## <a name="relationships"></a><span data-ttu-id="640f2-187">关系</span><span class="sxs-lookup"><span data-stu-id="640f2-187">Relationships</span></span>
|<span data-ttu-id="640f2-188">关系</span><span class="sxs-lookup"><span data-stu-id="640f2-188">Relationship</span></span>|<span data-ttu-id="640f2-189">类型</span><span class="sxs-lookup"><span data-stu-id="640f2-189">Type</span></span>|<span data-ttu-id="640f2-190">说明</span><span class="sxs-lookup"><span data-stu-id="640f2-190">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="640f2-191">categories</span><span class="sxs-lookup"><span data-stu-id="640f2-191">categories</span></span>|<span data-ttu-id="640f2-192">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="640f2-192">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="640f2-193">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="640f2-193">The list of categories for this app.</span></span> <span data-ttu-id="640f2-194">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-194">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="640f2-195">assignments</span><span class="sxs-lookup"><span data-stu-id="640f2-195">assignments</span></span>|<span data-ttu-id="640f2-196">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="640f2-196">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="640f2-197">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="640f2-197">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="640f2-198">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="640f2-198">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="640f2-199">contentVersions</span><span class="sxs-lookup"><span data-stu-id="640f2-199">contentVersions</span></span>|<span data-ttu-id="640f2-200">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="640f2-200">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="640f2-201">此应用的内容版本列表。</span><span class="sxs-lookup"><span data-stu-id="640f2-201">The list of content versions for this app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="640f2-202">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="640f2-202">JSON Representation</span></span>
<span data-ttu-id="640f2-203">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="640f2-203">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileLobApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024
}
```



