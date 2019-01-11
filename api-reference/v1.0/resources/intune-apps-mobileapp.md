---
title: mobileApp 资源类型
description: 包含 Intune 移动应用基属性的抽象类。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aac7045bb446956b4df415a96e5c4a7b9cbbbbae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806613"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="6f9b1-103">mobileApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f9b1-103">mobileApp resource type</span></span>

> <span data-ttu-id="6f9b1-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f9b1-105">包含 Intune 移动应用基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-105">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="6f9b1-106">方法</span><span class="sxs-lookup"><span data-stu-id="6f9b1-106">Methods</span></span>
|<span data-ttu-id="6f9b1-107">方法</span><span class="sxs-lookup"><span data-stu-id="6f9b1-107">Method</span></span>|<span data-ttu-id="6f9b1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="6f9b1-108">Return Type</span></span>|<span data-ttu-id="6f9b1-109">说明</span><span class="sxs-lookup"><span data-stu-id="6f9b1-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6f9b1-110">List mobileApps</span><span class="sxs-lookup"><span data-stu-id="6f9b1-110">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="6f9b1-111">[mobileApp](../resources/intune-apps-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6f9b1-111">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="6f9b1-112">列出 [mobileApp](../resources/intune-apps-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-112">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="6f9b1-113">Get mobileApp</span><span class="sxs-lookup"><span data-stu-id="6f9b1-113">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="6f9b1-114">mobileApp</span><span class="sxs-lookup"><span data-stu-id="6f9b1-114">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="6f9b1-115">读取 [mobileApp](../resources/intune-apps-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-115">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="6f9b1-116">assign 操作</span><span class="sxs-lookup"><span data-stu-id="6f9b1-116">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="6f9b1-117">无</span><span class="sxs-lookup"><span data-stu-id="6f9b1-117">None</span></span>|<span data-ttu-id="6f9b1-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6f9b1-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6f9b1-119">属性</span><span class="sxs-lookup"><span data-stu-id="6f9b1-119">Properties</span></span>
|<span data-ttu-id="6f9b1-120">属性</span><span class="sxs-lookup"><span data-stu-id="6f9b1-120">Property</span></span>|<span data-ttu-id="6f9b1-121">类型</span><span class="sxs-lookup"><span data-stu-id="6f9b1-121">Type</span></span>|<span data-ttu-id="6f9b1-122">说明</span><span class="sxs-lookup"><span data-stu-id="6f9b1-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f9b1-123">id</span><span class="sxs-lookup"><span data-stu-id="6f9b1-123">id</span></span>|<span data-ttu-id="6f9b1-124">String</span><span class="sxs-lookup"><span data-stu-id="6f9b1-124">String</span></span>|<span data-ttu-id="6f9b1-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-125">Key of the entity.</span></span>|
|<span data-ttu-id="6f9b1-126">displayName</span><span class="sxs-lookup"><span data-stu-id="6f9b1-126">displayName</span></span>|<span data-ttu-id="6f9b1-127">String</span><span class="sxs-lookup"><span data-stu-id="6f9b1-127">String</span></span>|<span data-ttu-id="6f9b1-128">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-128">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="6f9b1-129">description</span><span class="sxs-lookup"><span data-stu-id="6f9b1-129">description</span></span>|<span data-ttu-id="6f9b1-130">String</span><span class="sxs-lookup"><span data-stu-id="6f9b1-130">String</span></span>|<span data-ttu-id="6f9b1-131">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-131">The description of the app.</span></span>|
|<span data-ttu-id="6f9b1-132">publisher</span><span class="sxs-lookup"><span data-stu-id="6f9b1-132">publisher</span></span>|<span data-ttu-id="6f9b1-133">String</span><span class="sxs-lookup"><span data-stu-id="6f9b1-133">String</span></span>|<span data-ttu-id="6f9b1-134">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-134">The publisher of the app.</span></span>|
|<span data-ttu-id="6f9b1-135">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6f9b1-135">largeIcon</span></span>|[<span data-ttu-id="6f9b1-136">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6f9b1-136">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6f9b1-137">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-137">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="6f9b1-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f9b1-138">createdDateTime</span></span>|<span data-ttu-id="6f9b1-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f9b1-139">DateTimeOffset</span></span>|<span data-ttu-id="6f9b1-140">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-140">The date and time the app was created.</span></span>|
|<span data-ttu-id="6f9b1-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f9b1-141">lastModifiedDateTime</span></span>|<span data-ttu-id="6f9b1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f9b1-142">DateTimeOffset</span></span>|<span data-ttu-id="6f9b1-143">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-143">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="6f9b1-144">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6f9b1-144">isFeatured</span></span>|<span data-ttu-id="6f9b1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f9b1-145">Boolean</span></span>|<span data-ttu-id="6f9b1-146">指示应用是否被管理员标记为特色的值。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-146">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="6f9b1-147">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6f9b1-147">privacyInformationUrl</span></span>|<span data-ttu-id="6f9b1-148">String</span><span class="sxs-lookup"><span data-stu-id="6f9b1-148">String</span></span>|<span data-ttu-id="6f9b1-149">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-149">The privacy statement Url.</span></span>|
|<span data-ttu-id="6f9b1-150">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6f9b1-150">informationUrl</span></span>|<span data-ttu-id="6f9b1-151">String</span><span class="sxs-lookup"><span data-stu-id="6f9b1-151">String</span></span>|<span data-ttu-id="6f9b1-152">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-152">The more information Url.</span></span>|
|<span data-ttu-id="6f9b1-153">owner</span><span class="sxs-lookup"><span data-stu-id="6f9b1-153">owner</span></span>|<span data-ttu-id="6f9b1-154">String</span><span class="sxs-lookup"><span data-stu-id="6f9b1-154">String</span></span>|<span data-ttu-id="6f9b1-155">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-155">The owner of the app.</span></span>|
|<span data-ttu-id="6f9b1-156">developer</span><span class="sxs-lookup"><span data-stu-id="6f9b1-156">developer</span></span>|<span data-ttu-id="6f9b1-157">String</span><span class="sxs-lookup"><span data-stu-id="6f9b1-157">String</span></span>|<span data-ttu-id="6f9b1-158">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-158">The developer of the app.</span></span>|
|<span data-ttu-id="6f9b1-159">notes</span><span class="sxs-lookup"><span data-stu-id="6f9b1-159">notes</span></span>|<span data-ttu-id="6f9b1-160">String</span><span class="sxs-lookup"><span data-stu-id="6f9b1-160">String</span></span>|<span data-ttu-id="6f9b1-161">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-161">Notes for the app.</span></span>|
|<span data-ttu-id="6f9b1-162">publishingState</span><span class="sxs-lookup"><span data-stu-id="6f9b1-162">publishingState</span></span>|[<span data-ttu-id="6f9b1-163">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6f9b1-163">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6f9b1-164">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-164">The publishing state for the app.</span></span> <span data-ttu-id="6f9b1-165">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-165">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6f9b1-166">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-166">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f9b1-167">Relationships</span><span class="sxs-lookup"><span data-stu-id="6f9b1-167">Relationships</span></span>
|<span data-ttu-id="6f9b1-168">关系</span><span class="sxs-lookup"><span data-stu-id="6f9b1-168">Relationship</span></span>|<span data-ttu-id="6f9b1-169">类型</span><span class="sxs-lookup"><span data-stu-id="6f9b1-169">Type</span></span>|<span data-ttu-id="6f9b1-170">说明</span><span class="sxs-lookup"><span data-stu-id="6f9b1-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f9b1-171">categories</span><span class="sxs-lookup"><span data-stu-id="6f9b1-171">categories</span></span>|<span data-ttu-id="6f9b1-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6f9b1-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="6f9b1-173">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-173">The list of categories for this app.</span></span>|
|<span data-ttu-id="6f9b1-174">assignments</span><span class="sxs-lookup"><span data-stu-id="6f9b1-174">assignments</span></span>|<span data-ttu-id="6f9b1-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6f9b1-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="6f9b1-176">此移动应用的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-176">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f9b1-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f9b1-177">JSON Representation</span></span>
<span data-ttu-id="6f9b1-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f9b1-178">Here is a JSON representation of the resource.</span></span>
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
  "publishingState": "String"
}
```



