---
title: mobileApp 资源类型
description: 包含 Intune 移动应用基属性的抽象类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 69e1e604fe3cc2cfc0702f54fcdc48e8941cf7ed
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368104"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="bf815-103">mobileApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf815-103">mobileApp resource type</span></span>

> <span data-ttu-id="bf815-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf815-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf815-105">包含 Intune 移动应用基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="bf815-105">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="bf815-106">方法</span><span class="sxs-lookup"><span data-stu-id="bf815-106">Methods</span></span>
|<span data-ttu-id="bf815-107">方法</span><span class="sxs-lookup"><span data-stu-id="bf815-107">Method</span></span>|<span data-ttu-id="bf815-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="bf815-108">Return Type</span></span>|<span data-ttu-id="bf815-109">说明</span><span class="sxs-lookup"><span data-stu-id="bf815-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bf815-110">List mobileApps</span><span class="sxs-lookup"><span data-stu-id="bf815-110">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="bf815-111">[mobileApp](../resources/intune-apps-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bf815-111">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="bf815-112">列出 [mobileApp](../resources/intune-apps-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bf815-112">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="bf815-113">Get mobileApp</span><span class="sxs-lookup"><span data-stu-id="bf815-113">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="bf815-114">mobileApp</span><span class="sxs-lookup"><span data-stu-id="bf815-114">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="bf815-115">读取 [mobileApp](../resources/intune-apps-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bf815-115">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="bf815-116">assign 操作</span><span class="sxs-lookup"><span data-stu-id="bf815-116">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="bf815-117">无</span><span class="sxs-lookup"><span data-stu-id="bf815-117">None</span></span>|<span data-ttu-id="bf815-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bf815-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="bf815-119">属性</span><span class="sxs-lookup"><span data-stu-id="bf815-119">Properties</span></span>
|<span data-ttu-id="bf815-120">属性</span><span class="sxs-lookup"><span data-stu-id="bf815-120">Property</span></span>|<span data-ttu-id="bf815-121">类型</span><span class="sxs-lookup"><span data-stu-id="bf815-121">Type</span></span>|<span data-ttu-id="bf815-122">说明</span><span class="sxs-lookup"><span data-stu-id="bf815-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf815-123">id</span><span class="sxs-lookup"><span data-stu-id="bf815-123">id</span></span>|<span data-ttu-id="bf815-124">字符串</span><span class="sxs-lookup"><span data-stu-id="bf815-124">String</span></span>|<span data-ttu-id="bf815-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bf815-125">Key of the entity.</span></span>|
|<span data-ttu-id="bf815-126">displayName</span><span class="sxs-lookup"><span data-stu-id="bf815-126">displayName</span></span>|<span data-ttu-id="bf815-127">String</span><span class="sxs-lookup"><span data-stu-id="bf815-127">String</span></span>|<span data-ttu-id="bf815-128">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="bf815-128">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="bf815-129">说明</span><span class="sxs-lookup"><span data-stu-id="bf815-129">description</span></span>|<span data-ttu-id="bf815-130">字符串</span><span class="sxs-lookup"><span data-stu-id="bf815-130">String</span></span>|<span data-ttu-id="bf815-131">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="bf815-131">The description of the app.</span></span>|
|<span data-ttu-id="bf815-132">publisher</span><span class="sxs-lookup"><span data-stu-id="bf815-132">publisher</span></span>|<span data-ttu-id="bf815-133">String</span><span class="sxs-lookup"><span data-stu-id="bf815-133">String</span></span>|<span data-ttu-id="bf815-134">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="bf815-134">The publisher of the app.</span></span>|
|<span data-ttu-id="bf815-135">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bf815-135">largeIcon</span></span>|[<span data-ttu-id="bf815-136">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bf815-136">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bf815-137">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="bf815-137">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="bf815-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf815-138">createdDateTime</span></span>|<span data-ttu-id="bf815-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf815-139">DateTimeOffset</span></span>|<span data-ttu-id="bf815-140">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bf815-140">The date and time the app was created.</span></span>|
|<span data-ttu-id="bf815-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf815-141">lastModifiedDateTime</span></span>|<span data-ttu-id="bf815-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf815-142">DateTimeOffset</span></span>|<span data-ttu-id="bf815-143">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bf815-143">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="bf815-144">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bf815-144">isFeatured</span></span>|<span data-ttu-id="bf815-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf815-145">Boolean</span></span>|<span data-ttu-id="bf815-146">指示应用是否被管理员标记为特色的值。</span><span class="sxs-lookup"><span data-stu-id="bf815-146">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="bf815-147">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bf815-147">privacyInformationUrl</span></span>|<span data-ttu-id="bf815-148">String</span><span class="sxs-lookup"><span data-stu-id="bf815-148">String</span></span>|<span data-ttu-id="bf815-149">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="bf815-149">The privacy statement Url.</span></span>|
|<span data-ttu-id="bf815-150">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bf815-150">informationUrl</span></span>|<span data-ttu-id="bf815-151">String</span><span class="sxs-lookup"><span data-stu-id="bf815-151">String</span></span>|<span data-ttu-id="bf815-152">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="bf815-152">The more information Url.</span></span>|
|<span data-ttu-id="bf815-153">owner</span><span class="sxs-lookup"><span data-stu-id="bf815-153">owner</span></span>|<span data-ttu-id="bf815-154">String</span><span class="sxs-lookup"><span data-stu-id="bf815-154">String</span></span>|<span data-ttu-id="bf815-155">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="bf815-155">The owner of the app.</span></span>|
|<span data-ttu-id="bf815-156">developer</span><span class="sxs-lookup"><span data-stu-id="bf815-156">developer</span></span>|<span data-ttu-id="bf815-157">String</span><span class="sxs-lookup"><span data-stu-id="bf815-157">String</span></span>|<span data-ttu-id="bf815-158">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="bf815-158">The developer of the app.</span></span>|
|<span data-ttu-id="bf815-159">notes</span><span class="sxs-lookup"><span data-stu-id="bf815-159">notes</span></span>|<span data-ttu-id="bf815-160">String</span><span class="sxs-lookup"><span data-stu-id="bf815-160">String</span></span>|<span data-ttu-id="bf815-161">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="bf815-161">Notes for the app.</span></span>|
|<span data-ttu-id="bf815-162">publishingState</span><span class="sxs-lookup"><span data-stu-id="bf815-162">publishingState</span></span>|[<span data-ttu-id="bf815-163">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bf815-163">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bf815-164">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="bf815-164">The publishing state for the app.</span></span> <span data-ttu-id="bf815-165">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="bf815-165">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bf815-166">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="bf815-166">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf815-167">关系</span><span class="sxs-lookup"><span data-stu-id="bf815-167">Relationships</span></span>
|<span data-ttu-id="bf815-168">关系</span><span class="sxs-lookup"><span data-stu-id="bf815-168">Relationship</span></span>|<span data-ttu-id="bf815-169">类型</span><span class="sxs-lookup"><span data-stu-id="bf815-169">Type</span></span>|<span data-ttu-id="bf815-170">说明</span><span class="sxs-lookup"><span data-stu-id="bf815-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf815-171">categories</span><span class="sxs-lookup"><span data-stu-id="bf815-171">categories</span></span>|<span data-ttu-id="bf815-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bf815-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="bf815-173">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="bf815-173">The list of categories for this app.</span></span>|
|<span data-ttu-id="bf815-174">assignments</span><span class="sxs-lookup"><span data-stu-id="bf815-174">assignments</span></span>|<span data-ttu-id="bf815-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bf815-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="bf815-176">此移动应用的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="bf815-176">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bf815-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf815-177">JSON Representation</span></span>
<span data-ttu-id="bf815-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf815-178">Here is a JSON representation of the resource.</span></span>
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




