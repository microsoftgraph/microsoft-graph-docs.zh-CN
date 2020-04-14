---
title: managedEBook 资源类型
description: 包含托管电子书基属性的抽象类。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f3bcbd777c87150103fe21495370adddf3afe90
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43403012"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="56bc0-103">managedEBook 资源类型</span><span class="sxs-lookup"><span data-stu-id="56bc0-103">managedEBook resource type</span></span>

<span data-ttu-id="56bc0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56bc0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56bc0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56bc0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56bc0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56bc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56bc0-107">包含托管电子书基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="56bc0-107">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="56bc0-108">方法</span><span class="sxs-lookup"><span data-stu-id="56bc0-108">Methods</span></span>
|<span data-ttu-id="56bc0-109">方法</span><span class="sxs-lookup"><span data-stu-id="56bc0-109">Method</span></span>|<span data-ttu-id="56bc0-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="56bc0-110">Return Type</span></span>|<span data-ttu-id="56bc0-111">说明</span><span class="sxs-lookup"><span data-stu-id="56bc0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="56bc0-112">List managedEBooks</span><span class="sxs-lookup"><span data-stu-id="56bc0-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="56bc0-113">[managedEBook](../resources/intune-books-managedebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56bc0-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="56bc0-114">列出 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56bc0-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="56bc0-115">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="56bc0-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="56bc0-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="56bc0-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="56bc0-117">读取 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56bc0-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="56bc0-118">assign 操作</span><span class="sxs-lookup"><span data-stu-id="56bc0-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="56bc0-119">无</span><span class="sxs-lookup"><span data-stu-id="56bc0-119">None</span></span>|<span data-ttu-id="56bc0-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="56bc0-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="56bc0-121">属性</span><span class="sxs-lookup"><span data-stu-id="56bc0-121">Properties</span></span>
|<span data-ttu-id="56bc0-122">属性</span><span class="sxs-lookup"><span data-stu-id="56bc0-122">Property</span></span>|<span data-ttu-id="56bc0-123">类型</span><span class="sxs-lookup"><span data-stu-id="56bc0-123">Type</span></span>|<span data-ttu-id="56bc0-124">说明</span><span class="sxs-lookup"><span data-stu-id="56bc0-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56bc0-125">id</span><span class="sxs-lookup"><span data-stu-id="56bc0-125">id</span></span>|<span data-ttu-id="56bc0-126">字符串</span><span class="sxs-lookup"><span data-stu-id="56bc0-126">String</span></span>|<span data-ttu-id="56bc0-127">实体的键。</span><span class="sxs-lookup"><span data-stu-id="56bc0-127">Key of the entity.</span></span>|
|<span data-ttu-id="56bc0-128">displayName</span><span class="sxs-lookup"><span data-stu-id="56bc0-128">displayName</span></span>|<span data-ttu-id="56bc0-129">字符串</span><span class="sxs-lookup"><span data-stu-id="56bc0-129">String</span></span>|<span data-ttu-id="56bc0-130">电子书的名称。</span><span class="sxs-lookup"><span data-stu-id="56bc0-130">Name of the eBook.</span></span>|
|<span data-ttu-id="56bc0-131">description</span><span class="sxs-lookup"><span data-stu-id="56bc0-131">description</span></span>|<span data-ttu-id="56bc0-132">String</span><span class="sxs-lookup"><span data-stu-id="56bc0-132">String</span></span>|<span data-ttu-id="56bc0-133">说明。</span><span class="sxs-lookup"><span data-stu-id="56bc0-133">Description.</span></span>|
|<span data-ttu-id="56bc0-134">publisher</span><span class="sxs-lookup"><span data-stu-id="56bc0-134">publisher</span></span>|<span data-ttu-id="56bc0-135">String</span><span class="sxs-lookup"><span data-stu-id="56bc0-135">String</span></span>|<span data-ttu-id="56bc0-136">发布者。</span><span class="sxs-lookup"><span data-stu-id="56bc0-136">Publisher.</span></span>|
|<span data-ttu-id="56bc0-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="56bc0-137">publishedDateTime</span></span>|<span data-ttu-id="56bc0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56bc0-138">DateTimeOffset</span></span>|<span data-ttu-id="56bc0-139">电子书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="56bc0-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="56bc0-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="56bc0-140">largeCover</span></span>|[<span data-ttu-id="56bc0-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="56bc0-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="56bc0-142">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="56bc0-142">Book cover.</span></span>|
|<span data-ttu-id="56bc0-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56bc0-143">createdDateTime</span></span>|<span data-ttu-id="56bc0-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56bc0-144">DateTimeOffset</span></span>|<span data-ttu-id="56bc0-145">电子书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="56bc0-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="56bc0-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56bc0-146">lastModifiedDateTime</span></span>|<span data-ttu-id="56bc0-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56bc0-147">DateTimeOffset</span></span>|<span data-ttu-id="56bc0-148">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="56bc0-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="56bc0-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="56bc0-149">informationUrl</span></span>|<span data-ttu-id="56bc0-150">String</span><span class="sxs-lookup"><span data-stu-id="56bc0-150">String</span></span>|<span data-ttu-id="56bc0-151">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="56bc0-151">The more information Url.</span></span>|
|<span data-ttu-id="56bc0-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="56bc0-152">privacyInformationUrl</span></span>|<span data-ttu-id="56bc0-153">字符串</span><span class="sxs-lookup"><span data-stu-id="56bc0-153">String</span></span>|<span data-ttu-id="56bc0-154">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="56bc0-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56bc0-155">关系</span><span class="sxs-lookup"><span data-stu-id="56bc0-155">Relationships</span></span>
|<span data-ttu-id="56bc0-156">关系</span><span class="sxs-lookup"><span data-stu-id="56bc0-156">Relationship</span></span>|<span data-ttu-id="56bc0-157">类型</span><span class="sxs-lookup"><span data-stu-id="56bc0-157">Type</span></span>|<span data-ttu-id="56bc0-158">说明</span><span class="sxs-lookup"><span data-stu-id="56bc0-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56bc0-159">类别</span><span class="sxs-lookup"><span data-stu-id="56bc0-159">categories</span></span>|<span data-ttu-id="56bc0-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="56bc0-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="56bc0-161">此电子书的类别列表。</span><span class="sxs-lookup"><span data-stu-id="56bc0-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="56bc0-162">assignments</span><span class="sxs-lookup"><span data-stu-id="56bc0-162">assignments</span></span>|<span data-ttu-id="56bc0-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56bc0-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="56bc0-164">此电子书的分配列表。</span><span class="sxs-lookup"><span data-stu-id="56bc0-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="56bc0-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="56bc0-165">installSummary</span></span>|[<span data-ttu-id="56bc0-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="56bc0-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="56bc0-167">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="56bc0-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="56bc0-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="56bc0-168">deviceStates</span></span>|<span data-ttu-id="56bc0-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56bc0-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="56bc0-170">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="56bc0-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="56bc0-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="56bc0-171">userStateSummary</span></span>|<span data-ttu-id="56bc0-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56bc0-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="56bc0-173">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="56bc0-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56bc0-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56bc0-174">JSON Representation</span></span>
<span data-ttu-id="56bc0-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56bc0-175">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```



