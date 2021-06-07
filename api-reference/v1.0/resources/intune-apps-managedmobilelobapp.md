---
title: managedMobileLobApp 资源类型
description: 包含所有托管移动业务线应用的属性的抽象基类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f40d0c1e00595b70ebf30dea3c572ad364e3c668
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756027"
---
# <a name="managedmobilelobapp-resource-type"></a><span data-ttu-id="06538-103">managedMobileLobApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="06538-103">managedMobileLobApp resource type</span></span>

<span data-ttu-id="06538-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06538-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06538-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06538-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06538-106">包含所有托管移动业务线应用的属性的抽象基类。</span><span class="sxs-lookup"><span data-stu-id="06538-106">An abstract base class containing properties for all managed mobile line of business apps.</span></span>


<span data-ttu-id="06538-107">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-107">Inherits from [managedApp](../resources/intune-apps-managedapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="06538-108">Methods</span><span class="sxs-lookup"><span data-stu-id="06538-108">Methods</span></span>
|<span data-ttu-id="06538-109">方法</span><span class="sxs-lookup"><span data-stu-id="06538-109">Method</span></span>|<span data-ttu-id="06538-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="06538-110">Return Type</span></span>|<span data-ttu-id="06538-111">Description</span><span class="sxs-lookup"><span data-stu-id="06538-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06538-112">List managedMobileLobApps</span><span class="sxs-lookup"><span data-stu-id="06538-112">List managedMobileLobApps</span></span>](../api/intune-apps-managedmobilelobapp-list.md)|<span data-ttu-id="06538-113">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06538-113">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) collection</span></span>|<span data-ttu-id="06538-114">列出 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06538-114">List properties and relationships of the [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) objects.</span></span>|
|[<span data-ttu-id="06538-115">Get managedMobileLobApp</span><span class="sxs-lookup"><span data-stu-id="06538-115">Get managedMobileLobApp</span></span>](../api/intune-apps-managedmobilelobapp-get.md)|[<span data-ttu-id="06538-116">managedMobileLobApp</span><span class="sxs-lookup"><span data-stu-id="06538-116">managedMobileLobApp</span></span>](../resources/intune-apps-managedmobilelobapp.md)|<span data-ttu-id="06538-117">读取 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06538-117">Read properties and relationships of the [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06538-118">属性</span><span class="sxs-lookup"><span data-stu-id="06538-118">Properties</span></span>
|<span data-ttu-id="06538-119">属性</span><span class="sxs-lookup"><span data-stu-id="06538-119">Property</span></span>|<span data-ttu-id="06538-120">类型</span><span class="sxs-lookup"><span data-stu-id="06538-120">Type</span></span>|<span data-ttu-id="06538-121">说明</span><span class="sxs-lookup"><span data-stu-id="06538-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06538-122">id</span><span class="sxs-lookup"><span data-stu-id="06538-122">id</span></span>|<span data-ttu-id="06538-123">String</span><span class="sxs-lookup"><span data-stu-id="06538-123">String</span></span>|<span data-ttu-id="06538-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="06538-124">Key of the entity.</span></span> <span data-ttu-id="06538-125">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-125">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06538-126">displayName</span><span class="sxs-lookup"><span data-stu-id="06538-126">displayName</span></span>|<span data-ttu-id="06538-127">String</span><span class="sxs-lookup"><span data-stu-id="06538-127">String</span></span>|<span data-ttu-id="06538-128">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="06538-128">The admin provided or imported title of the app.</span></span> <span data-ttu-id="06538-129">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-129">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06538-130">说明</span><span class="sxs-lookup"><span data-stu-id="06538-130">description</span></span>|<span data-ttu-id="06538-131">String</span><span class="sxs-lookup"><span data-stu-id="06538-131">String</span></span>|<span data-ttu-id="06538-132">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="06538-132">The description of the app.</span></span> <span data-ttu-id="06538-133">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06538-134">publisher</span><span class="sxs-lookup"><span data-stu-id="06538-134">publisher</span></span>|<span data-ttu-id="06538-135">String</span><span class="sxs-lookup"><span data-stu-id="06538-135">String</span></span>|<span data-ttu-id="06538-136">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="06538-136">The publisher of the app.</span></span> <span data-ttu-id="06538-137">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06538-138">largeIcon</span><span class="sxs-lookup"><span data-stu-id="06538-138">largeIcon</span></span>|[<span data-ttu-id="06538-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="06538-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="06538-140">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="06538-140">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="06538-141">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06538-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06538-142">createdDateTime</span></span>|<span data-ttu-id="06538-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06538-143">DateTimeOffset</span></span>|<span data-ttu-id="06538-144">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="06538-144">The date and time the app was created.</span></span> <span data-ttu-id="06538-145">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06538-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06538-146">lastModifiedDateTime</span></span>|<span data-ttu-id="06538-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06538-147">DateTimeOffset</span></span>|<span data-ttu-id="06538-148">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="06538-148">The date and time the app was last modified.</span></span> <span data-ttu-id="06538-149">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06538-150">isFeatured</span><span class="sxs-lookup"><span data-stu-id="06538-150">isFeatured</span></span>|<span data-ttu-id="06538-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="06538-151">Boolean</span></span>|<span data-ttu-id="06538-152">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-152">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06538-153">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="06538-153">privacyInformationUrl</span></span>|<span data-ttu-id="06538-154">String</span><span class="sxs-lookup"><span data-stu-id="06538-154">String</span></span>|<span data-ttu-id="06538-155">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="06538-155">The privacy statement Url.</span></span> <span data-ttu-id="06538-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06538-157">informationUrl</span><span class="sxs-lookup"><span data-stu-id="06538-157">informationUrl</span></span>|<span data-ttu-id="06538-158">String</span><span class="sxs-lookup"><span data-stu-id="06538-158">String</span></span>|<span data-ttu-id="06538-159">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="06538-159">The more information Url.</span></span> <span data-ttu-id="06538-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06538-161">所有者</span><span class="sxs-lookup"><span data-stu-id="06538-161">owner</span></span>|<span data-ttu-id="06538-162">String</span><span class="sxs-lookup"><span data-stu-id="06538-162">String</span></span>|<span data-ttu-id="06538-163">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="06538-163">The owner of the app.</span></span> <span data-ttu-id="06538-164">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06538-165">developer</span><span class="sxs-lookup"><span data-stu-id="06538-165">developer</span></span>|<span data-ttu-id="06538-166">String</span><span class="sxs-lookup"><span data-stu-id="06538-166">String</span></span>|<span data-ttu-id="06538-167">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="06538-167">The developer of the app.</span></span> <span data-ttu-id="06538-168">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06538-169">notes</span><span class="sxs-lookup"><span data-stu-id="06538-169">notes</span></span>|<span data-ttu-id="06538-170">String</span><span class="sxs-lookup"><span data-stu-id="06538-170">String</span></span>|<span data-ttu-id="06538-171">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="06538-171">Notes for the app.</span></span> <span data-ttu-id="06538-172">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06538-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="06538-173">publishingState</span></span>|[<span data-ttu-id="06538-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="06538-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="06538-175">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="06538-175">The publishing state for the app.</span></span> <span data-ttu-id="06538-176">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="06538-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="06538-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="06538-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="06538-178">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="06538-178">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="06538-179">appAvailability</span><span class="sxs-lookup"><span data-stu-id="06538-179">appAvailability</span></span>|[<span data-ttu-id="06538-180">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="06538-180">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="06538-181">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="06538-181">The Application's availability.</span></span> <span data-ttu-id="06538-182">继承自 [managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="06538-182">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="06538-183">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="06538-183">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="06538-184">version</span><span class="sxs-lookup"><span data-stu-id="06538-184">version</span></span>|<span data-ttu-id="06538-185">String</span><span class="sxs-lookup"><span data-stu-id="06538-185">String</span></span>|<span data-ttu-id="06538-186">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="06538-186">The Application's version.</span></span> <span data-ttu-id="06538-187">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-187">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="06538-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="06538-188">committedContentVersion</span></span>|<span data-ttu-id="06538-189">String</span><span class="sxs-lookup"><span data-stu-id="06538-189">String</span></span>|<span data-ttu-id="06538-190">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="06538-190">The internal committed content version.</span></span>|
|<span data-ttu-id="06538-191">fileName</span><span class="sxs-lookup"><span data-stu-id="06538-191">fileName</span></span>|<span data-ttu-id="06538-192">String</span><span class="sxs-lookup"><span data-stu-id="06538-192">String</span></span>|<span data-ttu-id="06538-193">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="06538-193">The name of the main Lob application file.</span></span>|
|<span data-ttu-id="06538-194">size</span><span class="sxs-lookup"><span data-stu-id="06538-194">size</span></span>|<span data-ttu-id="06538-195">Int64</span><span class="sxs-lookup"><span data-stu-id="06538-195">Int64</span></span>|<span data-ttu-id="06538-196">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="06538-196">The total size, including all uploaded files.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06538-197">关系</span><span class="sxs-lookup"><span data-stu-id="06538-197">Relationships</span></span>
|<span data-ttu-id="06538-198">关系</span><span class="sxs-lookup"><span data-stu-id="06538-198">Relationship</span></span>|<span data-ttu-id="06538-199">类型</span><span class="sxs-lookup"><span data-stu-id="06538-199">Type</span></span>|<span data-ttu-id="06538-200">Description</span><span class="sxs-lookup"><span data-stu-id="06538-200">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06538-201">categories</span><span class="sxs-lookup"><span data-stu-id="06538-201">categories</span></span>|<span data-ttu-id="06538-202">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06538-202">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="06538-203">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="06538-203">The list of categories for this app.</span></span> <span data-ttu-id="06538-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06538-205">assignments</span><span class="sxs-lookup"><span data-stu-id="06538-205">assignments</span></span>|<span data-ttu-id="06538-206">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06538-206">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="06538-207">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="06538-207">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="06538-208">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06538-208">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06538-209">contentVersions</span><span class="sxs-lookup"><span data-stu-id="06538-209">contentVersions</span></span>|<span data-ttu-id="06538-210">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06538-210">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="06538-211">此应用的内容版本列表。</span><span class="sxs-lookup"><span data-stu-id="06538-211">The list of content versions for this app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06538-212">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06538-212">JSON Representation</span></span>
<span data-ttu-id="06538-213">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06538-213">Here is a JSON representation of the resource.</span></span>
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




