---
title: mobileLobApp 资源类型
description: 包含所有移动业务线应用的属性的抽象基类。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f87769fa7d56bcd97dca165f40d1277ffa0dcd7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932663"
---
# <a name="mobilelobapp-resource-type"></a><span data-ttu-id="e39cd-103">mobileLobApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="e39cd-103">mobileLobApp resource type</span></span>

> <span data-ttu-id="e39cd-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e39cd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e39cd-105">包含所有移动业务线应用的属性的抽象基类。</span><span class="sxs-lookup"><span data-stu-id="e39cd-105">An abstract base class containing properties for all mobile line of business apps.</span></span>

<span data-ttu-id="e39cd-106">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-106">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e39cd-107">方法</span><span class="sxs-lookup"><span data-stu-id="e39cd-107">Methods</span></span>
|<span data-ttu-id="e39cd-108">方法</span><span class="sxs-lookup"><span data-stu-id="e39cd-108">Method</span></span>|<span data-ttu-id="e39cd-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e39cd-109">Return Type</span></span>|<span data-ttu-id="e39cd-110">说明</span><span class="sxs-lookup"><span data-stu-id="e39cd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e39cd-111">List mobileLobApps</span><span class="sxs-lookup"><span data-stu-id="e39cd-111">List mobileLobApps</span></span>](../api/intune-apps-mobilelobapp-list.md)|<span data-ttu-id="e39cd-112">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e39cd-112">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) collection</span></span>|<span data-ttu-id="e39cd-113">列出 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e39cd-113">List properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects.</span></span>|
|[<span data-ttu-id="e39cd-114">Get mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="e39cd-114">Get mobileLobApp</span></span>](../api/intune-apps-mobilelobapp-get.md)|[<span data-ttu-id="e39cd-115">mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="e39cd-115">mobileLobApp</span></span>](../resources/intune-apps-mobilelobapp.md)|<span data-ttu-id="e39cd-116">读取 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e39cd-116">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e39cd-117">属性</span><span class="sxs-lookup"><span data-stu-id="e39cd-117">Properties</span></span>
|<span data-ttu-id="e39cd-118">属性</span><span class="sxs-lookup"><span data-stu-id="e39cd-118">Property</span></span>|<span data-ttu-id="e39cd-119">类型</span><span class="sxs-lookup"><span data-stu-id="e39cd-119">Type</span></span>|<span data-ttu-id="e39cd-120">说明</span><span class="sxs-lookup"><span data-stu-id="e39cd-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e39cd-121">id</span><span class="sxs-lookup"><span data-stu-id="e39cd-121">id</span></span>|<span data-ttu-id="e39cd-122">String</span><span class="sxs-lookup"><span data-stu-id="e39cd-122">String</span></span>|<span data-ttu-id="e39cd-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e39cd-123">Key of the entity.</span></span> <span data-ttu-id="e39cd-124">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-124">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39cd-125">displayName</span><span class="sxs-lookup"><span data-stu-id="e39cd-125">displayName</span></span>|<span data-ttu-id="e39cd-126">String</span><span class="sxs-lookup"><span data-stu-id="e39cd-126">String</span></span>|<span data-ttu-id="e39cd-127">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="e39cd-127">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e39cd-128">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-128">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39cd-129">description</span><span class="sxs-lookup"><span data-stu-id="e39cd-129">description</span></span>|<span data-ttu-id="e39cd-130">String</span><span class="sxs-lookup"><span data-stu-id="e39cd-130">String</span></span>|<span data-ttu-id="e39cd-131">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="e39cd-131">The description of the app.</span></span> <span data-ttu-id="e39cd-132">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-132">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39cd-133">publisher</span><span class="sxs-lookup"><span data-stu-id="e39cd-133">publisher</span></span>|<span data-ttu-id="e39cd-134">String</span><span class="sxs-lookup"><span data-stu-id="e39cd-134">String</span></span>|<span data-ttu-id="e39cd-135">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="e39cd-135">The publisher of the app.</span></span> <span data-ttu-id="e39cd-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39cd-137">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e39cd-137">largeIcon</span></span>|[<span data-ttu-id="e39cd-138">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e39cd-138">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e39cd-139">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="e39cd-139">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e39cd-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39cd-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e39cd-141">createdDateTime</span></span>|<span data-ttu-id="e39cd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e39cd-142">DateTimeOffset</span></span>|<span data-ttu-id="e39cd-143">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e39cd-143">The date and time the app was created.</span></span> <span data-ttu-id="e39cd-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39cd-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e39cd-145">lastModifiedDateTime</span></span>|<span data-ttu-id="e39cd-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e39cd-146">DateTimeOffset</span></span>|<span data-ttu-id="e39cd-147">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e39cd-147">The date and time the app was last modified.</span></span> <span data-ttu-id="e39cd-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39cd-149">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e39cd-149">isFeatured</span></span>|<span data-ttu-id="e39cd-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="e39cd-150">Boolean</span></span>|<span data-ttu-id="e39cd-151">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-151">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39cd-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e39cd-152">privacyInformationUrl</span></span>|<span data-ttu-id="e39cd-153">String</span><span class="sxs-lookup"><span data-stu-id="e39cd-153">String</span></span>|<span data-ttu-id="e39cd-154">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="e39cd-154">The privacy statement Url.</span></span> <span data-ttu-id="e39cd-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39cd-156">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e39cd-156">informationUrl</span></span>|<span data-ttu-id="e39cd-157">String</span><span class="sxs-lookup"><span data-stu-id="e39cd-157">String</span></span>|<span data-ttu-id="e39cd-158">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="e39cd-158">The more information Url.</span></span> <span data-ttu-id="e39cd-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39cd-160">owner</span><span class="sxs-lookup"><span data-stu-id="e39cd-160">owner</span></span>|<span data-ttu-id="e39cd-161">String</span><span class="sxs-lookup"><span data-stu-id="e39cd-161">String</span></span>|<span data-ttu-id="e39cd-162">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="e39cd-162">The owner of the app.</span></span> <span data-ttu-id="e39cd-163">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-163">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39cd-164">developer</span><span class="sxs-lookup"><span data-stu-id="e39cd-164">developer</span></span>|<span data-ttu-id="e39cd-165">String</span><span class="sxs-lookup"><span data-stu-id="e39cd-165">String</span></span>|<span data-ttu-id="e39cd-166">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="e39cd-166">The developer of the app.</span></span> <span data-ttu-id="e39cd-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39cd-168">notes</span><span class="sxs-lookup"><span data-stu-id="e39cd-168">notes</span></span>|<span data-ttu-id="e39cd-169">String</span><span class="sxs-lookup"><span data-stu-id="e39cd-169">String</span></span>|<span data-ttu-id="e39cd-170">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="e39cd-170">Notes for the app.</span></span> <span data-ttu-id="e39cd-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39cd-172">publishingState</span><span class="sxs-lookup"><span data-stu-id="e39cd-172">publishingState</span></span>|[<span data-ttu-id="e39cd-173">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e39cd-173">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e39cd-174">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="e39cd-174">The publishing state for the app.</span></span> <span data-ttu-id="e39cd-175">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="e39cd-175">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e39cd-176">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="e39cd-176">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e39cd-177">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="e39cd-177">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e39cd-178">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e39cd-178">committedContentVersion</span></span>|<span data-ttu-id="e39cd-179">String</span><span class="sxs-lookup"><span data-stu-id="e39cd-179">String</span></span>|<span data-ttu-id="e39cd-180">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="e39cd-180">The internal committed content version.</span></span>|
|<span data-ttu-id="e39cd-181">fileName</span><span class="sxs-lookup"><span data-stu-id="e39cd-181">fileName</span></span>|<span data-ttu-id="e39cd-182">String</span><span class="sxs-lookup"><span data-stu-id="e39cd-182">String</span></span>|<span data-ttu-id="e39cd-183">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="e39cd-183">The name of the main Lob application file.</span></span>|
|<span data-ttu-id="e39cd-184">size</span><span class="sxs-lookup"><span data-stu-id="e39cd-184">size</span></span>|<span data-ttu-id="e39cd-185">Int64</span><span class="sxs-lookup"><span data-stu-id="e39cd-185">Int64</span></span>|<span data-ttu-id="e39cd-186">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="e39cd-186">The total size, including all uploaded files.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e39cd-187">关系</span><span class="sxs-lookup"><span data-stu-id="e39cd-187">Relationships</span></span>
|<span data-ttu-id="e39cd-188">关系</span><span class="sxs-lookup"><span data-stu-id="e39cd-188">Relationship</span></span>|<span data-ttu-id="e39cd-189">类型</span><span class="sxs-lookup"><span data-stu-id="e39cd-189">Type</span></span>|<span data-ttu-id="e39cd-190">说明</span><span class="sxs-lookup"><span data-stu-id="e39cd-190">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e39cd-191">categories</span><span class="sxs-lookup"><span data-stu-id="e39cd-191">categories</span></span>|<span data-ttu-id="e39cd-192">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e39cd-192">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="e39cd-193">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="e39cd-193">The list of categories for this app.</span></span> <span data-ttu-id="e39cd-194">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-194">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39cd-195">assignments</span><span class="sxs-lookup"><span data-stu-id="e39cd-195">assignments</span></span>|<span data-ttu-id="e39cd-196">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e39cd-196">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="e39cd-197">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="e39cd-197">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="e39cd-198">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39cd-198">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39cd-199">contentVersions</span><span class="sxs-lookup"><span data-stu-id="e39cd-199">contentVersions</span></span>|<span data-ttu-id="e39cd-200">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e39cd-200">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="e39cd-201">此应用的内容版本列表。</span><span class="sxs-lookup"><span data-stu-id="e39cd-201">The list of content versions for this app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e39cd-202">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e39cd-202">JSON Representation</span></span>
<span data-ttu-id="e39cd-203">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e39cd-203">Here is a JSON representation of the resource.</span></span>
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



