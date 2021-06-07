---
title: mobileLobApp 资源类型
description: 包含所有移动业务线应用的属性的抽象基类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a9c3673618ea15547a61a93a0af9b11a80cc66f8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756006"
---
# <a name="mobilelobapp-resource-type"></a><span data-ttu-id="d348e-103">mobileLobApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="d348e-103">mobileLobApp resource type</span></span>

<span data-ttu-id="d348e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d348e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d348e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d348e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d348e-106">包含所有移动业务线应用的属性的抽象基类。</span><span class="sxs-lookup"><span data-stu-id="d348e-106">An abstract base class containing properties for all mobile line of business apps.</span></span>


<span data-ttu-id="d348e-107">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-107">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d348e-108">Methods</span><span class="sxs-lookup"><span data-stu-id="d348e-108">Methods</span></span>
|<span data-ttu-id="d348e-109">方法</span><span class="sxs-lookup"><span data-stu-id="d348e-109">Method</span></span>|<span data-ttu-id="d348e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d348e-110">Return Type</span></span>|<span data-ttu-id="d348e-111">Description</span><span class="sxs-lookup"><span data-stu-id="d348e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d348e-112">List mobileLobApps</span><span class="sxs-lookup"><span data-stu-id="d348e-112">List mobileLobApps</span></span>](../api/intune-apps-mobilelobapp-list.md)|<span data-ttu-id="d348e-113">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d348e-113">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) collection</span></span>|<span data-ttu-id="d348e-114">列出 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d348e-114">List properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects.</span></span>|
|[<span data-ttu-id="d348e-115">Get mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="d348e-115">Get mobileLobApp</span></span>](../api/intune-apps-mobilelobapp-get.md)|[<span data-ttu-id="d348e-116">mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="d348e-116">mobileLobApp</span></span>](../resources/intune-apps-mobilelobapp.md)|<span data-ttu-id="d348e-117">读取 [mobileLobApp](../resources/intune-apps-mobilelobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d348e-117">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d348e-118">属性</span><span class="sxs-lookup"><span data-stu-id="d348e-118">Properties</span></span>
|<span data-ttu-id="d348e-119">属性</span><span class="sxs-lookup"><span data-stu-id="d348e-119">Property</span></span>|<span data-ttu-id="d348e-120">类型</span><span class="sxs-lookup"><span data-stu-id="d348e-120">Type</span></span>|<span data-ttu-id="d348e-121">说明</span><span class="sxs-lookup"><span data-stu-id="d348e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d348e-122">id</span><span class="sxs-lookup"><span data-stu-id="d348e-122">id</span></span>|<span data-ttu-id="d348e-123">String</span><span class="sxs-lookup"><span data-stu-id="d348e-123">String</span></span>|<span data-ttu-id="d348e-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d348e-124">Key of the entity.</span></span> <span data-ttu-id="d348e-125">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-125">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d348e-126">displayName</span><span class="sxs-lookup"><span data-stu-id="d348e-126">displayName</span></span>|<span data-ttu-id="d348e-127">String</span><span class="sxs-lookup"><span data-stu-id="d348e-127">String</span></span>|<span data-ttu-id="d348e-128">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="d348e-128">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d348e-129">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-129">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d348e-130">说明</span><span class="sxs-lookup"><span data-stu-id="d348e-130">description</span></span>|<span data-ttu-id="d348e-131">String</span><span class="sxs-lookup"><span data-stu-id="d348e-131">String</span></span>|<span data-ttu-id="d348e-132">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="d348e-132">The description of the app.</span></span> <span data-ttu-id="d348e-133">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d348e-134">publisher</span><span class="sxs-lookup"><span data-stu-id="d348e-134">publisher</span></span>|<span data-ttu-id="d348e-135">String</span><span class="sxs-lookup"><span data-stu-id="d348e-135">String</span></span>|<span data-ttu-id="d348e-136">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="d348e-136">The publisher of the app.</span></span> <span data-ttu-id="d348e-137">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d348e-138">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d348e-138">largeIcon</span></span>|[<span data-ttu-id="d348e-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d348e-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d348e-140">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="d348e-140">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d348e-141">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d348e-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d348e-142">createdDateTime</span></span>|<span data-ttu-id="d348e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d348e-143">DateTimeOffset</span></span>|<span data-ttu-id="d348e-144">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d348e-144">The date and time the app was created.</span></span> <span data-ttu-id="d348e-145">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d348e-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d348e-146">lastModifiedDateTime</span></span>|<span data-ttu-id="d348e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d348e-147">DateTimeOffset</span></span>|<span data-ttu-id="d348e-148">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d348e-148">The date and time the app was last modified.</span></span> <span data-ttu-id="d348e-149">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d348e-150">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d348e-150">isFeatured</span></span>|<span data-ttu-id="d348e-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="d348e-151">Boolean</span></span>|<span data-ttu-id="d348e-152">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-152">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d348e-153">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d348e-153">privacyInformationUrl</span></span>|<span data-ttu-id="d348e-154">String</span><span class="sxs-lookup"><span data-stu-id="d348e-154">String</span></span>|<span data-ttu-id="d348e-155">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="d348e-155">The privacy statement Url.</span></span> <span data-ttu-id="d348e-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d348e-157">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d348e-157">informationUrl</span></span>|<span data-ttu-id="d348e-158">String</span><span class="sxs-lookup"><span data-stu-id="d348e-158">String</span></span>|<span data-ttu-id="d348e-159">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="d348e-159">The more information Url.</span></span> <span data-ttu-id="d348e-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d348e-161">所有者</span><span class="sxs-lookup"><span data-stu-id="d348e-161">owner</span></span>|<span data-ttu-id="d348e-162">String</span><span class="sxs-lookup"><span data-stu-id="d348e-162">String</span></span>|<span data-ttu-id="d348e-163">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="d348e-163">The owner of the app.</span></span> <span data-ttu-id="d348e-164">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d348e-165">developer</span><span class="sxs-lookup"><span data-stu-id="d348e-165">developer</span></span>|<span data-ttu-id="d348e-166">String</span><span class="sxs-lookup"><span data-stu-id="d348e-166">String</span></span>|<span data-ttu-id="d348e-167">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="d348e-167">The developer of the app.</span></span> <span data-ttu-id="d348e-168">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d348e-169">notes</span><span class="sxs-lookup"><span data-stu-id="d348e-169">notes</span></span>|<span data-ttu-id="d348e-170">String</span><span class="sxs-lookup"><span data-stu-id="d348e-170">String</span></span>|<span data-ttu-id="d348e-171">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="d348e-171">Notes for the app.</span></span> <span data-ttu-id="d348e-172">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d348e-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="d348e-173">publishingState</span></span>|[<span data-ttu-id="d348e-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d348e-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d348e-175">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="d348e-175">The publishing state for the app.</span></span> <span data-ttu-id="d348e-176">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="d348e-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d348e-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="d348e-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d348e-178">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="d348e-178">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d348e-179">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d348e-179">committedContentVersion</span></span>|<span data-ttu-id="d348e-180">String</span><span class="sxs-lookup"><span data-stu-id="d348e-180">String</span></span>|<span data-ttu-id="d348e-181">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="d348e-181">The internal committed content version.</span></span>|
|<span data-ttu-id="d348e-182">fileName</span><span class="sxs-lookup"><span data-stu-id="d348e-182">fileName</span></span>|<span data-ttu-id="d348e-183">String</span><span class="sxs-lookup"><span data-stu-id="d348e-183">String</span></span>|<span data-ttu-id="d348e-184">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="d348e-184">The name of the main Lob application file.</span></span>|
|<span data-ttu-id="d348e-185">size</span><span class="sxs-lookup"><span data-stu-id="d348e-185">size</span></span>|<span data-ttu-id="d348e-186">Int64</span><span class="sxs-lookup"><span data-stu-id="d348e-186">Int64</span></span>|<span data-ttu-id="d348e-187">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="d348e-187">The total size, including all uploaded files.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d348e-188">关系</span><span class="sxs-lookup"><span data-stu-id="d348e-188">Relationships</span></span>
|<span data-ttu-id="d348e-189">关系</span><span class="sxs-lookup"><span data-stu-id="d348e-189">Relationship</span></span>|<span data-ttu-id="d348e-190">类型</span><span class="sxs-lookup"><span data-stu-id="d348e-190">Type</span></span>|<span data-ttu-id="d348e-191">Description</span><span class="sxs-lookup"><span data-stu-id="d348e-191">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d348e-192">categories</span><span class="sxs-lookup"><span data-stu-id="d348e-192">categories</span></span>|<span data-ttu-id="d348e-193">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d348e-193">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="d348e-194">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="d348e-194">The list of categories for this app.</span></span> <span data-ttu-id="d348e-195">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-195">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d348e-196">assignments</span><span class="sxs-lookup"><span data-stu-id="d348e-196">assignments</span></span>|<span data-ttu-id="d348e-197">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d348e-197">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="d348e-198">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="d348e-198">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="d348e-199">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d348e-199">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d348e-200">contentVersions</span><span class="sxs-lookup"><span data-stu-id="d348e-200">contentVersions</span></span>|<span data-ttu-id="d348e-201">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d348e-201">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="d348e-202">此应用的内容版本列表。</span><span class="sxs-lookup"><span data-stu-id="d348e-202">The list of content versions for this app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d348e-203">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d348e-203">JSON Representation</span></span>
<span data-ttu-id="d348e-204">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d348e-204">Here is a JSON representation of the resource.</span></span>
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




