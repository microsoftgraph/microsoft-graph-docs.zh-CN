---
title: mobileLobApp 资源类型
description: 包含所有移动业务线应用的属性的抽象基类。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1003d8e7e2ef0295f7635b478a0e5de32cf3414a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439650"
---
# <a name="mobilelobapp-resource-type"></a><span data-ttu-id="eb888-103">mobileLobApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb888-103">mobileLobApp resource type</span></span>

<span data-ttu-id="eb888-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb888-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb888-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb888-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb888-106">包含所有移动业务线应用的属性的抽象基类。</span><span class="sxs-lookup"><span data-stu-id="eb888-106">An abstract base class containing properties for all mobile line of business apps.</span></span>


<span data-ttu-id="eb888-107">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-107">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="eb888-108">方法</span><span class="sxs-lookup"><span data-stu-id="eb888-108">Methods</span></span>
|<span data-ttu-id="eb888-109">方法</span><span class="sxs-lookup"><span data-stu-id="eb888-109">Method</span></span>|<span data-ttu-id="eb888-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="eb888-110">Return Type</span></span>|<span data-ttu-id="eb888-111">说明</span><span class="sxs-lookup"><span data-stu-id="eb888-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eb888-112">List mobileLobApps</span><span class="sxs-lookup"><span data-stu-id="eb888-112">List mobileLobApps</span></span>](../api/intune-apps-mobilelobapp-list.md)|<span data-ttu-id="eb888-113">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb888-113">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) collection</span></span>|<span data-ttu-id="eb888-114">列出 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eb888-114">List properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects.</span></span>|
|[<span data-ttu-id="eb888-115">Get mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="eb888-115">Get mobileLobApp</span></span>](../api/intune-apps-mobilelobapp-get.md)|[<span data-ttu-id="eb888-116">mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="eb888-116">mobileLobApp</span></span>](../resources/intune-apps-mobilelobapp.md)|<span data-ttu-id="eb888-117">读取 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eb888-117">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="eb888-118">属性</span><span class="sxs-lookup"><span data-stu-id="eb888-118">Properties</span></span>
|<span data-ttu-id="eb888-119">属性</span><span class="sxs-lookup"><span data-stu-id="eb888-119">Property</span></span>|<span data-ttu-id="eb888-120">类型</span><span class="sxs-lookup"><span data-stu-id="eb888-120">Type</span></span>|<span data-ttu-id="eb888-121">说明</span><span class="sxs-lookup"><span data-stu-id="eb888-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb888-122">id</span><span class="sxs-lookup"><span data-stu-id="eb888-122">id</span></span>|<span data-ttu-id="eb888-123">字符串</span><span class="sxs-lookup"><span data-stu-id="eb888-123">String</span></span>|<span data-ttu-id="eb888-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="eb888-124">Key of the entity.</span></span> <span data-ttu-id="eb888-125">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-125">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb888-126">displayName</span><span class="sxs-lookup"><span data-stu-id="eb888-126">displayName</span></span>|<span data-ttu-id="eb888-127">String</span><span class="sxs-lookup"><span data-stu-id="eb888-127">String</span></span>|<span data-ttu-id="eb888-128">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="eb888-128">The admin provided or imported title of the app.</span></span> <span data-ttu-id="eb888-129">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-129">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb888-130">description</span><span class="sxs-lookup"><span data-stu-id="eb888-130">description</span></span>|<span data-ttu-id="eb888-131">字符串</span><span class="sxs-lookup"><span data-stu-id="eb888-131">String</span></span>|<span data-ttu-id="eb888-132">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="eb888-132">The description of the app.</span></span> <span data-ttu-id="eb888-133">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb888-134">publisher</span><span class="sxs-lookup"><span data-stu-id="eb888-134">publisher</span></span>|<span data-ttu-id="eb888-135">String</span><span class="sxs-lookup"><span data-stu-id="eb888-135">String</span></span>|<span data-ttu-id="eb888-136">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="eb888-136">The publisher of the app.</span></span> <span data-ttu-id="eb888-137">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb888-138">largeIcon</span><span class="sxs-lookup"><span data-stu-id="eb888-138">largeIcon</span></span>|[<span data-ttu-id="eb888-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="eb888-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="eb888-140">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="eb888-140">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="eb888-141">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb888-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb888-142">createdDateTime</span></span>|<span data-ttu-id="eb888-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb888-143">DateTimeOffset</span></span>|<span data-ttu-id="eb888-144">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="eb888-144">The date and time the app was created.</span></span> <span data-ttu-id="eb888-145">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb888-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb888-146">lastModifiedDateTime</span></span>|<span data-ttu-id="eb888-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb888-147">DateTimeOffset</span></span>|<span data-ttu-id="eb888-148">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="eb888-148">The date and time the app was last modified.</span></span> <span data-ttu-id="eb888-149">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb888-150">isFeatured</span><span class="sxs-lookup"><span data-stu-id="eb888-150">isFeatured</span></span>|<span data-ttu-id="eb888-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb888-151">Boolean</span></span>|<span data-ttu-id="eb888-152">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-152">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb888-153">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="eb888-153">privacyInformationUrl</span></span>|<span data-ttu-id="eb888-154">String</span><span class="sxs-lookup"><span data-stu-id="eb888-154">String</span></span>|<span data-ttu-id="eb888-155">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="eb888-155">The privacy statement Url.</span></span> <span data-ttu-id="eb888-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb888-157">informationUrl</span><span class="sxs-lookup"><span data-stu-id="eb888-157">informationUrl</span></span>|<span data-ttu-id="eb888-158">String</span><span class="sxs-lookup"><span data-stu-id="eb888-158">String</span></span>|<span data-ttu-id="eb888-159">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="eb888-159">The more information Url.</span></span> <span data-ttu-id="eb888-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb888-161">owner</span><span class="sxs-lookup"><span data-stu-id="eb888-161">owner</span></span>|<span data-ttu-id="eb888-162">String</span><span class="sxs-lookup"><span data-stu-id="eb888-162">String</span></span>|<span data-ttu-id="eb888-163">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="eb888-163">The owner of the app.</span></span> <span data-ttu-id="eb888-164">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb888-165">developer</span><span class="sxs-lookup"><span data-stu-id="eb888-165">developer</span></span>|<span data-ttu-id="eb888-166">String</span><span class="sxs-lookup"><span data-stu-id="eb888-166">String</span></span>|<span data-ttu-id="eb888-167">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="eb888-167">The developer of the app.</span></span> <span data-ttu-id="eb888-168">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb888-169">notes</span><span class="sxs-lookup"><span data-stu-id="eb888-169">notes</span></span>|<span data-ttu-id="eb888-170">String</span><span class="sxs-lookup"><span data-stu-id="eb888-170">String</span></span>|<span data-ttu-id="eb888-171">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="eb888-171">Notes for the app.</span></span> <span data-ttu-id="eb888-172">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb888-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="eb888-173">publishingState</span></span>|[<span data-ttu-id="eb888-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="eb888-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="eb888-175">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="eb888-175">The publishing state for the app.</span></span> <span data-ttu-id="eb888-176">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="eb888-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="eb888-177">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="eb888-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="eb888-178">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="eb888-178">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="eb888-179">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="eb888-179">committedContentVersion</span></span>|<span data-ttu-id="eb888-180">String</span><span class="sxs-lookup"><span data-stu-id="eb888-180">String</span></span>|<span data-ttu-id="eb888-181">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="eb888-181">The internal committed content version.</span></span>|
|<span data-ttu-id="eb888-182">fileName</span><span class="sxs-lookup"><span data-stu-id="eb888-182">fileName</span></span>|<span data-ttu-id="eb888-183">String</span><span class="sxs-lookup"><span data-stu-id="eb888-183">String</span></span>|<span data-ttu-id="eb888-184">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="eb888-184">The name of the main Lob application file.</span></span>|
|<span data-ttu-id="eb888-185">size</span><span class="sxs-lookup"><span data-stu-id="eb888-185">size</span></span>|<span data-ttu-id="eb888-186">Int64</span><span class="sxs-lookup"><span data-stu-id="eb888-186">Int64</span></span>|<span data-ttu-id="eb888-187">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="eb888-187">The total size, including all uploaded files.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb888-188">关系</span><span class="sxs-lookup"><span data-stu-id="eb888-188">Relationships</span></span>
|<span data-ttu-id="eb888-189">关系</span><span class="sxs-lookup"><span data-stu-id="eb888-189">Relationship</span></span>|<span data-ttu-id="eb888-190">类型</span><span class="sxs-lookup"><span data-stu-id="eb888-190">Type</span></span>|<span data-ttu-id="eb888-191">说明</span><span class="sxs-lookup"><span data-stu-id="eb888-191">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb888-192">categories</span><span class="sxs-lookup"><span data-stu-id="eb888-192">categories</span></span>|<span data-ttu-id="eb888-193">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb888-193">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="eb888-194">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="eb888-194">The list of categories for this app.</span></span> <span data-ttu-id="eb888-195">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-195">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb888-196">assignments</span><span class="sxs-lookup"><span data-stu-id="eb888-196">assignments</span></span>|<span data-ttu-id="eb888-197">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb888-197">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="eb888-198">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="eb888-198">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="eb888-199">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb888-199">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eb888-200">contentVersions</span><span class="sxs-lookup"><span data-stu-id="eb888-200">contentVersions</span></span>|<span data-ttu-id="eb888-201">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb888-201">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="eb888-202">此应用的内容版本列表。</span><span class="sxs-lookup"><span data-stu-id="eb888-202">The list of content versions for this app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb888-203">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb888-203">JSON Representation</span></span>
<span data-ttu-id="eb888-204">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb888-204">Here is a JSON representation of the resource.</span></span>
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







