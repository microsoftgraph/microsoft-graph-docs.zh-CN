---
title: mobileApp 资源类型
description: 包含 Intune 移动应用基属性的抽象类。
ms.openlocfilehash: 1c3c573d0802cd937cdb44d9a2fdacf5cdbc6e56
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048005"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="06039-103">mobileApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="06039-103">mobileApp resource type</span></span>

> <span data-ttu-id="06039-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="06039-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06039-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="06039-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06039-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="06039-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06039-107">包含 Intune 移动应用基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="06039-107">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="06039-108">方法</span><span class="sxs-lookup"><span data-stu-id="06039-108">Methods</span></span>
|<span data-ttu-id="06039-109">方法</span><span class="sxs-lookup"><span data-stu-id="06039-109">Method</span></span>|<span data-ttu-id="06039-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="06039-110">Return Type</span></span>|<span data-ttu-id="06039-111">说明</span><span class="sxs-lookup"><span data-stu-id="06039-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06039-112">List mobileApps</span><span class="sxs-lookup"><span data-stu-id="06039-112">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="06039-113">[mobileApp](../resources/intune-apps-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06039-113">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="06039-114">列出 [mobileApp](../resources/intune-apps-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06039-114">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="06039-115">Get mobileApp</span><span class="sxs-lookup"><span data-stu-id="06039-115">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="06039-116">mobileApp</span><span class="sxs-lookup"><span data-stu-id="06039-116">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="06039-117">读取 [mobileApp](../resources/intune-apps-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06039-117">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="06039-118">assign 操作</span><span class="sxs-lookup"><span data-stu-id="06039-118">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="06039-119">无</span><span class="sxs-lookup"><span data-stu-id="06039-119">None</span></span>|<span data-ttu-id="06039-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="06039-120">Not yet documented</span></span>|
|[<span data-ttu-id="06039-121">getMobileAppCount 函数</span><span class="sxs-lookup"><span data-stu-id="06039-121">getMobileAppCount function</span></span>](../api/intune-apps-mobileapp-getmobileappcount.md)|<span data-ttu-id="06039-122">Int64</span><span class="sxs-lookup"><span data-stu-id="06039-122">Int64</span></span>|<span data-ttu-id="06039-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="06039-123">Not yet documented</span></span>|
|[<span data-ttu-id="06039-124">getTopMobileApps 函数</span><span class="sxs-lookup"><span data-stu-id="06039-124">getTopMobileApps function</span></span>](../api/intune-apps-mobileapp-gettopmobileapps.md)|<span data-ttu-id="06039-125">[mobileApp](../resources/intune-apps-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06039-125">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="06039-126">尚未记录</span><span class="sxs-lookup"><span data-stu-id="06039-126">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="06039-127">属性</span><span class="sxs-lookup"><span data-stu-id="06039-127">Properties</span></span>
|<span data-ttu-id="06039-128">属性</span><span class="sxs-lookup"><span data-stu-id="06039-128">Property</span></span>|<span data-ttu-id="06039-129">类型</span><span class="sxs-lookup"><span data-stu-id="06039-129">Type</span></span>|<span data-ttu-id="06039-130">说明</span><span class="sxs-lookup"><span data-stu-id="06039-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06039-131">id</span><span class="sxs-lookup"><span data-stu-id="06039-131">id</span></span>|<span data-ttu-id="06039-132">String</span><span class="sxs-lookup"><span data-stu-id="06039-132">String</span></span>|<span data-ttu-id="06039-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="06039-133">Key of the entity.</span></span>|
|<span data-ttu-id="06039-134">displayName</span><span class="sxs-lookup"><span data-stu-id="06039-134">displayName</span></span>|<span data-ttu-id="06039-135">String</span><span class="sxs-lookup"><span data-stu-id="06039-135">String</span></span>|<span data-ttu-id="06039-136">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="06039-136">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="06039-137">description</span><span class="sxs-lookup"><span data-stu-id="06039-137">description</span></span>|<span data-ttu-id="06039-138">String</span><span class="sxs-lookup"><span data-stu-id="06039-138">String</span></span>|<span data-ttu-id="06039-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="06039-139">The description of the app.</span></span>|
|<span data-ttu-id="06039-140">publisher</span><span class="sxs-lookup"><span data-stu-id="06039-140">publisher</span></span>|<span data-ttu-id="06039-141">String</span><span class="sxs-lookup"><span data-stu-id="06039-141">String</span></span>|<span data-ttu-id="06039-142">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="06039-142">The publisher of the app.</span></span>|
|<span data-ttu-id="06039-143">largeIcon</span><span class="sxs-lookup"><span data-stu-id="06039-143">largeIcon</span></span>|[<span data-ttu-id="06039-144">mimeContent</span><span class="sxs-lookup"><span data-stu-id="06039-144">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="06039-145">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="06039-145">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="06039-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06039-146">createdDateTime</span></span>|<span data-ttu-id="06039-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06039-147">DateTimeOffset</span></span>|<span data-ttu-id="06039-148">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="06039-148">The date and time the app was created.</span></span>|
|<span data-ttu-id="06039-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06039-149">lastModifiedDateTime</span></span>|<span data-ttu-id="06039-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06039-150">DateTimeOffset</span></span>|<span data-ttu-id="06039-151">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="06039-151">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="06039-152">isFeatured</span><span class="sxs-lookup"><span data-stu-id="06039-152">isFeatured</span></span>|<span data-ttu-id="06039-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="06039-153">Boolean</span></span>|<span data-ttu-id="06039-154">指示应用是否被管理员标记为特色的值。</span><span class="sxs-lookup"><span data-stu-id="06039-154">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="06039-155">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="06039-155">privacyInformationUrl</span></span>|<span data-ttu-id="06039-156">String</span><span class="sxs-lookup"><span data-stu-id="06039-156">String</span></span>|<span data-ttu-id="06039-157">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="06039-157">The privacy statement Url.</span></span>|
|<span data-ttu-id="06039-158">informationUrl</span><span class="sxs-lookup"><span data-stu-id="06039-158">informationUrl</span></span>|<span data-ttu-id="06039-159">String</span><span class="sxs-lookup"><span data-stu-id="06039-159">String</span></span>|<span data-ttu-id="06039-160">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="06039-160">The more information Url.</span></span>|
|<span data-ttu-id="06039-161">owner</span><span class="sxs-lookup"><span data-stu-id="06039-161">owner</span></span>|<span data-ttu-id="06039-162">String</span><span class="sxs-lookup"><span data-stu-id="06039-162">String</span></span>|<span data-ttu-id="06039-163">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="06039-163">The owner of the app.</span></span>|
|<span data-ttu-id="06039-164">developer</span><span class="sxs-lookup"><span data-stu-id="06039-164">developer</span></span>|<span data-ttu-id="06039-165">String</span><span class="sxs-lookup"><span data-stu-id="06039-165">String</span></span>|<span data-ttu-id="06039-166">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="06039-166">The developer of the app.</span></span>|
|<span data-ttu-id="06039-167">notes</span><span class="sxs-lookup"><span data-stu-id="06039-167">notes</span></span>|<span data-ttu-id="06039-168">String</span><span class="sxs-lookup"><span data-stu-id="06039-168">String</span></span>|<span data-ttu-id="06039-169">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="06039-169">Notes for the app.</span></span>|
|<span data-ttu-id="06039-170">uploadState</span><span class="sxs-lookup"><span data-stu-id="06039-170">uploadState</span></span>|<span data-ttu-id="06039-171">Int32</span><span class="sxs-lookup"><span data-stu-id="06039-171">Int32</span></span>|<span data-ttu-id="06039-172">上载状态。</span><span class="sxs-lookup"><span data-stu-id="06039-172">The upload state.</span></span>|
|<span data-ttu-id="06039-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="06039-173">publishingState</span></span>|[<span data-ttu-id="06039-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="06039-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="06039-175">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="06039-175">The publishing state for the app.</span></span> <span data-ttu-id="06039-176">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="06039-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="06039-177">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="06039-177">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06039-178">Relationships</span><span class="sxs-lookup"><span data-stu-id="06039-178">Relationships</span></span>
|<span data-ttu-id="06039-179">关系</span><span class="sxs-lookup"><span data-stu-id="06039-179">Relationship</span></span>|<span data-ttu-id="06039-180">类型</span><span class="sxs-lookup"><span data-stu-id="06039-180">Type</span></span>|<span data-ttu-id="06039-181">说明</span><span class="sxs-lookup"><span data-stu-id="06039-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06039-182">categories</span><span class="sxs-lookup"><span data-stu-id="06039-182">categories</span></span>|<span data-ttu-id="06039-183">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06039-183">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="06039-184">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="06039-184">The list of categories for this app.</span></span>|
|<span data-ttu-id="06039-185">assignments</span><span class="sxs-lookup"><span data-stu-id="06039-185">assignments</span></span>|<span data-ttu-id="06039-186">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06039-186">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="06039-187">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="06039-187">The list of group assignments for this mobile app.</span></span>|
|<span data-ttu-id="06039-188">installSummary</span><span class="sxs-lookup"><span data-stu-id="06039-188">installSummary</span></span>|[<span data-ttu-id="06039-189">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="06039-189">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="06039-190">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="06039-190">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="06039-191">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="06039-191">deviceStatuses</span></span>|<span data-ttu-id="06039-192">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="06039-192">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="06039-193">此移动应用程序的安装状态的列表。</span><span class="sxs-lookup"><span data-stu-id="06039-193">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="06039-194">userStatuses</span><span class="sxs-lookup"><span data-stu-id="06039-194">userStatuses</span></span>|<span data-ttu-id="06039-195">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="06039-195">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="06039-196">此移动应用程序的安装状态的列表。</span><span class="sxs-lookup"><span data-stu-id="06039-196">The list of installation states for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06039-197">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06039-197">JSON Representation</span></span>
<span data-ttu-id="06039-198">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06039-198">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
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
  "uploadState": 1024,
  "publishingState": "String"
}
```





