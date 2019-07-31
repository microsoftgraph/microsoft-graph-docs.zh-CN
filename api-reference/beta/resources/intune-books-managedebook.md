---
title: managedEBook 资源类型
description: 包含托管电子书基属性的抽象类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c6d39e1a965713054304e7faaf127ab8a735758c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004832"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="7ae49-103">managedEBook 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ae49-103">managedEBook resource type</span></span>

> <span data-ttu-id="7ae49-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7ae49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ae49-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ae49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ae49-106">包含托管电子书基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="7ae49-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="7ae49-107">方法</span><span class="sxs-lookup"><span data-stu-id="7ae49-107">Methods</span></span>
|<span data-ttu-id="7ae49-108">方法</span><span class="sxs-lookup"><span data-stu-id="7ae49-108">Method</span></span>|<span data-ttu-id="7ae49-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7ae49-109">Return Type</span></span>|<span data-ttu-id="7ae49-110">说明</span><span class="sxs-lookup"><span data-stu-id="7ae49-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7ae49-111">List managedEBooks</span><span class="sxs-lookup"><span data-stu-id="7ae49-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="7ae49-112">[managedEBook](../resources/intune-books-managedebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ae49-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="7ae49-113">列出 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7ae49-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="7ae49-114">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="7ae49-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="7ae49-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="7ae49-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="7ae49-116">读取 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7ae49-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="7ae49-117">assign 操作</span><span class="sxs-lookup"><span data-stu-id="7ae49-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="7ae49-118">无</span><span class="sxs-lookup"><span data-stu-id="7ae49-118">None</span></span>|<span data-ttu-id="7ae49-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7ae49-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="7ae49-120">属性</span><span class="sxs-lookup"><span data-stu-id="7ae49-120">Properties</span></span>
|<span data-ttu-id="7ae49-121">属性</span><span class="sxs-lookup"><span data-stu-id="7ae49-121">Property</span></span>|<span data-ttu-id="7ae49-122">类型</span><span class="sxs-lookup"><span data-stu-id="7ae49-122">Type</span></span>|<span data-ttu-id="7ae49-123">说明</span><span class="sxs-lookup"><span data-stu-id="7ae49-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ae49-124">id</span><span class="sxs-lookup"><span data-stu-id="7ae49-124">id</span></span>|<span data-ttu-id="7ae49-125">字符串</span><span class="sxs-lookup"><span data-stu-id="7ae49-125">String</span></span>|<span data-ttu-id="7ae49-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7ae49-126">Key of the entity.</span></span>|
|<span data-ttu-id="7ae49-127">displayName</span><span class="sxs-lookup"><span data-stu-id="7ae49-127">displayName</span></span>|<span data-ttu-id="7ae49-128">字符串</span><span class="sxs-lookup"><span data-stu-id="7ae49-128">String</span></span>|<span data-ttu-id="7ae49-129">电子书的名称。</span><span class="sxs-lookup"><span data-stu-id="7ae49-129">Name of the eBook.</span></span>|
|<span data-ttu-id="7ae49-130">说明</span><span class="sxs-lookup"><span data-stu-id="7ae49-130">description</span></span>|<span data-ttu-id="7ae49-131">String</span><span class="sxs-lookup"><span data-stu-id="7ae49-131">String</span></span>|<span data-ttu-id="7ae49-132">说明。</span><span class="sxs-lookup"><span data-stu-id="7ae49-132">Description.</span></span>|
|<span data-ttu-id="7ae49-133">publisher</span><span class="sxs-lookup"><span data-stu-id="7ae49-133">publisher</span></span>|<span data-ttu-id="7ae49-134">String</span><span class="sxs-lookup"><span data-stu-id="7ae49-134">String</span></span>|<span data-ttu-id="7ae49-135">发布者。</span><span class="sxs-lookup"><span data-stu-id="7ae49-135">Publisher.</span></span>|
|<span data-ttu-id="7ae49-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ae49-136">publishedDateTime</span></span>|<span data-ttu-id="7ae49-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ae49-137">DateTimeOffset</span></span>|<span data-ttu-id="7ae49-138">电子书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7ae49-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="7ae49-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="7ae49-139">largeCover</span></span>|[<span data-ttu-id="7ae49-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7ae49-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7ae49-141">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="7ae49-141">Book cover.</span></span>|
|<span data-ttu-id="7ae49-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ae49-142">createdDateTime</span></span>|<span data-ttu-id="7ae49-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ae49-143">DateTimeOffset</span></span>|<span data-ttu-id="7ae49-144">电子书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7ae49-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="7ae49-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ae49-145">lastModifiedDateTime</span></span>|<span data-ttu-id="7ae49-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ae49-146">DateTimeOffset</span></span>|<span data-ttu-id="7ae49-147">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7ae49-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="7ae49-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7ae49-148">informationUrl</span></span>|<span data-ttu-id="7ae49-149">String</span><span class="sxs-lookup"><span data-stu-id="7ae49-149">String</span></span>|<span data-ttu-id="7ae49-150">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="7ae49-150">The more information Url.</span></span>|
|<span data-ttu-id="7ae49-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7ae49-151">privacyInformationUrl</span></span>|<span data-ttu-id="7ae49-152">String</span><span class="sxs-lookup"><span data-stu-id="7ae49-152">String</span></span>|<span data-ttu-id="7ae49-153">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="7ae49-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ae49-154">关系</span><span class="sxs-lookup"><span data-stu-id="7ae49-154">Relationships</span></span>
|<span data-ttu-id="7ae49-155">关系</span><span class="sxs-lookup"><span data-stu-id="7ae49-155">Relationship</span></span>|<span data-ttu-id="7ae49-156">类型</span><span class="sxs-lookup"><span data-stu-id="7ae49-156">Type</span></span>|<span data-ttu-id="7ae49-157">说明</span><span class="sxs-lookup"><span data-stu-id="7ae49-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ae49-158">类别</span><span class="sxs-lookup"><span data-stu-id="7ae49-158">categories</span></span>|<span data-ttu-id="7ae49-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="7ae49-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="7ae49-160">此电子书的类别列表。</span><span class="sxs-lookup"><span data-stu-id="7ae49-160">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="7ae49-161">assignments</span><span class="sxs-lookup"><span data-stu-id="7ae49-161">assignments</span></span>|<span data-ttu-id="7ae49-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ae49-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="7ae49-163">此电子书的分配列表。</span><span class="sxs-lookup"><span data-stu-id="7ae49-163">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="7ae49-164">installSummary</span><span class="sxs-lookup"><span data-stu-id="7ae49-164">installSummary</span></span>|[<span data-ttu-id="7ae49-165">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7ae49-165">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="7ae49-166">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="7ae49-166">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="7ae49-167">deviceStates</span><span class="sxs-lookup"><span data-stu-id="7ae49-167">deviceStates</span></span>|<span data-ttu-id="7ae49-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ae49-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="7ae49-169">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="7ae49-169">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="7ae49-170">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="7ae49-170">userStateSummary</span></span>|<span data-ttu-id="7ae49-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7ae49-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="7ae49-172">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="7ae49-172">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ae49-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ae49-173">JSON Representation</span></span>
<span data-ttu-id="7ae49-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ae49-174">Here is a JSON representation of the resource.</span></span>
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





