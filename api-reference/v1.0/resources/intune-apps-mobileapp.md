---
title: mobileApp 资源类型
description: 包含 Intune 移动应用基属性的抽象类。
ms.openlocfilehash: 7de5450ade7c95984107026eb8a6b19e07a2ba82
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010779"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="61676-103">mobileApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="61676-103">mobileApp resource type</span></span>

> <span data-ttu-id="61676-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="61676-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61676-105">包含 Intune 移动应用基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="61676-105">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="61676-106">方法</span><span class="sxs-lookup"><span data-stu-id="61676-106">Methods</span></span>
|<span data-ttu-id="61676-107">方法</span><span class="sxs-lookup"><span data-stu-id="61676-107">Method</span></span>|<span data-ttu-id="61676-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="61676-108">Return Type</span></span>|<span data-ttu-id="61676-109">说明</span><span class="sxs-lookup"><span data-stu-id="61676-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="61676-110">List mobileApps</span><span class="sxs-lookup"><span data-stu-id="61676-110">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="61676-111">[mobileApp](../resources/intune-apps-mobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="61676-111">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="61676-112">列出 [mobileApp](../resources/intune-apps-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="61676-112">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="61676-113">Get mobileApp</span><span class="sxs-lookup"><span data-stu-id="61676-113">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="61676-114">mobileApp</span><span class="sxs-lookup"><span data-stu-id="61676-114">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="61676-115">读取 [mobileApp](../resources/intune-apps-mobileapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="61676-115">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="61676-116">assign 操作</span><span class="sxs-lookup"><span data-stu-id="61676-116">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="61676-117">无</span><span class="sxs-lookup"><span data-stu-id="61676-117">None</span></span>|<span data-ttu-id="61676-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="61676-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="61676-119">属性</span><span class="sxs-lookup"><span data-stu-id="61676-119">Properties</span></span>
|<span data-ttu-id="61676-120">属性</span><span class="sxs-lookup"><span data-stu-id="61676-120">Property</span></span>|<span data-ttu-id="61676-121">类型</span><span class="sxs-lookup"><span data-stu-id="61676-121">Type</span></span>|<span data-ttu-id="61676-122">说明</span><span class="sxs-lookup"><span data-stu-id="61676-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61676-123">id</span><span class="sxs-lookup"><span data-stu-id="61676-123">id</span></span>|<span data-ttu-id="61676-124">String</span><span class="sxs-lookup"><span data-stu-id="61676-124">String</span></span>|<span data-ttu-id="61676-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="61676-125">Key of the entity.</span></span>|
|<span data-ttu-id="61676-126">displayName</span><span class="sxs-lookup"><span data-stu-id="61676-126">displayName</span></span>|<span data-ttu-id="61676-127">String</span><span class="sxs-lookup"><span data-stu-id="61676-127">String</span></span>|<span data-ttu-id="61676-128">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="61676-128">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="61676-129">description</span><span class="sxs-lookup"><span data-stu-id="61676-129">description</span></span>|<span data-ttu-id="61676-130">String</span><span class="sxs-lookup"><span data-stu-id="61676-130">String</span></span>|<span data-ttu-id="61676-131">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="61676-131">The description of the app.</span></span>|
|<span data-ttu-id="61676-132">publisher</span><span class="sxs-lookup"><span data-stu-id="61676-132">publisher</span></span>|<span data-ttu-id="61676-133">String</span><span class="sxs-lookup"><span data-stu-id="61676-133">String</span></span>|<span data-ttu-id="61676-134">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="61676-134">The publisher of the app.</span></span>|
|<span data-ttu-id="61676-135">largeIcon</span><span class="sxs-lookup"><span data-stu-id="61676-135">largeIcon</span></span>|[<span data-ttu-id="61676-136">mimeContent</span><span class="sxs-lookup"><span data-stu-id="61676-136">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="61676-137">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="61676-137">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="61676-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61676-138">createdDateTime</span></span>|<span data-ttu-id="61676-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61676-139">DateTimeOffset</span></span>|<span data-ttu-id="61676-140">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="61676-140">The date and time the app was created.</span></span>|
|<span data-ttu-id="61676-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61676-141">lastModifiedDateTime</span></span>|<span data-ttu-id="61676-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61676-142">DateTimeOffset</span></span>|<span data-ttu-id="61676-143">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="61676-143">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="61676-144">isFeatured</span><span class="sxs-lookup"><span data-stu-id="61676-144">isFeatured</span></span>|<span data-ttu-id="61676-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="61676-145">Boolean</span></span>|<span data-ttu-id="61676-146">指示应用是否被管理员标记为特色的值。</span><span class="sxs-lookup"><span data-stu-id="61676-146">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="61676-147">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="61676-147">privacyInformationUrl</span></span>|<span data-ttu-id="61676-148">String</span><span class="sxs-lookup"><span data-stu-id="61676-148">String</span></span>|<span data-ttu-id="61676-149">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="61676-149">The privacy statement Url.</span></span>|
|<span data-ttu-id="61676-150">informationUrl</span><span class="sxs-lookup"><span data-stu-id="61676-150">informationUrl</span></span>|<span data-ttu-id="61676-151">String</span><span class="sxs-lookup"><span data-stu-id="61676-151">String</span></span>|<span data-ttu-id="61676-152">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="61676-152">The more information Url.</span></span>|
|<span data-ttu-id="61676-153">owner</span><span class="sxs-lookup"><span data-stu-id="61676-153">owner</span></span>|<span data-ttu-id="61676-154">String</span><span class="sxs-lookup"><span data-stu-id="61676-154">String</span></span>|<span data-ttu-id="61676-155">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="61676-155">The owner of the app.</span></span>|
|<span data-ttu-id="61676-156">developer</span><span class="sxs-lookup"><span data-stu-id="61676-156">developer</span></span>|<span data-ttu-id="61676-157">String</span><span class="sxs-lookup"><span data-stu-id="61676-157">String</span></span>|<span data-ttu-id="61676-158">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="61676-158">The developer of the app.</span></span>|
|<span data-ttu-id="61676-159">notes</span><span class="sxs-lookup"><span data-stu-id="61676-159">notes</span></span>|<span data-ttu-id="61676-160">String</span><span class="sxs-lookup"><span data-stu-id="61676-160">String</span></span>|<span data-ttu-id="61676-161">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="61676-161">Notes for the app.</span></span>|
|<span data-ttu-id="61676-162">publishingState</span><span class="sxs-lookup"><span data-stu-id="61676-162">publishingState</span></span>|[<span data-ttu-id="61676-163">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="61676-163">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="61676-164">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="61676-164">The publishing state for the app.</span></span> <span data-ttu-id="61676-165">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="61676-165">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="61676-166">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="61676-166">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61676-167">Relationships</span><span class="sxs-lookup"><span data-stu-id="61676-167">Relationships</span></span>
|<span data-ttu-id="61676-168">关系</span><span class="sxs-lookup"><span data-stu-id="61676-168">Relationship</span></span>|<span data-ttu-id="61676-169">类型</span><span class="sxs-lookup"><span data-stu-id="61676-169">Type</span></span>|<span data-ttu-id="61676-170">说明</span><span class="sxs-lookup"><span data-stu-id="61676-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61676-171">categories</span><span class="sxs-lookup"><span data-stu-id="61676-171">categories</span></span>|<span data-ttu-id="61676-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="61676-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="61676-173">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="61676-173">The list of categories for this app.</span></span>|
|<span data-ttu-id="61676-174">assignments</span><span class="sxs-lookup"><span data-stu-id="61676-174">assignments</span></span>|<span data-ttu-id="61676-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="61676-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="61676-176">此移动应用的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="61676-176">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61676-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61676-177">JSON Representation</span></span>
<span data-ttu-id="61676-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61676-178">Here is a JSON representation of the resource.</span></span>
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



