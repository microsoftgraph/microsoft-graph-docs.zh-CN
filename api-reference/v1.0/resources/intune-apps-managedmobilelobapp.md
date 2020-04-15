---
title: managedMobileLobApp 资源类型
description: 包含所有托管移动业务线应用的属性的抽象基类。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a8783a72f59f51e002544320d0e58b65ffd6c87d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43382456"
---
# <a name="managedmobilelobapp-resource-type"></a><span data-ttu-id="8b246-103">managedMobileLobApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b246-103">managedMobileLobApp resource type</span></span>

<span data-ttu-id="8b246-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b246-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b246-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8b246-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b246-106">包含所有托管移动业务线应用的属性的抽象基类。</span><span class="sxs-lookup"><span data-stu-id="8b246-106">An abstract base class containing properties for all managed mobile line of business apps.</span></span>


<span data-ttu-id="8b246-107">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-107">Inherits from [managedApp](../resources/intune-apps-managedapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8b246-108">方法</span><span class="sxs-lookup"><span data-stu-id="8b246-108">Methods</span></span>
|<span data-ttu-id="8b246-109">方法</span><span class="sxs-lookup"><span data-stu-id="8b246-109">Method</span></span>|<span data-ttu-id="8b246-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8b246-110">Return Type</span></span>|<span data-ttu-id="8b246-111">说明</span><span class="sxs-lookup"><span data-stu-id="8b246-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8b246-112">List managedMobileLobApps</span><span class="sxs-lookup"><span data-stu-id="8b246-112">List managedMobileLobApps</span></span>](../api/intune-apps-managedmobilelobapp-list.md)|<span data-ttu-id="8b246-113">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8b246-113">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) collection</span></span>|<span data-ttu-id="8b246-114">列出 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8b246-114">List properties and relationships of the [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) objects.</span></span>|
|[<span data-ttu-id="8b246-115">Get managedMobileLobApp</span><span class="sxs-lookup"><span data-stu-id="8b246-115">Get managedMobileLobApp</span></span>](../api/intune-apps-managedmobilelobapp-get.md)|[<span data-ttu-id="8b246-116">managedMobileLobApp</span><span class="sxs-lookup"><span data-stu-id="8b246-116">managedMobileLobApp</span></span>](../resources/intune-apps-managedmobilelobapp.md)|<span data-ttu-id="8b246-117">读取 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8b246-117">Read properties and relationships of the [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8b246-118">属性</span><span class="sxs-lookup"><span data-stu-id="8b246-118">Properties</span></span>
|<span data-ttu-id="8b246-119">属性</span><span class="sxs-lookup"><span data-stu-id="8b246-119">Property</span></span>|<span data-ttu-id="8b246-120">类型</span><span class="sxs-lookup"><span data-stu-id="8b246-120">Type</span></span>|<span data-ttu-id="8b246-121">说明</span><span class="sxs-lookup"><span data-stu-id="8b246-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b246-122">id</span><span class="sxs-lookup"><span data-stu-id="8b246-122">id</span></span>|<span data-ttu-id="8b246-123">字符串</span><span class="sxs-lookup"><span data-stu-id="8b246-123">String</span></span>|<span data-ttu-id="8b246-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8b246-124">Key of the entity.</span></span> <span data-ttu-id="8b246-125">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-125">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8b246-126">displayName</span><span class="sxs-lookup"><span data-stu-id="8b246-126">displayName</span></span>|<span data-ttu-id="8b246-127">String</span><span class="sxs-lookup"><span data-stu-id="8b246-127">String</span></span>|<span data-ttu-id="8b246-128">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="8b246-128">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8b246-129">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-129">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8b246-130">description</span><span class="sxs-lookup"><span data-stu-id="8b246-130">description</span></span>|<span data-ttu-id="8b246-131">字符串</span><span class="sxs-lookup"><span data-stu-id="8b246-131">String</span></span>|<span data-ttu-id="8b246-132">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="8b246-132">The description of the app.</span></span> <span data-ttu-id="8b246-133">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8b246-134">publisher</span><span class="sxs-lookup"><span data-stu-id="8b246-134">publisher</span></span>|<span data-ttu-id="8b246-135">String</span><span class="sxs-lookup"><span data-stu-id="8b246-135">String</span></span>|<span data-ttu-id="8b246-136">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="8b246-136">The publisher of the app.</span></span> <span data-ttu-id="8b246-137">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8b246-138">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8b246-138">largeIcon</span></span>|[<span data-ttu-id="8b246-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8b246-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8b246-140">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="8b246-140">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8b246-141">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8b246-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b246-142">createdDateTime</span></span>|<span data-ttu-id="8b246-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b246-143">DateTimeOffset</span></span>|<span data-ttu-id="8b246-144">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8b246-144">The date and time the app was created.</span></span> <span data-ttu-id="8b246-145">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8b246-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b246-146">lastModifiedDateTime</span></span>|<span data-ttu-id="8b246-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b246-147">DateTimeOffset</span></span>|<span data-ttu-id="8b246-148">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8b246-148">The date and time the app was last modified.</span></span> <span data-ttu-id="8b246-149">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8b246-150">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8b246-150">isFeatured</span></span>|<span data-ttu-id="8b246-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b246-151">Boolean</span></span>|<span data-ttu-id="8b246-152">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-152">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8b246-153">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8b246-153">privacyInformationUrl</span></span>|<span data-ttu-id="8b246-154">String</span><span class="sxs-lookup"><span data-stu-id="8b246-154">String</span></span>|<span data-ttu-id="8b246-155">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="8b246-155">The privacy statement Url.</span></span> <span data-ttu-id="8b246-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8b246-157">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8b246-157">informationUrl</span></span>|<span data-ttu-id="8b246-158">String</span><span class="sxs-lookup"><span data-stu-id="8b246-158">String</span></span>|<span data-ttu-id="8b246-159">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="8b246-159">The more information Url.</span></span> <span data-ttu-id="8b246-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8b246-161">owner</span><span class="sxs-lookup"><span data-stu-id="8b246-161">owner</span></span>|<span data-ttu-id="8b246-162">String</span><span class="sxs-lookup"><span data-stu-id="8b246-162">String</span></span>|<span data-ttu-id="8b246-163">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="8b246-163">The owner of the app.</span></span> <span data-ttu-id="8b246-164">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8b246-165">developer</span><span class="sxs-lookup"><span data-stu-id="8b246-165">developer</span></span>|<span data-ttu-id="8b246-166">String</span><span class="sxs-lookup"><span data-stu-id="8b246-166">String</span></span>|<span data-ttu-id="8b246-167">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="8b246-167">The developer of the app.</span></span> <span data-ttu-id="8b246-168">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8b246-169">notes</span><span class="sxs-lookup"><span data-stu-id="8b246-169">notes</span></span>|<span data-ttu-id="8b246-170">String</span><span class="sxs-lookup"><span data-stu-id="8b246-170">String</span></span>|<span data-ttu-id="8b246-171">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="8b246-171">Notes for the app.</span></span> <span data-ttu-id="8b246-172">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8b246-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="8b246-173">publishingState</span></span>|[<span data-ttu-id="8b246-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8b246-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8b246-175">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="8b246-175">The publishing state for the app.</span></span> <span data-ttu-id="8b246-176">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="8b246-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8b246-177">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="8b246-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8b246-178">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="8b246-178">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8b246-179">appAvailability</span><span class="sxs-lookup"><span data-stu-id="8b246-179">appAvailability</span></span>|[<span data-ttu-id="8b246-180">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="8b246-180">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="8b246-181">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="8b246-181">The Application's availability.</span></span> <span data-ttu-id="8b246-182">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="8b246-182">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="8b246-183">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="8b246-183">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="8b246-184">version</span><span class="sxs-lookup"><span data-stu-id="8b246-184">version</span></span>|<span data-ttu-id="8b246-185">String</span><span class="sxs-lookup"><span data-stu-id="8b246-185">String</span></span>|<span data-ttu-id="8b246-186">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="8b246-186">The Application's version.</span></span> <span data-ttu-id="8b246-187">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-187">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="8b246-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8b246-188">committedContentVersion</span></span>|<span data-ttu-id="8b246-189">String</span><span class="sxs-lookup"><span data-stu-id="8b246-189">String</span></span>|<span data-ttu-id="8b246-190">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="8b246-190">The internal committed content version.</span></span>|
|<span data-ttu-id="8b246-191">fileName</span><span class="sxs-lookup"><span data-stu-id="8b246-191">fileName</span></span>|<span data-ttu-id="8b246-192">String</span><span class="sxs-lookup"><span data-stu-id="8b246-192">String</span></span>|<span data-ttu-id="8b246-193">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="8b246-193">The name of the main Lob application file.</span></span>|
|<span data-ttu-id="8b246-194">size</span><span class="sxs-lookup"><span data-stu-id="8b246-194">size</span></span>|<span data-ttu-id="8b246-195">Int64</span><span class="sxs-lookup"><span data-stu-id="8b246-195">Int64</span></span>|<span data-ttu-id="8b246-196">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="8b246-196">The total size, including all uploaded files.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b246-197">关系</span><span class="sxs-lookup"><span data-stu-id="8b246-197">Relationships</span></span>
|<span data-ttu-id="8b246-198">关系</span><span class="sxs-lookup"><span data-stu-id="8b246-198">Relationship</span></span>|<span data-ttu-id="8b246-199">类型</span><span class="sxs-lookup"><span data-stu-id="8b246-199">Type</span></span>|<span data-ttu-id="8b246-200">说明</span><span class="sxs-lookup"><span data-stu-id="8b246-200">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b246-201">categories</span><span class="sxs-lookup"><span data-stu-id="8b246-201">categories</span></span>|<span data-ttu-id="8b246-202">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8b246-202">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="8b246-203">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="8b246-203">The list of categories for this app.</span></span> <span data-ttu-id="8b246-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8b246-205">assignments</span><span class="sxs-lookup"><span data-stu-id="8b246-205">assignments</span></span>|<span data-ttu-id="8b246-206">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8b246-206">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="8b246-207">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="8b246-207">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="8b246-208">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8b246-208">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8b246-209">contentVersions</span><span class="sxs-lookup"><span data-stu-id="8b246-209">contentVersions</span></span>|<span data-ttu-id="8b246-210">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8b246-210">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="8b246-211">此应用的内容版本列表。</span><span class="sxs-lookup"><span data-stu-id="8b246-211">The list of content versions for this app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8b246-212">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b246-212">JSON Representation</span></span>
<span data-ttu-id="8b246-213">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b246-213">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileLobApp",
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
  "appAvailability": "String",
  "version": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024
}
```







